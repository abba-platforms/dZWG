# dZWG RESERVE POLICY

## 1. Purpose

This document establishes the full reserve management policy governing Digital Zimbabwe Gold (dZWG). It defines, in complete operational and enforceable terms, how reserve assets are structured, controlled, allocated, verified, safeguarded, and utilized to support the circulating supply of dZWG.

The policy is designed to ensure that reserve management is:

- operationally deterministic  
- quantitatively defined  
- enforceable under governance  
- auditable under institutional standards  
- aligned with liquidity and redemption requirements  
- resilient under normal and stressed market conditions  

This policy serves as the authoritative framework for all reserve-related activities and must be adhered to by all personnel, systems, and counterparties involved in reserve operations.

This document must be read in conjunction with:

- [RESERVE_ATTESTATION.md](./RESERVE_ATTESTATION.md)     
- [CONTROLS.md](./CONTROLS.md)       
- [RISK.md](./RISK.md)      
- [COMPLIANCE.md](./COMPLIANCE.md)     
- [GOVERNANCE.md](./GOVERNANCE.md) 
- [DISCLOSURES.md](./DISCLOSURES.md)     
- [TERMS.md](./TEEMS.md)       

---

## 2. Scope and Applicability

This policy applies to:

- all reserve assets designated to support dZWG  
- all reserve-related banking accounts  
- all on-chain reserve wallets  
- all treasury operations involving reserve movement  
- all issuance and redemption flows  
- all personnel involved in reserve management  
- all third-party custodians and banking partners  

No reserve-related activity may occur outside the boundaries defined in this policy.

---

## 3. Reserve Coverage Objective

### 3.1 Core Requirement

At all times, under normal operating conditions:

Eligible Verified Reserves ≥ Circulating dZWG Supply

This condition must hold continuously and not only at reporting intervals.

---

### 3.2 Target Coverage Ratio

The system targets a reserve coverage ratio between:

100% and 105% of circulating supply

This range is intended to:

- absorb settlement timing mismatches  
- account for operational latency  
- provide minimal liquidity buffer  

---

### 3.3 Threshold Definitions

#### Soft Threshold (Early Warning)
Reserve Ratio: 100% – 101%

Actions:
- increased monitoring  
- restricted issuance discretion  
- enhanced reconciliation frequency  

#### Hard Threshold (Breach)
Reserve Ratio: <100%

Actions:
- immediate halt of all issuance  
- mandatory escalation to governance  
- activation of remediation procedures  

---

## 4. Fundamental Reserve Principles

### 4.1 Capital Preservation

Reserve assets must not be exposed to loss of principal. No reserve asset may be deployed into any instrument or structure that introduces capital risk.

---

### 4.2 Liquidity

Reserve assets must be convertible to usable settlement value without material delay. Liquidity must be sufficient to meet redemption demand under both normal and stressed conditions.

---

### 4.3 Segregation

Reserve assets must be strictly separated from:

- corporate operating funds  
- revenue accounts  
- unrelated treasury activities  

At no point may reserves be commingled with non-reserve funds.

---

### 4.4 Control

All reserve access must be governed by multi-party authorization. No single individual may independently initiate and complete a reserve movement.

---

### 4.5 Transparency

Reserve balances must be:

- measurable  
- reconcilable  
- verifiable  
- attributable to specific accounts or wallets  

---

### 4.6 Prohibition of Yield-Seeking Behavior

Reserve assets must not be used for:

- lending  
- staking  
- liquidity mining  
- speculative trading  
- structured yield strategies  

Reserves exist solely to support redemption and system integrity.

---

## 5. Eligible Reserve Assets

Eligible reserve assets must satisfy all of the following conditions simultaneously:

- immediately available or near-immediately accessible  
- not subject to encumbrance or lien  
- not pledged or collateralized  
- not subject to third-party claims  
- not restricted for unrelated obligations  
- operationally usable for redemption  

### 5.1 Permitted Asset Types

Eligible reserves may include:

- fiat cash balances held in regulated banking institutions  
- custodial balances under verified control  
- liquid digital assets held in designated reserve wallets (subject to governance approval)  

---

## 6. Explicitly Prohibited Reserve Assets

The following must never be included in reserve calculations:

- receivables or unpaid obligations  
- loans extended to any party  
- investments in securities or instruments with maturity risk  
- speculative assets  
- affiliated entity exposures  
- encumbered or pledged funds  
- restricted or frozen balances  

---

## 7. Reserve Composition and Allocation Constraints

### 7.1 Structural Composition

Reserves are divided into:

- Primary Layer: Off-chain fiat reserves  
- Secondary Layer: On-chain reserve assets  

---

### 7.2 Concentration Limits

To reduce counterparty risk, the following limits apply:

