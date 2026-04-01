# Digital Zimbabwe Gold (dZWG)

![Zimbabwe Flag](https://upload.wikimedia.org/wikipedia/commons/6/6a/Flag_of_Zimbabwe.svg)

## Project Details

<!-- Project Badges -->
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Token Type](https://img.shields.io/badge/Token-BEP--20-blue.svg)
![Status](https://img.shields.io/badge/Status-Active-success.svg)
![Build](https://img.shields.io/badge/Build-Upgradeable%20UUPS-orange.svg)
![Creator](https://img.shields.io/badge/Creator-Simon%20Kapenda-lightgrey.svg)

---

**Token Name:** Digital Zimbabwe Gold (ZiG; ISO code: ZWG)     
**Token Symbol:** dZWG  
**Token Type:** BEP-20 Upgradeable  
**Total Supply:** Elastic, based on ZiG maximum supply     
**Creator:** [Simon Kapenda](https://linkedin.com/in/simonkapenda)       
**Version:** 1.2  
**Date:** September 17, 2025   
**Updated:** March 31, 2026     

---

## Deployment Status

Digital Zimbabwe Gold (dZWG) has been deployed to **BNB Smart Chain Mainnet** under a production-oriented upgradeable contract structure.

The current deployment status is as follows:

- **Network:** BNB Smart Chain (BSC) Mainnet  
- **Chain ID:** 56  
- **Token Name:** Digital Zimbabwe Gold  
- **Token Symbol:** dZWG  

### Contract Addresses

- **Proxy Contract (Primary User-Facing Contract):**          
  [0xb764383a8A0502c1CF6d58c9de3bA7e5AACdeeA3](https://bscscan.com/token/0xb764383a8A0502c1CF6d58c9de3bA7e5AACdeeA3)

- **Implementation Contract (Underlying Logic Contract):**         
  [0x9D596814CcA04A083a470014eacF7eDC2aA531e2](https://bscscan.com/token/0x9D596814CcA04A083a470014eacF7eDC2aA531e2#code)

### Deployment Structure

The dZWG system is deployed under an upgradeable architecture in which:

- the **proxy contract** serves as the canonical contract address for user interaction, wallet integration, exchange integration, and operational use; and  
- the **implementation contract** contains the executable logic referenced by the proxy under the defined upgrade framework.  

Accordingly, all production-facing integrations should reference the **proxy contract address** as the authoritative dZWG contract address.

### Verification Status

The implementation contract has been matched successfully at the bytecode and ABI level, supporting technical traceability and deployment integrity review.

For complete deployment architecture, governance context, and operational interpretation of these addresses, refer to [DEPLOYMENT.md](DEPLOYMENT.md).

---

## Executive Summary    

Digital Zimbabwe Gold (dZWG) is a blockchain-native digital settlement system designed to represent Zimbabwe Gold (ZiG; ISO code: ZWG) on-chain at a fixed parity of one dZWG to one ZWG in tokenized form under a controlled, 100% reserve-backed, compliance-aware operating framework.

dZWG is designed as a private digital payment and settlement instrument. It is intended to support programmable transfer, controlled issuance, governed redemption workflows, compliance-aware participation, and reserve-linked operation within a hybrid architecture that combines on-chain smart contracts with off-chain governance, treasury, reserve management, compliance, reconciliation, and legal controls.

dZWG is issued and operated by:

**Abba Payments (Namibia) (Pty) Ltd**, a wholly-owned subsidiary of [Abba Industries](https://abbaii.com/).     

dZWG is **not**:

- legal tender  
- issued by the Reserve Bank of Zimbabwe  
- a central bank digital currency  
- a bank deposit  
- a securities offering  
- an equity instrument  
- a debt instrument  
- a collective investment scheme  
- a sovereign monetary instrument  
- a risk-free product  

This repository contains the institutional documentation, governance framework, reserve framework, compliance structure, controls model, risk framework, disclosure layer, security framework, audit framework, and legal usage terms for dZWG.

---

## 1. Repository Purpose

This repository is intended to serve as the authoritative institutional documentation and technical reference base for dZWG.

The repository is structured to support review by:

- centralized exchanges (CEXs)  
- banking and custody partners  
- institutional counterparties  
- auditors  
- compliance and risk teams  
- governance participants  
- technical reviewers  
- regulators and supervisory stakeholders, where relevant  

This repository is not organized as a lightweight marketing package. It is organized as a formal operating, governance, reserve, compliance, risk, security, and assurance framework for a reserve-backed digital financial infrastructure system.

The documentation is intended to make the following clear:

- what dZWG is  
- what dZWG is not  
- how the system is structured  
- how the system is governed  
- how issuance and reserves are controlled  
- how compliance is enforced  
- how security is managed  
- how risks are identified and mitigated  
- how legal and operational limitations are disclosed  
- how institutional users should interpret the system  

---

## 2. Repository Navigation

The repository is organized into a set of linked institutional documents. Each document has a defined role in the overall system description.

### 2.1 Core System and Governance Documents

- [WHITEPAPER.md](WHITEAPPER.md)    
- [ARCHITECTURE.md](ARCHITECTURE.md)  
- [GOVERNANCE.md](GOVERNANCE.md)  
- [DEPLOYMENT.md](DEPLOYMENT.md)  

### 2.2 Risk, Control, and Security Documents

- [RISK.md](RISK.md)  
- [CONTROLS.md](CONTROLS.md)  
- [SECURITY.md](SECURITY.md)  

### 2.3 Compliance, Legal, and Disclosure Documents

- [COMPLIANCE.md](COMPLIANCE.md)  
- [DISCLOSURES.md](DISCLOSURES.md)  
- [TERMS.md](TERMS.md)  
- [DISCLAIMER.md](DISCLAIMER.md)  

### 2.4 Reserve, Treasury, and Assurance Documents

- [RESERVE_POLICY.md](RESERVE_POLICY.md)  
- [RESERVE_ATTESTATION.md](RESERVE_ATTESTATION.md)  

### 2.5 Audit and Review Documents

- [AUDIT_SCOPE.md](AUDIT_SCOPE.md)  
- [AUDIT_REPORT.md](AUDIT_REPORT.md)  

### 2.6 Contribution and Security Reporting Documents

- [CONTRIBUTING.md](CONTRIBUTING.md)  
- [SECURITY.md](SECURITY.md)  

This repository is designed to be read as an integrated documentation stack. No single file should be treated as a complete substitute for the others where detailed reliance is required.

---

## 3. How to Read This Repository

Different institutional readers typically need a different reading sequence. The following reading paths are recommended.

### 3.1 For Centralized Exchanges

Recommended reading order:

1. [README.md](README.md)
2. [WHITEPAPER.md](WHITEAPPER.md)    
3. [DISCLOSURES.md](DISCLOSURES.md)  
4. [COMPLIANCE.md](COMPLIANCE.md)  
5. [AUDIT_REPORT.md](AUDIT_REPORT.md)  
6. [RESERVE_ATTESTATION.md](RESERVE_ATTESTATION.md)  
7. [SECURITY.md](SECURITY.md)  
8. [DEPLOYMENT.md](DEPLOYMENT.md)  

### 3.2 For Banks and Custodians

Recommended reading order:

1. [README.md](README.md)
2. [WHITEPAPER.md](WHITEAPPER.md)    
3. [RESERVE_POLICY.md](RESERVE_POLICY.md)  
4. [RESERVE_ATTESTATION.md](RESERVE_ATTESTATION.md)  
5. [COMPLIANCE.md](COMPLIANCE.md)  
6. [TERMS.md](TERMS.md)  
7. [DISCLOSURES.md](DISCLOSURES.md)  
8. [GOVERNANCE.md](GOVERNANCE.md)  

### 3.3 For Auditors and Technical Reviewers

Recommended reading order:

1. [README.md](README.md)  
2. [ARCHITECTURE.md](ARCHITECTURE.md)  
3. [GOVERNANCE.md](GOVERNANCE.md)  
4. [CONTROLS.md](CONTROLS.md)  
5. [SECURITY.md](SECURITY.md)  
6. [AUDIT_SCOPE.md](AUDIT_SCOPE.md)  
7. [AUDIT_REPORT.md](AUDIT_REPORT.md)  
8. [DEPLOYMENT.md](DEPLOYMENT.md)  
9. [RESERVE_POLICY.md](RESERVE_POLICY.md)  
10. [RESERVE_ATTESTATION.md](RESERVE_ATTESTATION.md)  

### 3.4 For Regulators and Supervisory Readers

Recommended reading order:

1. [README.md](README.md)
2. [WHITEPAPER.md](WHITEAPPER.md)    
3. [DISCLOSURES.md](DISCLOSURES.md)  
4. [COMPLIANCE.md](COMPLIANCE.md)  
5. [TERMS.md](TERMS.md)  
6. [GOVERNANCE.md](GOVERNANCE.md)  
7. [RESERVE_POLICY.md](RESERVE_POLICY.md)  
8. [RESERVE_ATTESTATION.md](RESERVE_ATTESTATION.md)  
9. [AUDIT_REPORT.md](AUDIT_REPORT.md)  

### 3.5 For Governance and Internal Operations

Recommended reading order:

1. [README.md](README.md)
2. [WHITEPAPER.md](WHITEAPPER.md)    
3. [GOVERNANCE.md](GOVERNANCE.md)  
4. [CONTROLS.md](CONTROLS.md)  
5. [RISK.md](RISK.md)  
6. [SECURITY.md](SECURITY.md)  
7. [RESERVE_POLICY.md](RESERVE_POLICY.md)  
8. [COMPLIANCE.md](COMPLIANCE.md)  
9. [AUDIT_REPORT.md](AUDIT_REPORT.md)  

---

## 4. System Overview

dZWG is built around a simple core proposition:

**a digitally transferable unit representing Zimbabwe Gold (ZiG; ISO code: ZWG) value within a controlled reserve-backed framework**

That core proposition is implemented through a broader institutional structure that includes:

- a smart contract layer for issuance, transfer, burning, access control, pause controls, and upgradeability  
- a governance layer for role control, upgrades, emergency actions, and authority segregation  
- a reserve layer for backing, reserve policy, reserve attestation, reconciliation, and reserve risk management  
- a compliance layer for KYC/AML, sanctions controls, transaction restrictions, and jurisdictional risk handling  
- a controls layer for approvals, reconciliations, evidence retention, exceptions, and escalation  
- a legal and disclosures layer for system classification, user responsibilities, non-affiliation clarity, and use restrictions  
- an audit and assurance layer for internal review structure and institutional readiness documentation  

The result is not merely a token contract. It is a documented and controlled digital settlement architecture.

---

## 5. System Classification

dZWG is classified in this repository as a:

**privately issued, reserve-backed, blockchain-native digital payment and settlement instrument**

This classification is important because it distinguishes dZWG from categories that it is not intended to fall within.

### 5.1 dZWG Is Not Sovereign Money

dZWG is not issued by the Reserve Bank of Zimbabwe and is not an official monetary instrument of the Zimbabwean state.

### 5.2 dZWG Is Not a CBDC

dZWG is not a central bank digital currency and should not be interpreted as one.

### 5.3 dZWG Is Not a Deposit Product

Holding dZWG does not create a bank account, savings account, or depositor relationship with the issuer.

### 5.4 dZWG Is Not an Investment Security

Holding dZWG does not confer ownership rights, profit participation, dividend rights, or equity interest in the issuer.

### 5.5 dZWG Is Not Risk-Free

Although dZWG is reserve-backed by design, its operation depends on governance, reserves, banking relationships, infrastructure, compliance controls, and legal conditions. Those dependencies create residual risk, all of which is addressed throughout this repository.

---

## 6. Non-Affiliation and Regulatory Positioning

This repository takes a clear and explicit position on the legal and institutional characterization of dZWG.

dZWG is:

- privately issued  
- reserve-backed by design  
- governed under a controlled institutional framework  
- intended for digital payment and settlement use  

dZWG is not:

- issued by the Reserve Bank of Zimbabwe  
- endorsed by the Reserve Bank of Zimbabwe  
- a CBDC  
- legal tender  
- evidence of regulatory approval by default  

Nothing in this repository should be interpreted as implying that the existence of this documentation stack, reserve framework, or compliance structure constitutes formal approval, licensing, or endorsement by a central bank, regulator, or government unless such approval is separately obtained and explicitly disclosed.

---

## 7. Core Design Principles

The dZWG system is built around several core principles.

### 7.1 Reserve Discipline

The system is intended to operate with eligible reserves at or above circulating dZWG supply under normal operating conditions.

### 7.2 Controlled Issuance

New issuance must occur only through authorized roles and within the reserve-linked operating framework.

### 7.3 Controlled Redemption

Redemption, where available, is not an uncontrolled public withdrawal right. It is a governed, compliance-aware operational process supported by reserves and subject to policy and legal constraints.

### 7.4 Governance Segregation

Critical powers are separated across governance, treasury, compliance, and security functions to reduce unilateral risk.

### 7.5 Compliance-Aware Operation

The system is designed to support KYC, AML, sanctions controls, transaction restrictions, and jurisdiction-sensitive enforcement.

### 7.6 Upgradeable but Controlled Architecture

The system may use upgradeable smart contract architecture, but upgradeability is intended to be constrained by governance, authorization, and emergency controls.

### 7.7 Institutional Documentation Discipline

The system is documented in a way that supports audit, review, and due diligence rather than relying on informal explanation.

---

## 8. System Boundaries

A proper institutional understanding of dZWG requires a clear distinction between the on-chain system boundary and the off-chain operating boundary.

### 8.1 On-Chain Boundary

The on-chain boundary may include:

- token contract logic  
- mint and burn functions  
- access control roles  
- pause and emergency controls  
- upgradeable proxy and implementation logic where used  
- signed input validation or reserve-update-related control logic where applicable  
- event logging and transaction state transitions  

### 8.2 Off-Chain Boundary

The off-chain boundary includes:

- reserve custody and treasury operations  
- reserve reconciliation and reserve attestation workflows  
- compliance screening and user onboarding  
- governance decision-making and approvals  
- legal and regulatory interpretation  
- banking and settlement relationships  
- incident response and operational escalation  

### 8.3 Why the Boundary Matters

A fully on-chain system cannot by itself:

- hold fiat banking balances  
- perform legal identity verification  
- satisfy jurisdiction-specific compliance obligations  
- settle off-chain redemptions  
- execute banking relationships  
- operate institutional approval processes  

For this reason, dZWG is intentionally designed as a hybrid system rather than a purely on-chain token experiment.

---

## 9. Architecture Summary

The dZWG architecture is documented in detail in [ARCHITECTURE.md](ARCHITECTURE.md). The key architectural principle is the coexistence of deterministic on-chain logic with governed off-chain financial and operational processes.

### 9.1 On-Chain Layer

The on-chain layer is responsible for deterministic enforcement of the parts of the system that can and should be encoded directly in smart contract form.

This may include:

- token issuance logic  
- transfer logic  
- burn logic  
- role enforcement  
- emergency controls  
- upgrade controls  
- event logging  

### 9.2 Off-Chain Layer

The off-chain layer is responsible for the parts of the system that cannot be reduced to smart contract logic alone.

This includes:

- reserve custody  
- reserve movement approval  
- reconciliation  
- compliance review  
- legal interpretation  
- banking settlement  
- governance approvals  

### 9.3 Production and Deployment Context

Deployment context, contract addresses, network assumptions, and production structure are documented in [DEPLOYMENT.md](DEPLOYMENT.md).

The README is not the authoritative deployment record. It serves as an overview only. Reliance for deployment-specific details should be placed on [DEPLOYMENT.md](DEPLOYMENT.md).

---

## 10. Governance Model

The governance model for dZWG is documented in detail in [GOVERNANCE.md](GOVERNANCE.md), but the central principles are summarized here.

### 10.1 Centralized but Controlled

dZWG is not governed by a DAO and is not designed for anonymous token-holder governance.

It is governed through a controlled institutional model centered on:

- defined roles  
- restricted authority boundaries  
- governance-controlled upgrades  
- multisignature or equivalent protected approval structures  
- escalation and emergency powers  

### 10.2 Role Separation

The governance structure separates authority across domains such as:

- governance and upgrade authority  
- treasury and reserve-linked execution  
- compliance enforcement  
- security and incident response  

### 10.3 Governance Purpose

The purpose of the governance framework is to ensure that:

- critical actions are not unilateral  
- reserve-linked operations remain constrained  
- security actions can be taken when necessary  
- compliance decisions can be enforced  
- the system can adapt responsibly to new conditions  

---

## 11. Reserve Framework

The reserve framework is one of the core pillars of dZWG.

### 11.1 Reserve Objective

The reserve system is designed to maintain:

**Eligible Verified Reserves >= Circulating dZWG Supply**

This principle is defined, quantified, and operationalized through:

- [RESERVE_POLICY.md](RESERVE_POLICY.md)  
- [RESERVE_ATTESTATION.md](RESERVE_ATTESTATION.md)  

### 11.2 Reserve Composition

The reserve structure is documented as a hybrid model that may include:

- off-chain fiat reserves held in regulated banking institutions  
- on-chain reserve-designated assets where applicable and approved  

### 11.3 Eligible vs Non-Eligible Reserves

The reserve framework distinguishes between:

- eligible reserve assets  
- non-eligible assets  
- encumbered assets  
- restricted balances  
- operational funds that must not be treated as reserves  

### 11.4 Reserve Governance

Reserve operations are governed through:

- treasury function controls  
- finance verification  
- reconciliation procedures  
- discrepancy escalation  
- governance oversight  

### 11.5 Why the Reserve Framework Matters

For a reserve-backed digital settlement instrument, reserve policy is not supplementary documentation. It is a core part of system legitimacy, user confidence, exchange acceptability, and institutional due diligence.

---

## 12. Reserve Attestation Framework

Reserve attestation is documented separately in [RESERVE_ATTESTATION.md](RESERVE_ATTESTATION.md).

Its purpose is to define how reserve sufficiency is verified and reported.

### 12.1 Point-in-Time Verification

Reserve attestation is a point-in-time verification mechanism. It is not a guarantee of perpetual solvency, but a structured and documented confirmation of reserve sufficiency at a defined measurement point.

### 12.2 Attestation Types

The framework contemplates multiple forms of attestation, including:

- management attestation  
- limited assurance style third-party review  
- agreed-upon procedures engagement  
- full audit, where separately performed  

### 12.3 What Attestation Does

The attestation framework is designed to:

- measure circulating supply  
- measure eligible reserves  
- apply a defined methodology  
- classify discrepancies  
- support disclosure and governance action where required  

### 12.4 What Attestation Does Not Do

Attestation does not eliminate:

- future market or operational risk  
- banking counterparty risk  
- governance risk  
- jurisdictional or regulatory change risk  

These limitations are acknowledged openly in the repository.

---

## 13. Compliance Framework

Compliance is documented in detail in [COMPLIANCE.md](COMPLIANCE.md).

### 13.1 Hybrid Compliance Structure

The compliance model has two major components:

- off-chain compliance decision layer  
- on-chain compliance enforcement layer  

### 13.2 Off-Chain Compliance Activities

These may include:

- KYC onboarding  
- AML review  
- sanctions screening  
- transaction monitoring  
- policy interpretation  
- case management and escalation  

### 13.3 On-Chain Enforcement Activities

These may include:

- account restrictions  
- freeze controls  
- transfer limitations  
- blocked participation in governed processes  

### 13.4 Compliance Goal

The compliance framework is intended to make dZWG:

- legally aware  
- enforcement-capable  
- regulator-readable  
- institutionally acceptable for controlled use  

It is not designed as a token system that ignores legal reality.

---

## 14. Controls Framework

The system control environment is documented in [CONTROLS.md](CONTROLS.md).

### 14.1 Why Controls Matter

Policies and architecture are not enough unless they are paired with enforceable controls.

The controls framework addresses:

- who approves  
- who executes  
- what evidence is retained  
- how reconciliation occurs  
- how incidents are escalated  
- how exceptions are handled  
- how control failures are addressed  

### 14.2 Control Types

The control environment includes:

- preventive controls  
- detective controls  
- corrective controls  

### 14.3 Audit-Grade Orientation

The controls documentation is written to support:

- internal review  
- exchange due diligence  
- institutional counterparty review  
- audit mapping and evidence logic  

---

## 15. Risk Framework

The dZWG risk framework is documented in [RISK.md](RISK.md).

### 15.1 Risk Domains Addressed

The framework addresses multiple domains, including:

- smart contract risk  
- upgradeability risk  
- governance risk  
- reserve and financial risk  
- operational risk  
- compliance and regulatory risk  
- liquidity and redemption risk  
- counterparty risk  
- dependency and infrastructure risk  
- reputational risk  

### 15.2 Why Risk Documentation Matters

Institutional stakeholders do not expect a serious financial system to claim "no risk." They expect it to identify, classify, disclose, and mitigate risk. This repository follows that expectation.

### 15.3 Residual Risk

The documentation does not pretend that all risk can be eliminated. It distinguishes between:

- controlled risk  
- mitigated risk  
- residual risk  

That distinction is important for credibility.

---

## 16. Security Framework

Security is documented in [SECURITY.md](SECURITY.md).

### 16.1 Security Is Not Just Bug Reporting

The security framework extends beyond vulnerability disclosure. It includes:

- smart contract security architecture  
- role-based security boundaries  
- multisignature or equivalent authorization assumptions  
- key compromise handling principles  
- incident response structure  
- emergency controls  
- dependency risk acknowledgment  
- security limitations and residual risk  

### 16.2 Security and Governance Interdependence

In dZWG, security is not isolated from governance. Governance integrity, reserve controls, and emergency procedures are part of the security model.

### 16.3 Security Appendix Integration

The security documentation has been expanded to include architectural and control appendices so that the system is not described at a superficial level.

---

## 17. Disclosure Layer

dZWG disclosures are documented in [DISCLOSURES.md](DISCLOSURES.md).

### 17.1 Purpose of Disclosures

The disclosure layer exists to ensure that users, counterparties, exchanges, and institutional reviewers understand:

- what dZWG is  
- what rights dZWG does not create  
- what risks remain  
- what dependencies exist  
- what limitations apply  

### 17.2 Non-Affiliation and Non-Misrepresentation

The disclosures make clear that dZWG is not affiliated with the Reserve Bank of Zimbabwe and is not a sovereign product.

### 17.3 User Interpretation Discipline

Disclosures are designed to prevent:

- overstatement  
- misclassification  
- false assumptions about rights or guarantees  

---

## 18. Terms of Use

The legal usage framework is documented in [TERMS.md](TERMS.md).

### 18.1 Role of Terms

The terms document defines:

- eligibility  
- user responsibilities  
- prohibited uses  
- no-custody position  
- reserve and redemption legal treatment  
- limitations of liability  
- suspension and termination rights  
- governing law  
- dispute framework  
- survival and enforcement clauses  

### 18.2 Why Terms Matter

A repository that aspires to institutional use cannot rely only on technical and policy documents. It also needs a clear legal usage boundary.

---

## 19. Audit Framework and Audit Report

The repository includes:

- [AUDIT_SCOPE.md](AUDIT_SCOPE.md)  
- [AUDIT_REPORT.md](AUDIT_REPORT.md)  

### 19.1 Audit Scope

The audit scope document defines what should be reviewed in relation to:

- smart contracts  
- governance  
- reserve and treasury assumptions  
- compliance controls  
- security design  
- control environment  
- remediation process  
- evidence and reporting standards  

### 19.2 Audit Report

The audit report documents the internal OpenZeppelin-style production-grade review completed on the dZWG system.

As currently documented, that internal review concluded:

- approximately **9.2 / 10**  
- **0 critical findings**  
- **0 high findings**  
- strong production readiness subject to documented residual risks and limitations  

### 19.3 Internal vs Independent Audit

The audit report is explicitly classified as an internal audit artifact. It is not misrepresented as an independent third-party opinion.

---

## 20. Deployment and Production Context

Deployment context is documented in [DEPLOYMENT.md](DEPLOYMENT.md).

### 20.1 What Deployment Documentation Covers

The deployment file identifies:

- network context  
- contract deployment model  
- proxy and implementation relationships where applicable  
- governance or administrative structure  
- production deployment assumptions  

### 20.2 Why Deployment Documentation Matters

Institutional review of a tokenized financial system requires clarity not only about code, but also about where and how that code is deployed and controlled.

---

## 21. Official Sources of Truth

This repository contains multiple documents, but different documents are authoritative for different domains.

### 21.1 System Design and Architecture

Primary source of truth:
- [ARCHITECTURE.md](ARCHITECTURE.md)

### 21.2 Governance and Authority Structure

Primary source of truth:
- [GOVERNANCE.md](GOVERNANCE.md)

### 21.3 Deployment, Network, and Contract Address References

Primary source of truth:
- [DEPLOYMENT.md](DEPLOYMENT.md)

### 21.4 Risk Classification and Residual Risk Framing

Primary source of truth:
- [RISK.md](RISK.md)

### 21.5 Operational Controls and Control Ownership

Primary source of truth:
- [CONTROLS.md](CONTROLS.md)

### 21.6 Compliance and Enforcement Structure

Primary source of truth:
- [COMPLIANCE.md](COMPLIANCE.md)

### 21.7 Security Architecture and Security Reporting

Primary source of truth:
- [SECURITY.md](SECURITY.md)

### 21.8 Reserve Management Rules

Primary source of truth:
- [RESERVE_POLICY.md](RESERVE_POLICY.md)

### 21.9 Reserve Verification and Attestation Logic

Primary source of truth:
- [RESERVE_ATTESTATION.md](RESERVE_ATTESTATION.md)

### 21.10 Legal Disclosures and Interpretive Limitations

Primary sources of truth:
- [DISCLOSURES.md](DISCLOSURES.md)  
- [DISCLAIMER.md](DISCLAIMER.md)  

### 21.11 Terms of Use and Legal Usage Restrictions

Primary source of truth:
- [TERMS.md](TERMS.md)

### 21.12 Audit Structure and Audit Result

Primary sources of truth:
- [AUDIT_SCOPE.md](AUDIT_SCOPE.md)  
- [AUDIT_REPORT.md](AUDIT_REPORT.md)  

Where a reader requires detailed reliance, the specialist document for that subject should be preferred over the README.

---

## 22. Current System Status

The current repository position, as documented, is as follows.

### 22.1 Documentation Stack Status

The repository includes a full institutional documentation stack across:

- architecture  
- governance  
- controls  
- risk  
- compliance  
- security  
- reserve policy  
- reserve attestation  
- audit scope  
- audit report  
- legal disclosures and terms  

### 22.2 Internal Audit Status

The repository includes an internal OpenZeppelin-style production-grade audit report in [AUDIT_REPORT.md](AUDIT_REPORT.md).

### 22.3 Reserve Framework Status

The reserve management framework is defined in [RESERVE_POLICY.md](RESERVE_POLICY.md), and the reserve verification framework is defined in [RESERVE_ATTESTATION.md](RESERVE_ATTESTATION.md).

### 22.4 Governance Status

The governance framework is defined in [GOVERNANCE.md](GOVERNANCE.md).

### 22.5 Compliance Status

The compliance framework is defined in [COMPLIANCE.md](COMPLIANCE.md).

### 22.6 Deployment Status

Deployment context and deployment references are documented in [DEPLOYMENT.md](DEPLOYMENT.md).

### 22.7 Independent External Audit Status

Any independent external audit or external reserve assurance should not be assumed unless explicitly documented in the repository through an official document or disclosure.

---

## 23. Repository Document Index

The following documents form the core institutional stack of this repository.

### 23.1 Core System and Governance

- [ARCHITECTURE.md](ARCHITECTURE.md)  
- [GOVERNANCE.md](GOVERNANCE.md)  
- [DEPLOYMENT.md](DEPLOYMENT.md)  

### 23.2 Risk, Control, and Security

- [RISK.md](RISK.md)  
- [CONTROLS.md](CONTROLS.md)  
- [SECURITY.md](SECURITY.md)  

### 23.3 Compliance and Legal

- [COMPLIANCE.md](COMPLIANCE.md)  
- [DISCLOSURES.md](DISCLOSURES.md)  
- [TERMS.md](TERMS.md)  
- [DISCLAIMER.md](DISCLAIMER.md)  

### 23.4 Reserve and Financial Integrity

- [RESERVE_POLICY.md](RESERVE_POLICY.md)  
- [RESERVE_ATTESTATION.md](RESERVE_ATTESTATION.md)  

### 23.5 Audit and Assurance

- [AUDIT_SCOPE.md](AUDIT_SCOPE.md)  
- [AUDIT_REPORT.md](AUDIT_REPORT.md)  

### 23.6 Contribution and Security Reporting

- [CONTRIBUTING.md](CONTRIBUTING.md)  
- [SECURITY.md](SECURITY.md)  

These documents are intended to be read together, not in isolation.

---

## 24. Repository Use and Interpretation

This repository should be used as:

- a system reference  
- a due diligence package  
- a governance and controls record  
- a technical and institutional explanation base  

It should not be used as:

- investment promotion  
- legal advice  
- tax advice  
- a guarantee of future performance  
- a substitute for independent professional review where one is required  

### 24.1 For Exchanges

Exchanges may use this repository to review:

- token classification  
- control architecture  
- governance  
- reserve handling  
- audit structure  
- disclosure adequacy  

### 24.2 For Banks and Custodians

Banking and custody counterparties may use this repository to review:

- reserve discipline  
- compliance posture  
- operational governance  
- legal classification clarity  

### 24.3 For Technical Reviewers

Technical reviewers may use this repository to understand:

- system design  
- authority boundaries  
- contract assumptions  
- risk treatment  
- security model  

---

## 25. Important Interpretive Boundaries

There are several points that all readers should understand clearly.

### 25.1 Repository Completeness Does Not Eliminate Risk

A well-documented system is not the same as a risk-free system.

### 25.2 Internal Audit Is Not Independent Assurance

The existence of an internal audit report strengthens institutional readiness, but should not be presented as equivalent to independent third-party audit assurance.

### 25.3 Reserve Framework Is Structured, but Off-Chain Dependencies Remain

Reserve discipline is documented thoroughly, but reserve operations still depend on real-world institutions and controls that cannot be reduced entirely to code.

### 25.4 Governance Integrity Remains Foundational

The quality of governance remains one of the most important variables affecting the long-term integrity of the system.

---

## 26. Special ASCII Diagrams

The following diagrams are included to support rapid institutional understanding of repository structure and system boundaries.

### 26.1 Repository Layering Diagram

```text
+--------------------------------------------------------------+
|                     dZWG Repository Stack                    |
+--------------------------------------------------------------+
| README.md                                                    |
|  - System overview                                           |
|  - Classification                                            |
|  - Navigation                                                |
|  - Reading paths                                             |
+--------------------------------------------------------------+
| Core System and Governance Layer                             |
|  - ARCHITECTURE.md                                           |
|  - GOVERNANCE.md                                             |
|  - DEPLOYMENT.md                                             |
+--------------------------------------------------------------+
| Risk / Control / Security Layer                              |
|  - RISK.md                                                   |
|  - CONTROLS.md                                               |
|  - SECURITY.md                                               |
+--------------------------------------------------------------+
| Compliance / Legal / Disclosure Layer                        |
|  - COMPLIANCE.md                                             |
|  - DISCLOSURES.md                                            |
|  - TERMS.md                                                  |
|  - DISCLAIMER.md                                             |
+--------------------------------------------------------------+
| Reserve / Assurance / Audit Layer                            |
|  - RESERVE_POLICY.md                                         |
|  - RESERVE_ATTESTATION.md                                    |
|  - AUDIT_SCOPE.md                                            |
|  - AUDIT_REPORT.md                                           |
+--------------------------------------------------------------+
```

### 26.2 Hybrid Operating Model Diagram

```text
                 +------------------------------+
                 |           On-Chain           |
                 |------------------------------|
                 | Token logic                  |
                 | Access controls              |
                 | Pause / emergency controls   |
                 | Upgrade logic                |
                 | Event logging                |
                 +--------------+---------------+
                                |
                                |
                                v
                 +------------------------------+
                 |           dZWG System        |
                 +--------------+---------------+
                                |
                                |
                                v
                 +------------------------------+
                 |          Off-Chain           |
                 |------------------------------|
                 | Reserve custody              |
                 | Treasury operations          |
                 | Compliance review            |
                 | Governance approvals         |
                 | Banking settlement           |
                 | Reserve attestation inputs   |
                 +------------------------------+
```

### 26.3 Institutional Reading Paths Diagram

```text
Exchanges        -> README -> DISCLOSURES -> COMPLIANCE -> AUDIT_REPORT -> RESERVE_ATTESTATION
Banks/Custodians -> README -> RESERVE_POLICY -> RESERVE_ATTESTATION -> COMPLIANCE -> TERMS
Auditors         -> README -> ARCHITECTURE -> GOVERNANCE -> CONTROLS -> SECURITY -> AUDIT_SCOPE
Regulators       -> README -> DISCLOSURES -> COMPLIANCE -> TERMS -> GOVERNANCE -> RESERVE_POLICY
```

These diagrams are functional navigation aids. They are not decorative. Their purpose is to reduce ambiguity and improve due diligence usability.

---

## 27. README Limitations

This README is an institutional entry point and orientation document. It is not intended to replace the specialized documents contained in the repository.

The README provides:

- classification context  
- navigation guidance  
- a structured overview of the system  

The README does not, by itself, provide the full detail necessary for:

- reserve reliance  
- deployment reliance  
- governance authority reliance  
- legal interpretation  
- compliance process reliance  
- audit interpretation  

For those purposes, readers should rely on the specialized documents identified throughout this README.

---

## 28. Versioning and Update Discipline

This repository may evolve over time as the system matures, governance changes, reserve processes are refined, documentation is improved, or deployment context changes.

Accordingly:

- readers should rely on the latest official repository version  
- institutional reviewers should confirm they are reading the current official version of the repository  
- deployment-specific reliance should be confirmed against [DEPLOYMENT.md](DEPLOYMENT.md)  
- audit-related reliance should be confirmed against [AUDIT_REPORT.md](AUDIT_REPORT.md) and [AUDIT_SCOPE.md](AUDIT_SCOPE.md)  
- reserve-related reliance should be confirmed against [RESERVE_POLICY.md](RESERVE_POLICY.md) and [RESERVE_ATTESTATION.md](RESERVE_ATTESTATION.md)  

Unofficial forks, copied materials, screenshots, altered reproductions, or partial excerpts should not be treated as authoritative.

---

## 29. Contribution and Security Reporting

Public contribution rights and security reporting procedures are governed by:

- [CONTRIBUTING.md](CONTRIBUTING.md)  
- [SECURITY.md](SECURITY.md)  

### 29.1 Contribution Model

This repository is not an unrestricted public code-contribution environment for live protocol modification.

### 29.2 Security Reporting

Security issues must not be disclosed publicly before remediation. The official security reporting channel is defined in the repository security policy in [SECURITY.md](SECURITY.md).

---

## 30. Intellectual and Operational Positioning

The repository documents a system intended to be treated as digital financial infrastructure, not as a casual token launch.

This distinction affects:

- the quality of documentation  
- the legal structure  
- the compliance architecture  
- the reserve framework  
- the operational expectations  

The repository has therefore been built to support:

- institutional reading  
- formal review  
- auditability  
- governance continuity  
- operational defensibility  

---

## 31. Current Readiness Position

Based on the documentation and internal audit posture reflected in this repository, dZWG presents as:

- structurally documented  
- reserve-policy supported  
- governance-defined  
- compliance-aware  
- control-mapped  
- security-scoped  
- internally audited  

This does not mean the system is beyond further enhancement. It means the system is already documented at a level that supports serious review rather than informal explanation.

---

## 32. Conclusion

Digital Zimbabwe Gold (dZWG) is presented in this repository as a fully documented, reserve-backed, compliance-aware, governance-controlled digital settlement system.

The repository does not rely on marketing language to explain the project. It relies on architecture, controls, governance, reserve policy, legal classification, security structure, disclosures, and audit documentation.

That is intentional.

The aim of this repository is to make dZWG understandable and reviewable in institutional terms.

The system, as documented here, is designed to support:

- controlled production deployment  
- exchange and institutional due diligence  
- governance-managed operation  
- reserve-linked digital settlement within a documented legal and compliance framework  

---

## 33. Contact

For formal inquiries regarding dZWG, repository documentation, or institutional review:

**Abba Payments (Namibia) (Pty) Ltd**, a wholly-owned subsidiary of [Abba Industries](https://abbaii.com/)

For security-related reporting, use the official security channel identified in [SECURITY.md](SECURITY.md).

---

## 34. License and Use of Repository Materials

Use of repository materials is subject to the applicable repository license and the legal and usage boundaries described throughout the documentation stack.

Readers and counterparties must rely on the latest official version of repository documents and should not rely on unofficial forks, copied materials, or altered reproductions not identified by the issuer as official.

---

End of Document
