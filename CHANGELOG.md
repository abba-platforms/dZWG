# Changelog

All notable changes to the Digital Zimbabwe Gold (dZWG) project will be documented in this file. The format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [v1.2.0] - 2026-03-31
### Institutional Rebuild, Mainnet Deployment, and Full Documentation Stack

This release represents a complete transition from the Zimbabwe Digital Dollar (ZDD) concept to the **Digital Zimbabwe Gold (dZWG)** system, aligned with Zimbabwe Gold (ZiG; ISO code: ZWG), and includes a full institutional-grade repository rebuild.

---

### System Transition

**Protocol Evolution**
- Transitioned system from **Zimbabwe Digital Dollar (ZDD)** to **Digital Zimbabwe Gold (dZWG)**.
- Updated denomination framework from USD-referenced to **ZiG (ZWG)-referenced monetary unit**.
- Repositioned system as a **digital settlement instrument aligned with Zimbabwe Gold (ZiG)**.
- Updated all documentation to reflect ZiG monetary framework and terminology consistency.

---

### Mainnet Deployment

**Deployment**
- Successfully deployed dZWG on **BNB Smart Chain (BSC) Mainnet**.
- Implemented **upgradeable proxy architecture** for production-grade deployment.

**Contract Addresses**
- Proxy Contract: `0xb764383a8A0502c1CF6d58c9de3bA7e5AACdeeA3`
- Implementation Contract: `0x9D596814CcA04A083a470014eacF7eDC2aA531e2`

**Architecture**
- Proxy contract designated as the **canonical integration address** for:
  - wallets
  - exchanges
  - payment systems
- Implementation contract contains logic referenced through proxy.
- Upgradeability governed through controlled administrative processes.

---

### README.md — Full Institutional Rebuild

- Rebuilt README.md to **institutional-grade standard** without condensing or truncating content.
- Added **Deployment Status synopsis** with full token metadata and contract addresses.
- Introduced **complete repository navigation structure**.
- Implemented **full Markdown backlinking** to all referenced documents.
- Added **"How to Read This Repository"** section with role-specific reading paths.
- Defined **system boundaries** (on-chain vs off-chain responsibilities).
- Introduced **official sources of truth** across all documentation layers.
- Added **current system status** section for clarity of readiness.
- Added **explicit non-affiliation and regulatory positioning**:
  - not issued by Reserve Bank of Zimbabwe
  - not legal tender
  - not a CBDC
- Added **ASCII diagrams**:
  - repository architecture layers
  - hybrid system model
  - institutional reading flows
- Added **README scope and reliance limitations**.
- Introduced **versioning and update discipline guidance**.

---

### New Institutional Documents Added

**Governance, Risk, and Controls**
- Added **GOVERNANCE.md**:
  - role-based authority model
  - upgrade control and decision flow
  - administrative segregation of duties
- Added **RISK.md**:
  - full risk taxonomy (technical, financial, operational, regulatory)
  - mitigation frameworks
- Added **CONTROLS.md**:
  - internal control framework
  - access control, upgrade control, reserve control structures

**Compliance and Legal**
- Added **COMPLIANCE.md**:
  - regulatory positioning framework
  - AML/KYC integration considerations
  - jurisdictional boundaries
- Added **DISCLOSURES.md**:
  - full transparency statements
  - non-affiliation disclosures
  - limitation disclosures
- Added **TERMS.md**:
  - structured system usage terms
  - legal boundaries and responsibilities
- Added **DISCLAIMER.md**:
  - formal disclaimers covering:
    - non-legal tender status
    - non-CBDC classification
    - non-affiliation with Reserve Bank of Zimbabwe

---

### Reserve and Assurance Framework

- Added **RESERVE_POLICY.md**:
  - reserve structure definition
  - custody and allocation principles
  - operational reserve management framework
- Added **RESERVE_ATTESTATION.md**:
  - attestation methodology
  - verification process structure
  - reporting expectations

---

### Security and Audit

- Rebuilt **SECURITY.md**:
  - expanded responsible disclosure framework
  - detailed reporting requirements
  - system integrity and governance controls
  - structured incident handling process
- Added **AUDIT_SCOPE.md**:
  - defined scope of internal audit coverage
  - components included in audit evaluation