- Maximum exposure to a single banking institution: 40% of total reserves  
- Maximum exposure to a single jurisdiction: 60% of total reserves  
- Minimum number of banking counterparties: 2 (where operationally feasible)  

---

## 8. Banking Counterparty Requirements

All banking partners must meet the following minimum criteria:

- legally licensed and regulated financial institution  
- operationally capable of handling settlement flows  
- located in a jurisdiction with acceptable regulatory stability  
- capable of providing account verification and reporting  

Bank counterparties must be periodically reviewed and may be replaced if risk increases.

---

## 9. Treasury Operating Model

### 9.1 Treasury Function

Responsible for:

- reserve allocation  
- execution of reserve movements  
- liquidity planning  
- reconciliation preparation  

---

### 9.2 Finance Function

Responsible for:

- verification of balances  
- certification of reconciliations  
- reporting accuracy  

---

### 9.3 Governance Function

Responsible for:

- policy enforcement  
- approval of major actions  
- escalation decisions  

---

### 9.4 Segregation of Duties

No single function may:

- initiate  
- approve  
- and execute  

the same reserve movement.

---

## 10. Classification of Reserve Movements

All reserve movements must be categorized as:

### 10.1 Issuance Inflows
Funds received corresponding to token minting.

### 10.2 Redemption Outflows
Funds released for token redemption.

### 10.3 Rebalancing Transfers
Movement between reserve accounts or wallets.

### 10.4 Operational Adjustments
Corrections or reconciliation adjustments.

### 10.5 Emergency Movements
Actions taken under stress conditions.

---

## 11. Approval Framework

### 11.1 Standard Movements

Require:
- minimum 2 independent approvals  

---

### 11.2 Large Movements

Require:
- minimum 3 approvals  
- finance validation  

---

### 11.3 Critical or Emergency Movements

Require:
- governance-level approval  
- documented justification  

---

## 12. Issuance Controls

### 12.1 Pre-Issuance Requirement

Before minting dZWG:

- funds must be confirmed received  
- reserves must be verified  

---

### 12.2 Issuance Restrictions

Issuance must not occur if:

- reserves are below threshold  
- reconciliation is incomplete  
- attestation is unavailable  

---

## 13. Redemption Policy

### 13.1 Processing Framework

Redemptions are processed based on:

- compliance clearance  
- liquidity availability  
- operational capacity  

---

### 13.2 Prioritization Logic

Under normal conditions:
- FIFO processing  

Under high volume:
- batch processing  

---

## 14. Liquidity Management

### 14.1 Minimum Liquidity Requirement

A defined portion of reserves must be maintained in immediately accessible form.

---

### 14.2 Intraday Liquidity

Reserves must support:

- same-day processing where feasible  
- predictable settlement timelines  

---

## 15. Stress and Contingency Framework

The system must maintain readiness for:

- redemption surges  
- banking disruptions  
- liquidity shortages  

### 15.1 Contingency Measures

- reserve buffers  
- alternative banking arrangements  
- temporary operational restrictions  

---

## 16. Foreign Exchange and Valuation

All reserves are measured in Zimbabwe Gold (ZWG).

Where equivalent instruments are used:

- valuation must follow a defined methodology  
- reference rates must be consistent  
- FX exposure must be monitored  

---

## 17. Reconciliation Framework

### 17.1 Daily Reconciliation

Performed by treasury and verified by finance.

---

### 17.2 Certification

Finance must certify:

- completeness  
- accuracy  
- consistency  

---

## 18. Breach and Escalation Protocol

### 18.1 Immediate Actions

- halt issuance  
- notify governance  
- initiate investigation  

---

### 18.2 Remediation

- restore reserves  
- rebalance assets  

---

## 19. System Integration

Reserve policy is enforced through:

- smart contract issuance controls  
- reserve update mechanisms  
- oracle-based validation  

---

## 20. Recordkeeping and Audit Trail

All reserve operations must be:

- recorded  
- timestamped  
- auditable  
- retained  

Historical records must be preserved.

---

## 21. Disclosure Framework

Reserve disclosures may include:

- balances  
- composition  
- attestation results  

Disclosure must align with DISCLOSURES.md.

---

## 22. Policy Violations

Violations of this policy may result in:

- suspension of operations  
- governance intervention  
- enforcement actions  

---

## 23. Review and Amendment

This policy may be updated to reflect:

- regulatory developments  
- operational changes  
- governance decisions  

---

## 24. Conclusion

This policy establishes a complete, enforceable, and institutionally aligned reserve management framework for dZWG.

---

## 25. Contact

Abba Payments (Namibia) (Pty) Ltd., Oshakati, Namibia     
security@abbaii.com  

---

End of Document
