# dZWG Compliance Framework

## 1. Overview

The Digital Zimbabwe Gold (dZWG) system operates within a formal compliance framework designed to support lawful usage, controlled participation, and enforceable restrictions across a hybrid blockchain and off-chain financial environment.

Compliance in dZWG is not treated as an optional operational feature. It is a foundational system layer. The framework is designed to ensure that the system can operate as a controlled, reserve-backed digital settlement instrument while maintaining alignment with anti-money laundering requirements, counter-terrorist financing expectations, sanctions controls, and broader financial integrity obligations.

The dZWG compliance model is intentionally hybrid in structure. Certain compliance functions, such as identity verification, sanctions screening, risk assessment, and records management, necessarily occur off-chain because they depend on legal identity, documentary evidence, and external information sources. Other compliance functions, such as transaction restriction, address-level controls, and operational enforcement, are executed on-chain through smart contract permissions and governance-controlled mechanisms.

This document defines the compliance structure of dZWG in full institutional form. It explains the objectives, legal posture, participant categorization, enforcement model, jurisdictional considerations, recordkeeping, regulatory change management, and limitations of the compliance framework.

dZWG is issued and operated by:

Abba Payments (Namibia) (Pty) Ltd

dZWG is not affiliated with, endorsed by, or issued by the Reserve Bank of Zimbabwe.

---

## 2. Compliance Objectives

The dZWG compliance framework is designed to achieve the following objectives.

First, it is intended to ensure that participants using the system can be identified, categorized, monitored, and, where necessary, restricted in accordance with applicable legal and regulatory expectations.

Second, it is intended to reduce the risk that dZWG is used for illicit purposes, including money laundering, terrorist financing, sanctions evasion, fraud, or other prohibited financial activity.

Third, it is intended to provide an operational framework within which reserve-backed issuance, redemptions, account controls, and transaction flows can be supported by auditable compliance decisions.

Fourth, it is intended to support institutional engagement. This includes interaction with regulators, financial institutions, exchanges, liquidity providers, and other counterparties that require evidence of structured compliance governance.

Fifth, it is intended to preserve the integrity of the system by ensuring that compliance decisions are not merely policy statements, but can be translated into enforceable operational outcomes.

---

## 3. Compliance Model Structure

### 3.1 Hybrid Compliance Model

The dZWG compliance system is divided into two interdependent layers.

The first layer is the off-chain compliance layer. This includes participant onboarding, KYC verification, sanctions screening, risk review, records retention, case handling, and internal compliance decision-making. This layer exists off-chain because it depends on legal identity, documentary records, and external compliance information sources that do not exist natively on-chain.

The second layer is the on-chain enforcement layer. This includes account restrictions, transfer blocking, freeze status, sanctions flags, and any other enforceable state changes that determine whether a wallet or transaction is permitted to proceed within the dZWG system.

This separation is deliberate. The off-chain layer establishes the legal and evidentiary basis for a compliance decision. The on-chain layer ensures that the decision can be enforced through the settlement infrastructure itself.

### 3.2 Compliance Decision and Enforcement Relationship

Compliance decisions are not made by the smart contract. They are made through off-chain compliance review and governance procedures. Once a determination has been made, authorized on-chain roles implement that decision through system controls.

This means the system distinguishes clearly between:

- compliance analysis and determination  
- compliance execution and enforcement  

That distinction is necessary for legal defensibility, operational accountability, and auditability.

---

## 4. Participant Classification

The dZWG system classifies participants according to compliance status and permitted scope of activity.

### 4.1 Fully Verified Participants

Fully verified participants are individuals or entities that have completed the required identity verification, risk review, and onboarding procedures to the satisfaction of the operator.

These participants may access the system within the limits of applicable policy, operational rules, and regulatory restrictions.

### 4.2 Limited Access Participants

Limited access participants are users whose verification status is sufficient only for restricted system usage. This category may apply to users who have satisfied simplified or reduced due diligence requirements but have not completed full KYC onboarding.

These participants are subject to lower transaction thresholds, reduced privileges, and closer monitoring.

