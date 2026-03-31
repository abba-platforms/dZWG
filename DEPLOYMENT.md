# dZWG Deployment Summary

## Overview

This document provides the authoritative and complete deployment record for the Digital Zimbabwe Gold (dZWG) smart contract system.

The dZWG system is deployed on-chain using a proxy-based upgradeable architecture. This structure separates user interaction (proxy) from executable logic (implementation), allowing controlled upgrades without changing the primary contract address.

All production deployments, upgrades, and administrative actions are executed under controlled governance and restricted access controls.

This document serves as the single source of truth for:

- contract addresses  
- deployment configuration  
- upgrade architecture  
- administrative control structure  

---

## Network

- **Blockchain Network:** BNB Smart Chain (BSC) Mainnet  
- **Chain ID:** 56  
- **Network Type:** Public EVM-compatible blockchain  
- **RPC Endpoint:** https://bsc-dataseed.binance.org/  

---

## Contract Architecture

The dZWG system is deployed using an upgradeable proxy architecture.

- **Pattern:** UUPS (Universal Upgradeable Proxy Standard)  
- **Standard:** ERC-1967 proxy storage slots  
- **Separation Model:**  
  - Proxy contract: storage + user entry point  
  - Implementation contract: executable logic  

All state (balances, allowances, roles) is stored in the proxy contract, while execution is delegated to the implementation contract via `delegatecall`.

All user-facing interactions must be performed through the proxy contract.

---

## Contract Addresses

### Proxy Contract (Primary Contract)

- **Contract Name:** Digital Zimbabwe Gold  
- **Symbol:** dZWG  
- **Address:**  
  `0xb764383a8A0502c1CF6d58c9de3bA7e5AACdeeA3`  

- **Explorer Link:**  
  https://bscscan.com/address/0xb764383a8A0502c1CF6d58c9de3bA7e5AACdeeA3  

- **Role in System:**  
  - Primary entry point for all user and integration interactions  
  - Maintains all persistent storage  
  - Delegates execution to the implementation contract  

- **Verification Status:**  
  Verified on BscScan  

- **Proxy Type Recognition:**  
  Recognized as ERC-1967 proxy on BscScan  

---

### Implementation Contract (Logic Contract)

- **Contract Name:** dZWG Implementation  
- **Address:**  
  `0x9D596814CcA04A083a470014eacF7eDC2aA531e2`  

- **Explorer Link:**  
  https://bscscan.com/address/0x9D596814CcA04A083a470014eacF7eDC2aA531e2  

- **Role in System:**  
  - Contains executable smart contract logic  
  - Defines token behavior, minting, burning, and administrative controls  
  - Does not store user balances directly  

- **Verification Status:**  
  Verified via matching bytecode and ABI  

---

## Deployment Configuration

- **Solidity Version:** ^0.8.20  
- **EVM Target:** Cancun-compatible compilation  
- **Optimization:** Enabled  
- **Optimization Runs:** Standard production configuration  

- **Dependencies:**  
  - OpenZeppelin Contracts  
  - OpenZeppelin Upgradeable Contracts  
  - Hardhat deployment framework  

---

## Deployment Details

- **Initial Deployment Date:** March 2026  
- **Deployer Address:**  
  `0x75638d9DA050819d4fd298F8a3FbD5b08fCc1799`  

- **Deployment Method:**  
  Hardhat deployment using OpenZeppelin Upgrades (UUPS proxy deployment)  

- **Proxy Initialization:**  
  Executed during deployment via initializer function (no constructor used in upgradeable contract)  

---

## Governance and Administration

The dZWG system operates under controlled administrative governance.

### Administrative Authority

- **Primary Administrative / Multisig Address:**  
  `0x96255a65685086FbeceB1B4aCcd1F8D0E7b1559E`  

### Governance Model

- Role-based access control (RBAC) enforced at contract level  
- Administrative actions restricted to authorized addresses  
- Upgrade authority controlled through designated governance roles  

### Administrative Capabilities

Authorized governance roles may perform the following actions:

- upgrade implementation contract  
- manage system parameters  
- execute mint and burn operations (where applicable)  
- pause or restrict system operations  
- enforce compliance-related controls  

---

## Upgradeability

The system uses the UUPS proxy pattern to support controlled upgrades.

### Upgrade Process

1. A new implementation contract is developed and deployed  
2. The new implementation contract is verified on-chain  
3. Governance initiates upgrade via authorized role  
4. Proxy contract updates its implementation pointer  
5. System continues operating with updated logic  

### Upgrade Constraints

- Storage layout must remain fully compatible  
- Unauthorized upgrades are prevented through access control  
- Upgrade authority is restricted to governance-controlled addresses  

---

## Verification and Transparency

Both proxy and implementation contracts are verified on-chain.

Verification ensures:

- public visibility of contract logic  
- reproducibility of compiled bytecode  
- transparency for auditors, exchanges, and stakeholders  

---

## Interaction Guidelines

- All integrations must use the proxy contract address  
- Direct interaction with the implementation contract is not supported  
- ABI used must correspond to the current implementation logic  
- Wallets, exchanges, and integrations should treat the proxy as the canonical contract  

---

## Operational Notes

- This deployment represents the official production instance of dZWG  
- Any other deployments, forks, or contract instances are not recognized as official  
- All upgrades and administrative actions are executed under controlled governance  

---

## Security Considerations

- Administrative control is restricted to authorized addresses  
- Upgradeability introduces controlled flexibility but requires strict governance  
- Users must rely on verified contract addresses and official documentation  

---

## Disclaimer

This document is provided strictly for technical and informational purposes.

It does not constitute financial, legal, or investment advice.  
Use of the dZWG system is subject to applicable laws, regulations, and operational constraints.

---

End of Document
