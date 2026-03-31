# dZWG RESERVE ATTESTATION

## 1. Purpose

This document establishes the comprehensive reserve attestation framework for Digital Zimbabwe Gold (dZWG). It defines the standards, methodologies, eligibility rules, governance structures, assurance levels, verification procedures, disclosure protocols, and limitations applicable to confirming that dZWG is supported by sufficient reserves.

The purpose of this framework is to ensure that reserve verification is:

- methodologically consistent  
- independently verifiable  
- institutionally interpretable  
- aligned with financial assurance practices  
- auditable and reproducible  
- governed under defined control structures  

This document is intended to support:

- centralized exchange (CEX) due diligence  
- banking and custodial counterparties  
- institutional investors and partners  
- regulatory engagement and supervisory review  
- internal governance and treasury controls  

This framework must be read in conjunction with:

- [COMPLIANCE.md](./COMPLIANCE.md)     
- [CONTROLS.md](./CONTROLS.md)      
- [RISK.md](./RISK.md)     
- [DISCLOSURES.md](./DISCLOSURES.md) 
- [TERMS.md](./TERMS.md)      
- [GOVERNANCE.md](./GOVERNANCE.md)     

---

## 2. Definition and Nature of Reserve Attestation

Reserve attestation is a structured, point-in-time verification process designed to confirm that reserve assets designated to support dZWG meet or exceed the circulating token supply under a defined methodology.

Reserve attestation is not inherently equivalent to a full financial audit unless explicitly stated. It is a defined assurance activity with varying levels of rigor depending on the attestation type.

Reserve attestation serves as:

- a verification mechanism for reserve sufficiency  
- a transparency mechanism for stakeholders  
- a control validation layer within the broader system  
- an input into audit and regulatory review processes  

---

## 3. Levels of Attestation and Assurance

Reserve attestation may be conducted under one of the following assurance levels:

### 3.1 Internal Management Attestation

An internal certification issued by authorized treasury and finance functions confirming that:

- reserve balances have been reconciled  
- supply has been accurately determined  
- reserves meet or exceed circulating supply  

This attestation relies on internal controls, reconciliation systems, and management representations.

### 3.2 Independent Limited Assurance Attestation

An engagement conducted by an independent third party providing limited assurance that:

- no material inconsistencies were identified  
- reserve balances reasonably align with reported supply  

This level of assurance does not constitute a full audit and is based on defined procedures.

### 3.3 Agreed-Upon Procedures Engagement

A third-party engagement where:

- specific procedures are executed  
- findings are reported without expressing an assurance opinion  

This form of attestation provides transparency but does not provide assurance conclusions.

### 3.4 Full Audit (If Implemented)

A formal audit conducted under recognized auditing standards, including:

- detailed testing of controls  
- verification of balances  
- audit opinion issuance  

Unless explicitly stated, reserve attestation should not be interpreted as a full audit.

---

## 4. Scope of Attestation

The attestation framework applies to:

- total dZWG token supply  
- circulating supply  
- treasury-controlled allocations  
- reserve assets (on-chain and off-chain)  
- reserve account structures  
- issuance and redemption flows impacting reserves  

The attestation objective is defined as:

Eligible Verified Reserves ≥ Circulating dZWG Supply

at a defined measurement point.

---

## 5. Snapshot and Measurement Framework

### 5.1 Snapshot Definition

Each attestation is conducted at a defined cutoff point consisting of:

- a specific date  
- a specific time  
- a clearly defined timezone  

All measurements must reference the same snapshot.

### 5.2 Supply Measurement

Supply is determined using:

- smart contract totalSupply  
- mint event logs  
- burn event logs  
- treasury allocation tracking  

Circulating supply excludes:

- treasury-held tokens  
- restricted allocations  
- locked or non-circulating balances  

### 5.3 Reserve Measurement

Reserves are measured at the same snapshot and include:

- on-chain wallet balances  
- fiat account balances  
- custodial balances  

### 5.4 Timing Adjustments

Where timing mismatches occur:

- settlement delays must be identified  
- adjustments must be documented  
- material adjustments must be disclosed  

---

## 6. Eligible Reserve Asset Criteria

Only assets meeting strict eligibility criteria may be included in reserve calculations.

Eligible reserve assets must be:

- immediately available or readily accessible  
- liquid or near-liquid  
- not encumbered or pledged  
- not subject to third-party claims  
- not restricted for unrelated obligations  
- operationally usable for redemption  

Examples of eligible reserves include:

- fiat cash balances held in banking institutions  
- verified custodial balances  
- liquid on-chain assets designated as reserves  

Non-eligible assets include:

- receivables  
- loans or credit exposures  
- illiquid investments  
- speculative instruments  
- affiliated entity balances without immediate liquidity  
- pledged or encumbered assets  

---

## 7. Treatment of Encumbered and Restricted Assets

Assets that are:

- pledged  
- subject to lien  
- contractually restricted  
- allocated for unrelated obligations  