### 4.3 Restricted Participants

Restricted participants are those whose activity, identity status, or compliance posture requires operational limitation. This may include participants under review, participants with incomplete documentation, or participants associated with elevated risk patterns.

Restricted participants may be subject to transaction limits, account freezes, or other controls.

### 4.4 Prohibited Participants

Prohibited participants are those who may not use the system at all. This category includes sanctioned persons, blacklisted addresses, participants associated with prohibited conduct, and any user whose participation would expose the system to unacceptable legal or regulatory risk.

The prohibited category is enforced through both off-chain exclusion and on-chain restriction mechanisms.

---

## 5. KYC and Identity Verification

### 5.1 Objective

The purpose of KYC within dZWG is to ensure that participants can be sufficiently identified and risk-assessed in accordance with the intended use of the system and applicable regulatory expectations.

The framework is designed to support a risk-based approach rather than a one-size-fits-all onboarding model.

### 5.2 KYC Levels

#### Level 1: Mini-KYC

Mini-KYC is intended for lower-risk or lower-threshold participation. It supports reduced onboarding friction while preserving basic compliance screening.

Participants at this level may be permitted to transact only within defined thresholds. The exact thresholds are subject to policy and governance, but are intended to limit exposure associated with reduced diligence.

#### Level 2: Full KYC

Full KYC applies to participants who require broader system access, higher transaction capacity, or institutional usage privileges.

This level requires complete identity verification, and where relevant may include enhanced due diligence, beneficial ownership review, proof of address, or other supporting documentation appropriate to the participant type and risk level.

### 5.3 KYC Threshold Model

The dZWG framework is designed to support threshold-based compliance treatment. Mini-KYC users may be permitted to operate below specified transaction or cumulative limits, while activity above those limits triggers the need for fuller verification.

Thresholds are not static by assumption. They may be adjusted through governance, subject to regulatory, operational, or risk-based considerations.

The purpose of thresholding is to align the compliance burden with transaction risk while preserving system accessibility where appropriate.

---

## 6. AML and Transaction Monitoring

### 6.1 Objective

The AML monitoring layer exists to detect and deter suspicious or prohibited financial activity within the dZWG system.

### 6.2 Monitoring Scope

Monitoring may include review of:

- transaction size  
- transaction frequency  
- unusual transaction patterns  
- linked wallet behavior  
- rapid movement of funds  
- structuring behavior intended to avoid thresholds  
- interactions suggestive of sanctions or illicit finance risk  

### 6.3 Monitoring Methods

The system is designed to support both automated and manual monitoring.

Automated monitoring may be used to detect defined patterns, threshold breaches, or anomalies in transaction behavior.

Manual review may be conducted where automated alerts, external information, or case-specific analysis indicates the need for deeper assessment.

### 6.4 Monitoring Outcomes

Monitoring may result in:

- no action  
- enhanced review  
- temporary restriction  
- account freeze  
- escalation to governance  
- reporting to relevant authorities where legally required  

The compliance framework does not assume that monitoring alone eliminates illicit use. It is a risk-reduction layer, not a guarantee of perfect detection.

---

## 7. Sanctions and Screening

### 7.1 Objective

The objective of sanctions screening is to prevent participation in the dZWG system by individuals, entities, or counterparties that are prohibited by applicable law, sanctions regimes, or internal risk policy.

### 7.2 Screening Inputs

Screening may rely on:

- sanctions lists  
- internal prohibited-participant lists  
- regulatory watchlists  
- risk intelligence sources  
- adverse compliance findings  

### 7.3 Screening Timing

Screening may occur:

- during onboarding  
- during periodic review  
- in response to transaction activity  
- when external information changes  
- prior to redemption or settlement processing  

### 7.4 Enforcement

Where sanctions or equivalent prohibitions are identified, the system may enforce restrictions including:

- onboarding refusal  
- transaction blocking  
- account freezing  
- permanent exclusion  

Sanctions enforcement is a mandatory compliance function, not a discretionary convenience measure.

---

## 8. On-Chain Compliance Enforcement

