# dZWG System Architecture

## 1. Overview

The Digital Zimbabwe Gold (dZWG) system is a blockchain-based digital settlement infrastructure deployed on BNB Smart Chain (BSC). It is designed to represent Zimbabwe Gold (ZiG; ISO code: ZWG) in a programmable, auditable, and transferable on-chain form.

The system is not designed as a speculative asset or investment instrument. It is architected as a controlled issuance and settlement layer that integrates blockchain execution with off-chain financial infrastructure, including banking systems, reserve custody, and compliance processes.

The architecture reflects a hybrid model where:

- transactional state and execution are maintained on-chain  
- financial backing, compliance, and settlement are managed off-chain  

This separation is intentional and fundamental to the system design.

---

## 2. Architectural Rationale

The system architecture is designed to solve three primary constraints:

1. Blockchain provides deterministic execution but cannot natively custody fiat or sovereign reserve assets.
2. Financial systems require compliance, identity, and legal enforcement that cannot be fully encoded on-chain.
3. Upgradeability is required to maintain long-term system relevance and security.

To address these constraints, the architecture is built on:

- proxy-based upgradeability  
- strict role-based governance  
- off-chain reserve custody with on-chain attestation  
- controlled interaction points between financial systems and smart contracts  

---

## 3. Proxy and Upgradeability Architecture

### 3.1 Design Choice

The system uses the UUPS (Universal Upgradeable Proxy Standard) pattern, based on ERC-1967 storage slots.

This design is selected over non-upgradeable contracts to allow:

- security patches  
- feature extensions  
- regulatory adaptations  

without changing the primary contract address.

### 3.2 Structural Separation

The architecture separates execution and storage:

- Proxy contract:
  - stores balances, allowances, roles, and all persistent state  
  - acts as the canonical user-facing contract  

- Implementation contract:
  - contains executable logic  
  - defines all system behavior  

### 3.3 Execution Model

All user interactions are routed through the proxy:

```
User → Proxy → delegatecall → Implementation → Execution → Proxy storage updated
```

The proxy never executes logic directly. It forwards execution context to the implementation contract using `delegatecall`, ensuring that all state mutations occur within proxy storage.

### 3.4 Upgrade Workflow

The upgrade process is controlled and multi-stage:

1. A new implementation contract is developed and deployed.
2. The implementation contract is verified on-chain.
3. A governance-controlled upgrade request is submitted.
4. The implementation is stored as a pending upgrade.
5. A timelock period is enforced.
6. After the timelock expires, the upgrade is executed by an authorized role.
7. The proxy updates its implementation reference.

This prevents immediate or arbitrary upgrades and introduces a review window.

---

## 4. Initialization and Deployment Lifecycle

### 4.1 Constructor Constraint

Upgradeable contracts cannot use constructors because the proxy delegates execution and does not run constructor logic.

### 4.2 Initialization Model

Instead, initialization is performed via an `initialize(...)` function.

This function sets:

- token name and symbol  
- administrative roles  
- governance addresses  
- fee parameters  
- compliance configuration  
- operational thresholds  

### 4.3 Initialization Safety

The initializer is protected by a guard that ensures:

- it can only be executed once  
- re-initialization is prevented  

If initialization is skipped or incorrectly executed, the system may remain unconfigured or vulnerable. Therefore, initialization is considered part of the deployment lifecycle and must be executed atomically with proxy deployment.

---

## 5. Role-Based Governance Architecture

### 5.1 Design Philosophy

The system enforces strict separation of authority using role-based access control. Each role is assigned a narrowly defined scope to reduce risk concentration.

### 5.2 Roles and Responsibilities

#### DEFAULT_ADMIN_ROLE

This role represents the highest authority within the system.

Responsibilities include:

- assigning and revoking roles  
- managing governance structure  
- controlling role hierarchy  

This role is expected to be held by a multisignature governance wallet, not a single externally owned account.

#### UPGRADER_ROLE

This role controls contract upgradeability.

Responsibilities include:

- initiating upgrades  
- executing upgrade transactions  

This role must be isolated from operational roles to prevent unauthorized logic changes.

#### ISSUER_ROLE

This role controls token supply expansion.

Responsibilities include:

- minting tokens in response to reserve inflows  

This role is tied to financial operations and must be tightly controlled.

#### BURNER_ROLE

This role controls supply reduction.

Responsibilities include:

- burning tokens during redemption  
- removing tokens from circulation  

#### COMPLIANCE_ROLE

This role enforces compliance controls.

Responsibilities include:

- freezing accounts  
- restricting transfers  
- managing sanctioned addresses  

#### FEE_ADMIN_ROLE

This role manages economic parameters.

Responsibilities include:

- setting fee rates  
- updating fee collector addresses  

---

## 6. Reserve Attestation Architecture

### 6.1 Design Constraint

Reserves cannot be held on-chain because Zimbabwe Gold (ZWG) exists within traditional financial systems.