- Added **AUDIT_REPORT.md**:
  - full OpenZeppelin-style production-grade audit report
  - overall score: approximately **9.2/10**
  - detailed findings, validation, and control analysis

---

### Deployment and Architecture Documentation

- Added **DEPLOYMENT.md**:
  - full deployment structure
  - contract architecture and relationships
  - operational interpretation of addresses
- Updated **ARCHITECTURE.md**:
  - expanded system design
  - on-chain/off-chain separation
  - upgradeable contract model

---

### Contribution and Security Updates

- Updated **CONTRIBUTING.md**:
  - clarified restricted contribution model
  - defined acceptable community interactions
  - reinforced controlled development approach
- Updated **SECURITY.md** contact:
  - standardized reporting email: **security@abbaii.com**

---

### Repository Standardization

- Ensured all documents:
  - remain in **pure raw Markdown format**
  - contain **no truncation, compression, or condensation**
  - follow **institutional documentation structure**
- Standardized:
  - terminology across all files
  - formatting consistency
  - cross-referencing between documents

---

## [v1.1.1] - 2025-09-24
### README Refinement Update

**README.md**
- Fixed raw markdown formatting issue before the "Compile Contracts" section to ensure consistent preview rendering.
- Ensured README stays in pure raw markdown format without switching to preview mid-document.
- Deep-checked and preserved all existing content without truncation.
- Maintained original structure and wording while adding formatting improvements.

---

## [v1.1.0] - 2025-09-24
### Deployment & Documentation Update

**Deployment**
- Successfully deployed the Zimbabwe Digital Dollar (ZDD) smart contract on the Binance Smart Chain (BSC) Testnet.
- Added deployed contract addresses:
  - Proxy Contract: `0x93b2eFFC896fC3f3789c493972fe585A2C02B108`
  - Implementation Contract: `0x0197c9e1ed52dd74d9d3978A9dbe98408a59266f`
- Verified implementation contract on BSC Testnet Explorer: https://testnet.bscscan.com/address/0x0197c9e1ed52dd74d9d3978A9dbe98408a59266f#code
- Linked proxy to implementation for upgradeable contract architecture.

**Documentation**
- Updated **README.md** to include deployment details, contract addresses, and BSC Testnet explorer links.
- Added license badges for improved professionalism and clarity.
- Preserved all existing README content to maintain documentation continuity.

**Maintenance**
- Added deployment verification steps to project documentation for transparency.
- Ensured changelog follows Keep a Changelog format.

---

## [v1.0.0] - 2025-09-18
### Initial Release

**Repository Setup and Documentation**
- Created full project structure for ZDD repository
- Added **README.md**:
  - Project overview and vision
  - Executive Summary with key features
  - Stablecoin technical architecture overview
  - Disclaimer clarifying ZDD is independent and not affiliated with the Reserve Bank of Zimbabwe
  - Instructions for setup, compilation, and running tests
  - Repository contents overview

**Legal and Licensing**
- Added **LICENSE.md** using MIT License
- Added **CONTRIBUTION.md**:
  - Clarifies no public contributions to smart contracts
  - Provides guidance for non-technical feedback
  - Includes **security@zddollar.io** as official contact for reporting errors or concerns
- Added **SECURITY.md**:
  - Responsible vulnerability reporting procedures
  - Scope of coverage (smart contracts, libraries, governance logic)
  - Response and disclosure guidelines
  - Contact email: **security@zddollar.io**

**Research and Analysis**
- Added **ZIMBABWE_ANALYSIS.md**:
  - Comprehensive country analysis (population, economy, currency usage, remittance flows)
  - Opportunity for ZDD adoption in domestic and cross-border trade
  - Historical monetary instability and market gap analysis

**Smart Contract**
- Added **ZDD_SMART_CONTRACT_SHORT.md**:
  - Draft of ZDD smart contract
  - ERC-3643 compliant, USD-pegged stablecoin architecture
  - Tiered KYC/AML logic and proof-of-reserves
  - Placeholder for enterprise-grade governance features

**Formatting and Standards**
- All files generated in pure raw Markdown for easy GitHub copy-paste
- Tables, code blocks, and examples fully preserved
- Ensured no truncation or condensation of content
- Indented code blocks for commands and scripts to maintain Markdown integrity

**Future placeholders**
- CHANGELOG.md initialized for tracking future versions
- Smart contract, governance, and feature updates to be documented here

---