### 8.1 Enforcement Mechanisms

dZWG is designed to support on-chain enforcement mechanisms including:

- freeze status  
- blacklist status  
- sanctions status  
- transfer restrictions  
- operational blocks on sending or receiving  

### 8.2 Execution Authority

On-chain compliance enforcement is executed through the authorized compliance role defined in the governance architecture.

This role does not determine compliance outcomes independently. It implements compliance decisions that have been reached through the off-chain compliance process.

### 8.3 Enforcement Logic

The smart contract is designed to check compliance state before allowing relevant transaction paths to proceed. A restricted account may be prevented from sending tokens, receiving tokens, participating in mint-related flows, or completing other system interactions depending on the specific control applied.

### 8.4 Institutional Significance

This enforcement architecture is essential to institutional readiness because it ensures compliance is not merely documented but enforceable at the transaction layer.

---

## 9. Compliance Decision and Execution Separation

The dZWG framework treats compliance determination and compliance execution as separate but coordinated functions.

The compliance function reviews documentation, activity, jurisdictional exposure, sanctions information, and operational context. Based on that review, it determines whether a participant may transact, whether restrictions should apply, or whether escalation is required.

Once that determination exists, the on-chain compliance role executes the corresponding control.

This separation exists for four reasons.

First, it preserves legal and evidentiary discipline.

Second, it avoids arbitrary or undocumented on-chain enforcement.

Third, it allows compliance decisions to be reviewed, documented, and auditable.

Fourth, it reduces the risk that technical role holders act without policy authority.

---

## 10. Reporting and Recordkeeping

### 10.1 Compliance Records

The system is intended to maintain records relating to:

- KYC documentation  
- onboarding determinations  
- sanctions screening outcomes  
- transaction monitoring alerts  
- compliance enforcement decisions  
- case escalation and resolution records  

### 10.2 Retention

Records are to be retained in accordance with applicable legal, regulatory, and operational requirements. Retention periods may vary by jurisdiction, record type, and regulatory expectation.

### 10.3 Auditability

dZWG supports a dual audit trail:

- immutable on-chain records of enforcement and transaction activity  
- off-chain records supporting the legal and procedural basis for those actions  

### 10.4 Importance

Without recordkeeping, compliance cannot be demonstrated. Record retention is therefore not administrative overhead; it is a foundational control.

---

## 11. Regulatory Engagement

### 11.1 Objective

The dZWG compliance framework is designed to support constructive engagement with regulators, financial institutions, auditors, and institutional counterparties.

### 11.2 Capabilities

The framework is intended to support the ability to provide:

- transaction records  
- compliance process descriptions  
- governance records  
- controls documentation  
- evidence of enforcement capabilities  

### 11.3 Institutional Position

The existence of a compliance framework does not itself mean regulatory approval exists. It means the system is structured in a way that can support lawful supervision, oversight, and review.

---

## 12. Privacy and Data Protection

### 12.1 Objective

The compliance framework must support identity verification and records retention while minimizing unnecessary exposure of sensitive personal information.

### 12.2 Data Placement

Sensitive identity data is not stored on-chain. Personal data and supporting KYC records are maintained off-chain in controlled systems.

On-chain records are limited to addresses, transactions, and state-related events required for system operation and auditability.

### 12.3 Access Control

Access to off-chain compliance data is expected to be restricted to authorized personnel and controlled systems.

### 12.4 Limitation

Blockchain transactions are inherently visible on public networks. The system therefore cannot guarantee transactional privacy in the same way as a private ledger or closed banking system.

---

## 13. Cross-Border Compliance Considerations

### 13.1 Nature of the Risk

dZWG may interact with users, counterparties, exchanges, or service providers across multiple jurisdictions. This creates legal and compliance complexity.

### 13.2 Core Challenges

Cross-border usage may involve:

- conflicting regulatory standards  
- differing sanctions requirements  
- different data protection obligations  
- licensing or registration triggers in certain jurisdictions  

### 13.3 Framework Response