must be excluded from eligible reserves unless:

- the restriction is removed  
- or the restriction is explicitly disclosed and adjusted  

Attestation must clearly distinguish:

- gross reserves  
- eligible reserves  

---

## 8. Treatment of Pending Obligations

Reserve calculations must account for obligations that affect reserve availability, including:

- pending redemption requests  
- unsettled banking transactions  
- operational liabilities tied directly to reserve balances  

Attestation methodology must specify whether reserves are reported:

- on a gross basis  
- on a net basis  

The selected basis must be consistently applied and disclosed.

---

## 9. Reserve Composition and Structure

dZWG reserves are structured under a hybrid model:

### 9.1 On-Chain Reserves

- held in designated treasury wallets  
- verifiable via blockchain explorers  
- controlled via multi-signature authorization  

### 9.2 Off-Chain Reserves

- held in regulated banking institutions  
- verified through bank documentation  
- subject to internal and external controls  

---

## 10. Attestation Methodology

The attestation process includes:

### 10.1 Supply Verification

- smart contract inspection  
- event log reconciliation  
- treasury allocation validation  

### 10.2 On-Chain Verification

- wallet balance confirmation  
- cryptographic verification  
- explorer-based validation  

### 10.3 Off-Chain Verification

- bank statements  
- confirmations  
- custodial records  

### 10.4 Reconciliation

- aggregation of eligible reserves  
- comparison against circulating supply  
- identification of discrepancies  

---

## 11. Shortfall Classification and Materiality

Discrepancies are classified as:

### 11.1 Immaterial Discrepancy
Does not impact system integrity or redemption capacity.

### 11.2 Material Discrepancy
May impact confidence or operational capacity.

### 11.3 Critical Shortfall
Eligible Reserves < Circulating Supply

### 11.4 Materiality Determination

Materiality is evaluated based on:

- percentage deviation  
- liquidity impact  
- redemption risk  
- regulatory implications  

---

## 12. Discrepancy Response Framework

### 12.1 Immediate Actions

- suspend issuance  
- initiate investigation  
- notify governance  

### 12.2 Remediation

- inject additional reserves  
- rebalance positions  
- adjust supply if required  

### 12.3 Disclosure

Material discrepancies must be disclosed in accordance with [DISCLOSURES.md](./DISCLOSURES.md).

---

## 13. Attestation Report Requirements

Each attestation report must include:

- reporting date  
- reporting time  
- timezone  
- circulating supply  
- total reserves  
- eligible reserves  
- reserve composition  
- methodology used  
- adjustments applied  
- discrepancies identified  
- classification of discrepancies  
- attestation level  
- identity of attestor  

---

## 14. Attestor Authority and Governance

Internal attestation authority resides with:

- treasury function  
- finance function  
- authorized governance roles  

Responsibilities include:

- accuracy of reporting  
- completeness of data  
- adherence to methodology  

---

## 15. Independence of External Attestors

External attestors must:

- not control reserve assets  
- not participate in treasury operations  
- not have conflicting financial interests  
- operate independently from issuer management  

---

## 16. Attestation Failure, Delay, or Non-Issuance

If attestation cannot be completed:

- issuance may be restricted  
- investigation must be initiated  
- governance must be notified  

Material delays must be disclosed where required.

---

## 17. Proof-of-Reserves Framework

Combines:

- on-chain verification  
- off-chain validation  
- consolidated reporting  

---

## 18. Governance Oversight

Governance is responsible for:

- approving methodology  
- reviewing attestation results  
- enforcing remediation  
- overseeing attestors  

---

## 19. Audit Alignment

Attestation aligns with:

- financial assurance practices  
- audit methodologies  
- internal control frameworks  

---

## 20. Recordkeeping and Archival

All attestation records must be:

- documented  
- version-controlled  
- archived  
- retained for audit and regulatory review  

---

## 21. Disclosure and Publication

Attestation results may be published through:

- repository updates  
- official communications  
- institutional reporting  

---

## 22. Denomination and Valuation Policy

Reserves are measured in Zimbabwe Gold (ZWG) terms.

Where equivalent instruments are used:

- valuation methodology must be defined  
- reference rates must be disclosed  

---

## 23. On-Chain Data Freshness

Reserve data must be current.

If data becomes stale:

- updates must be submitted  
- discrepancies evaluated  
- issuance may be restricted  

---

## 24. Limitations of Attestation

Attestation does not guarantee:

- future solvency  
- uninterrupted redemption  
- absence of systemic risk  
- immunity from banking failure  
- regulatory stability  

---

## 25. User Interpretation

Users must understand:

- attestation is point-in-time  
- not continuous assurance  
- must be read with full documentation  

---

## 26. Conclusion

This framework establishes a complete, structured, and institutionally aligned reserve attestation system for dZWG.

---

## 27. Contact

Abba Payments (Namibia) (Pty) Ltd  
security@abbaii.com  

---

End of Document