### 6.2 Architecture

The system uses an attestation model:

- reserves are held off-chain  
- reserve data is signed by an authorized signer  
- signed data is submitted on-chain  

### 6.3 Attestation Flow

1. Reserve balances are calculated off-chain.
2. A structured payload is created containing:
   - reserve amount  
   - nonce  
   - timestamp or deadline  
3. The payload is signed by an authorized reserve signer.
4. The signed payload is submitted to the contract.
5. The contract verifies:
   - signature authenticity  
   - nonce uniqueness  
   - deadline validity  
6. Valid updates are recorded on-chain.

### 6.4 Integrity Guarantees

- nonce prevents replay attacks  
- deadlines prevent stale updates  
- signer authority ensures data authenticity  

---

## 7. Minting and Supply Alignment

### 7.1 Operational Model

Minting is not arbitrary. It is tied to reserve inflows.

### 7.2 Flow

1. reserves are deposited off-chain  
2. reserve verification occurs  
3. issuer role executes mint  
4. tokens are created and assigned  

### 7.3 Constraint

Minting must remain aligned with reserves to preserve system integrity.

---

## 8. Transfer Fee Architecture

### 8.1 Purpose

Fees are used to support operational sustainability and infrastructure costs.

### 8.2 Calculation Model

- fee is defined in basis points  
- applied at transfer execution  

### 8.3 Execution Flow

1. transfer amount is submitted  
2. fee is calculated  
3. fee portion is redirected to fee collector  
4. remaining amount is transferred  

### 8.4 Governance Control

- fee rate is adjustable  
- fee exemptions may be configured  
- fee collector address is configurable  

---

## 9. Compliance Enforcement Architecture

### 9.1 Design Requirement

The system must support compliance obligations such as AML and sanctions enforcement.

### 9.2 Enforcement Points

Compliance checks are executed before transfer finalization.

### 9.3 Controls

- account freeze  
- blacklist enforcement  
- sanctions restrictions  

### 9.4 Behavior

- restricted accounts cannot send or receive tokens  
- compliance decisions originate off-chain  
- enforcement occurs on-chain  

---

## 10. Redemption Architecture

### 10.1 Hybrid Model

Redemption is a hybrid process involving on-chain and off-chain execution.

### 10.2 Flow

1. user submits redemption request  
2. tokens are transferred for redemption  
3. tokens are burned on-chain  
4. redemption event is recorded  
5. off-chain processing is initiated  
6. fiat or ZWG equivalent is settled  

### 10.3 Properties

- redemption is not instantaneous  
- subject to operational processing  
- fully auditable through on-chain records  

---

## 11. Pause and Emergency Controls

### 11.1 Purpose

Pause functionality exists to respond to:

- security incidents  
- governance compromise  
- regulatory directives  

### 11.2 Behavior

When paused:

- transfers are halted  
- minting and burning may be restricted  
- system enters controlled state  

### 11.3 Recovery

Authorized governance restores normal operation after issue resolution.

---

## 12. On-Chain and Off-Chain Boundary

### 12.1 On-Chain Responsibilities

- token balances  
- transfer execution  
- access control  
- fee logic  
- reserve attestation records  
- upgrade control  
- event emission  

### 12.2 Off-Chain Responsibilities

- reserve custody  
- compliance decision-making  
- banking operations  
- redemption settlement  
- signer management  

### 12.3 Rationale

Certain functions cannot be implemented on-chain due to legal, financial, and operational constraints.

---

## 13. Event and Audit Architecture

### 13.1 Event Emission

All critical actions emit events.

### 13.2 Categories

- mint  
- burn  
- transfer  
- reserve updates  
- compliance changes  
- fee updates  
- redemption events  
- upgrades  

### 13.3 Purpose

Events enable:

- auditability  
- monitoring  
- forensic analysis  
- regulatory reporting  

---

## 14. Failure-State Behavior

### 14.1 Reserve Shortfall

- minting is halted  
- governance intervention required  

### 14.2 Governance Compromise

- system may be paused  
- roles reassigned  

### 14.3 Network Failure

- transactions delayed  
- state remains consistent  

### 14.4 Upgrade Failure

- system continues on previous implementation  

---

## 15. Actor Interaction Model

### 15.1 Retail Users

- hold and transfer tokens  
- interact via wallets  

### 15.2 Institutional Integrators

- integrate for payments and settlement  

### 15.3 Issuer

- manages supply  

### 15.4 Governance

- controls upgrades and parameters  

### 15.5 Reserve Signer

- submits reserve attestations  

### 15.6 Exchanges

- integrate for trading and liquidity  

---

## Conclusion

The dZWG system architecture is designed to provide a controlled, auditable, and upgradeable digital settlement infrastructure that bridges blockchain execution with traditional financial systems.

The architecture prioritizes:

- governance control  
- operational alignment  
- auditability  
- security  
- regulatory compatibility  

---

End of Document