The system is designed to operate under a jurisdiction-aware compliance model. Core standards are centrally defined, but the system may apply higher or more restrictive standards where jurisdictional conflict exists.

Where legal uncertainty is material, access may be restricted until the relevant risk is resolved.

---

## 14. Compliance Governance

### 14.1 Ownership

The compliance framework is owned by the compliance function of the operating entity.

### 14.2 Operators

Operational execution of on-chain enforcement is handled through the authorized compliance role within the smart contract framework.

### 14.3 Review and Oversight

Governance retains oversight over compliance architecture, major enforcement categories, and policy changes. However, day-to-day compliance determinations should be made by the compliance function, not by technical operators acting independently.

### 14.4 Importance

This ownership model ensures compliance is governed as a formal control function, not as an ad hoc administrative task.

---

## 15. Exception Handling

### 15.1 Definition

An exception exists where standard compliance treatment cannot be applied cleanly, or where special handling is required due to legal, operational, or evidentiary complexity.

### 15.2 Requirements

Exceptions must be:

- documented  
- reviewed  
- approved through appropriate authority  
- resolved or closed with a record of disposition  

### 15.3 Importance

Institutional compliance frameworks must be able to handle edge cases without collapsing into inconsistency or arbitrary judgment.

---

## 16. Compliance Monitoring and Review

### 16.1 Continuous Monitoring

The framework supports ongoing review of:

- transaction behavior  
- threshold breaches  
- unusual activity patterns  
- enforcement events  

### 16.2 Periodic Review

Compliance policies, thresholds, and operational processes should be reviewed periodically to ensure continued relevance, legal sufficiency, and risk alignment.

### 16.3 Governance Link

Material policy changes require governance oversight and approval.

---

## 17. Compliance Risk

### 17.1 Residual Risk

Even with strong controls, compliance risk remains. This includes:

- evolving legal standards  
- false negatives in suspicious activity detection  
- cross-border regulatory conflict  
- imperfect information about counterparties  

### 17.2 Institutional Position

The dZWG compliance framework is designed to mitigate compliance risk, not eliminate it entirely. This distinction is essential for legal and operational honesty.

---

## 18. Non-Guarantees

The compliance framework does not guarantee:

- detection of all illicit activity  
- immunity from future regulatory changes  
- elimination of all abuse vectors  
- universal legal acceptance of the system  

It is a structured risk-mitigation and enforcement framework, not a guarantee of perfect compliance outcomes.

---

## 19. Legal and Regulatory Positioning

dZWG is a privately issued digital payment and settlement instrument designed to operate as a blockchain-native representation of Zimbabwe Gold.

dZWG is not legal tender. It is not issued by the Reserve Bank of Zimbabwe. It does not represent a claim on the central bank. It is not a central bank digital currency. It is not a deposit-taking instrument.

The system is issued and administered by:

Abba Payments (Namibia) (Pty) Ltd

The framework is structured to be regulator-compatible, but it does not assume that a compliance framework alone constitutes licensing, approval, or statutory recognition in any jurisdiction.

The legal and regulatory posture of dZWG is therefore one of compliance-oriented private issuance, subject to applicable law and oversight where relevant.

---

## 20. Jurisdictional Compliance Strategy

dZWG operates in a multi-jurisdictional environment.

### 20.1 Primary Jurisdiction

The issuer and operator is based in Namibia. This forms the primary operational and corporate control jurisdiction.

### 20.2 Functional Exposure

The system may involve Zimbabwe-linked users, regional participants, and cross-border counterparties. This creates exposure to multiple regulatory environments.

### 20.3 Strategy

The compliance strategy is jurisdiction-aware rather than jurisdiction-blind. Core compliance standards are centrally maintained, but the system may adopt stricter rules where required by law, counterparty obligation, or risk assessment.

Where legal conflict arises, the framework is intended to apply the higher or more restrictive standard pending resolution.

---

## 21. Licensing and Regulatory Status

dZWG does not assume or assert any banking license, deposit-taking license, central bank authorization, or sovereign endorsement unless such status is formally obtained and documented.

The framework is designed to be structurally compliance-ready. This means that the system can support controlled operation, enforceable restrictions, auditability, and engagement with regulated institutions. It does not mean that any specific regulatory permission should be presumed.

If licensing, registration, or formal approvals are required in a given jurisdiction, the system may need to adapt its structure, operations, onboarding, or access conditions accordingly.

---

## 22. Reserve Compliance and Safeguarding

### 22.1 Reserve Structure

dZWG is designed to operate on a reserve-backed basis, with reserves denominated in Zimbabwe Gold or equivalent cash instruments held in regulated financial environments.

### 22.2 Custody and Segregation

Reserves are intended to be segregated from operational funds and maintained for the benefit of dZWG token holders.

### 22.3 Governance Control

Movement of reserve assets is expected to be subject to governance controls, including multi-signature authorization and financial oversight procedures.

### 22.4 Compliance Objective

The objective of reserve compliance is to support:

- solvency discipline  
- redemption integrity  
- confidence in supply backing  
- operational transparency  

### 22.5 Institutional Significance

Reserve safeguarding is not merely a treasury function. It is a compliance-critical function because reserve misuse, commingling, or opacity would directly undermine the legal and regulatory posture of the system.

---

## 23. Redemption Compliance

### 23.1 Objective

The purpose of redemption compliance is to ensure that redemptions are processed lawfully, traceably, and in a manner consistent with reserve availability and participant verification.

### 23.2 Core Conditions

Redemption may require:

- participant identification  
- completion of required KYC  
- sanctions and compliance validation  
- satisfaction of operational conditions  
- sufficient reserve support  

### 23.3 Restrictions

Redemption may be delayed, restricted, or denied where:

- compliance requirements are incomplete  
- sanctions exposure exists  
- legal restrictions apply  
- operational risk conditions are present  

### 23.4 Institutional Significance

A reserve-backed system without a compliant redemption model is incomplete. Redemption compliance is therefore a central element of the framework, not a secondary process.

---

## 24. Transaction Restrictions and Limits

### 24.1 Purpose

Transaction limits are used to align user access with risk level and compliance status.

### 24.2 Types of Restrictions

Restrictions may include:

- per transaction limits  
- daily cumulative limits  
- threshold-based step-up to full KYC  
- restrictions by user category or jurisdiction  

### 24.3 Governance and Flexibility

Thresholds are expected to be configurable through governance, subject to compliance and risk review.

### 24.4 Importance

Transaction restriction architecture is essential because it allows the system to preserve access where possible while controlling exposure where risk is higher.

---

## 25. Third-Party and Counterparty Compliance

### 25.1 Scope

The dZWG system may interact with external parties including:

- exchanges  
- payment processors  
- liquidity providers  
- banking partners  
- other infrastructure providers  

### 25.2 Compliance Expectations

Where dZWG integrates with third parties, those parties are expected to maintain compliance standards that are compatible with the operator’s obligations and risk posture.

### 25.3 Risk Management

Non-compliant or higher-risk counterparties may be restricted, limited, or disconnected from system participation where necessary.

### 25.4 Significance

Institutional compliance does not end at the contract boundary. It extends to the counterparties that enable or distribute system access.

---

## 26. Compliance Controls Mapping

The compliance framework does not operate in isolation. It maps directly into the broader institutional control environment.

Compliance controls are linked to:

- [CONTROLS.md](./CONTROLS.md)    
- [GOVERNANCE.md](./GOVERNANCE.md) 
- [RISK.md](./RISK.md)      
- [ARCHITECTURE.md](./ARCHITECTURE.md)     

Each major compliance function should correspond to:

- a policy basis  
- an accountable owner  
- an on-chain or off-chain control  
- a monitoring or review mechanism  

This mapping is essential for auditability and institutional review.

---

## 27. Audit and Assurance

### 27.1 Internal Review

Compliance processes are expected to be reviewed internally on a periodic basis. This may include policy review, threshold testing, control review, and case management quality checks.

### 27.2 External Assurance

Where appropriate, external review, audit, or independent assurance procedures may be used to strengthen confidence in the framework.

### 27.3 Evidence Base

Evidence supporting compliance assurance may include:

- onboarding records  
- compliance logs  
- enforcement records  
- governance decisions  
- transaction histories  
- reserve-related documentation where relevant  

### 27.4 Institutional Importance

A compliance framework is materially stronger when it can be evidenced, reviewed, and challenged. Auditability is therefore not supplementary; it is integral.

---

## 28. Enforcement Actions

### 28.1 Available Actions

The system is designed to support enforcement measures including:

- account restriction  
- account freezing  
- transaction blocking  
- exclusion from onboarding or redemption  
- forced review or escalation  

### 28.2 Authority

On-chain enforcement is executed through the compliance role under governance-defined authority and procedural controls.

### 28.3 Principle

Enforcement should be proportionate, documented, and aligned with the reason for action.

---

## 29. Incident and Breach Handling

### 29.1 Definition

A compliance incident may include:

- suspected AML breach  
- sanctions exposure  
- suspicious transaction activity  
- unauthorized access to compliance records  
- breakdown in enforcement or onboarding process  

### 29.2 Response Process

Compliance incidents should trigger:

- investigation  
- containment where necessary  
- enforcement action if justified  
- escalation to governance where material  
- documentation of resolution  

### 29.3 Importance

Institutional-grade compliance requires breach handling discipline. A framework without incident handling is incomplete.

---

## 30. Policy Management

### 30.1 Ownership

Compliance policy is owned by the compliance function of the operator.

### 30.2 Updates

Policies may be updated in response to:

- regulatory change  
- operational experience  
- risk review  
- counterparty requirements  

### 30.3 Approval

Material policy changes require governance review and approval.

### 30.4 Recordkeeping

Superseded and current versions of policy should be retained in a controlled manner.

---

## 31. Training and Awareness

### 31.1 Objective

Personnel involved in compliance, operations, governance, and transaction handling must understand their responsibilities under the compliance framework.

### 31.2 Scope

Training and awareness should extend to:

- compliance staff  
- operations staff  
- governance participants  
- relevant technical personnel where enforcement logic is involved  

### 31.3 Significance

Controls are weakened where policy is not understood. Training is therefore a compliance control in its own right.

---

## 32. Record Integrity

### 32.1 Requirement

Compliance records must be accurate, complete, protected from tampering, and retrievable for review.

### 32.2 On-Chain Integrity

Blockchain records provide immutable evidence of transaction execution and enforcement state.

### 32.3 Off-Chain Integrity

Off-chain systems must support:

- controlled access  
- version integrity  
- retention discipline  
- reviewability  

### 32.4 Importance

Record integrity is fundamental to legal defensibility and regulatory response.

---

## 33. Regulatory Change Management

### 33.1 Nature of the Risk

Regulatory environments are not static. Legal and supervisory expectations for digital settlement systems may evolve materially over time.

### 33.2 Framework Response

The system is expected to monitor regulatory developments and adapt:

- policies  
- thresholds  
- controls  
- access conditions  
- disclosures  

where necessary.

### 33.3 Governance Link

Material regulatory response actions should be escalated through governance and documented accordingly.

---

## 34. Compliance Limitations

The compliance framework is designed to reduce and manage risk. It cannot eliminate all uncertainty, abuse, or legal change.

Limitations include:

- evolving regulations  
- incomplete external information  
- sophisticated evasion techniques  
- cross-border complexity  
- dependency on human and institutional judgment  

The framework should therefore be understood as a structured risk-mitigation and enforcement system, not a guarantee of perfect outcomes.

---

## 35. Conclusion

The dZWG compliance framework provides a structured institutional model that combines off-chain legal and regulatory processes with on-chain transaction enforcement.

It is designed to ensure that:

- participants are categorized and reviewed  
- restricted activity can be blocked  
- records are auditable  
- compliance decisions are enforceable  
- the system remains adaptable to evolving regulatory expectations  

The purpose of this framework is to make dZWG operationally defensible, regulator-compatible, and institutionally credible as a reserve-backed digital settlement system.

---

End of Document
