# Digital Zimbabwe Gold (dZWG) Whitepaper

## Version 1.2 (Institutional Edition)

**Date:** September 17, 2025      
**Creator:** [Simon Kapenda](https://linkedin.com/in/simonkapenda)         
**Issuer and Operator:** Abba Payments (Namibia) (Pty) Ltd., a wholly-owned subsidiary of [Abba Industries](https://abbaii.com)         
**Repository:** https://github.com/abba-platforms/dzwg

---

## Executive Summary

Digital Zimbabwe Gold (dZWG) is a privately issued, blockchain-native stablecoin designed to represent Zimbabwe Gold (ZWG) on-chain at a fixed parity of one dZWG to one ZWG. The system is structured as a reserve-backed digital payment and settlement instrument intended for retail, enterprise, institutional, and interoperable regional financial use.

dZWG is not denominated in United States Dollars (USD) and does not function as a USD substitute. It is designed to directly represent Zimbabwe Gold itself. Its monetary model is therefore locally aligned: one dZWG token corresponds to one unit of ZWG, and the system is intended to maintain full reserve backing in ZWG at all times. In operational terms, circulating supply is intended to remain fully matched by reserves denominated in ZWG and held under controlled custody arrangements.

The system combines on-chain transparency with off-chain reserve administration. On-chain, the protocol records balances, supply changes, administrative actions, compliance controls, and upgrade events. Off-chain, the system relies on reserve custody, attestation, governance, compliance administration, and redemption operations. dZWG is therefore designed as a hybrid financial infrastructure system: technologically native to blockchain, but governed with the controls expected of an institutional financial product.

dZWG forms part of a broader multi-currency digital financial infrastructure strategy that includes Namibia Digital Dollar (NADD) and Angola Digital Kwanza (AOAk). Within that broader framework, dZWG serves as the Zimbabwean monetary layer, intended to support domestic payments, enterprise finance, government disbursements, treasury operations, and structured cross-border settlement across compliant domestic-currency digital assets.

---

## Table of Contents

1. Executive Summary  
2. Issuer, Creator, and Operational Structure  
3. Legal Status and Disclaimers  
4. Introduction  
5. Background: Zimbabwe's Monetary Landscape  
6. Problem Statement  
7. Why dZWG  
8. Design Principles  
9. System Overview  
10. Technical Architecture  
11. Reserve Custody and Asset Policy  
12. Reserve Attestation and Reporting  
13. Reserve Shortfall Policy  
14. Issuance Framework  
15. Redemption Framework  
16. Compliance, KYC, AML, and Sanctions Controls  
17. Governance and Administrative Control Model  
18. Upgrade and Change Management Policy  
19. Fees and Treasury Policy  
20. Token Holder Rights and Limitations  
21. Supported Users and Access  
22. Jurisdictional Scope  
23. Infrastructure Dependency and Network Risk  
24. Market Structure and Secondary Trading Disclaimer  
25. Security Architecture  
26. Economic Model and Tokenomics  
27. Wind-Down and Orderly Termination Framework  
28. Risk Factors and Mitigations  
29. Parameter Governance Summary  
30. Deployment and Network Information  
31. Roadmap and Implementation Path  
32. Technical Appendix  
33. ASCII Diagrams  
34. References  

---

## 1. Issuer, Creator, and Operational Structure

dZWG was created by [Simon Kapenda](https://linkedin.com/in/simonkapenda), creator of [Namibia Digital Dollar (NADD)](https://nadd.io), [Angola Digital Kwanza (AOAk)](https://github.com/abba-platforms/AOAk), [Naira Index (NXY)](https://github.com/abba-platforms/NXY), [Namibia 30 Index (NAX30)](https://nax30.io), [Kenya 30 Index (KEN30)](https://ken30.com), [Malawi Digital Kwacha (ACHA)](https://github.com/abba-platforms/ACHA), [Zambia Digital Kwacha (dZMW)](https://github.com/abba-platforms/dZMW), and [SACE Index (SACE)](https://sacex.io).

dZWG is issued, operated, and maintained by Abba Payments (Namibia) (Pty) Ltd, a company incorporated and registered in Namibia and is wholly-owned subsidiary of [Abba Industries](https://abbaii.com). The issuer and operator is responsible for system administration, issuance controls, redemption administration, reserve custody coordination, governance execution, and compliance operations.

The creator serves as the system architect and originator of the framework. Legal, operational, and administrative responsibility for issuance and maintenance resides with the issuing entity unless otherwise formally delegated by policy, contract, or law.

This separation is intentional. Institutional financial systems require clarity on who designed the system, who operates it, and who is accountable for reserve-backed issuance and redemption. In the case of dZWG, authorship and operational responsibility are related but not identical concepts.

---

## 2. Legal Status and Disclaimers

dZWG is a privately issued digital asset. It is not issued by the Reserve Bank of Zimbabwe and does not constitute legal tender unless formally recognized by applicable law, regulation, or supervisory framework.

Ownership of dZWG does not constitute a bank deposit and does not provide deposit insurance, sovereign guarantee, or statutory protection merely by virtue of token possession. Holding dZWG represents a digital claim within the system and does not, by itself, create direct legal ownership of underlying reserve accounts.

The rights of token holders arise from the issuer's operating framework, reserve model, redemption procedures, governance controls, and applicable legal agreements. The blockchain records token balances and system events, but legal rights remain defined by the issuer's framework and applicable law.

dZWG should be understood as a reserve-backed digital settlement instrument rather than an equity instrument, a debt security, or a profit-sharing arrangement. Unless separately documented, holding dZWG does not confer corporate rights, dividend rights, governance rights, or ownership rights in the issuing entity.

Use of dZWG may be subject to applicable laws relating to digital assets, payments, anti-money laundering, sanctions compliance, reporting, data protection, financial conduct, and consumer protection.

---

## 3. Introduction

Digital Zimbabwe Gold (dZWG) is a blockchain-native token designed to function as a digital representation of Zimbabwe Gold (ZWG). It is created to support a more transparent, auditable, and programmable financial environment while preserving direct alignment with Zimbabwe's domestic unit of account.

The purpose of dZWG is not simply to issue a token on a blockchain. Its purpose is to establish a controlled digital monetary rail capable of supporting payments, treasury operations, regulated disbursements, interoperability, and structured financial workflows. In that sense, dZWG is intended to function as infrastructure rather than as a speculative crypto asset.

The system is designed around a simple monetary proposition: one token should correspond to one unit of Zimbabwe Gold, and the system should be administered in a way that preserves that relationship through reserve-backed issuance discipline, operational controls, and governance oversight.

---

## 4. Background: Zimbabwe's Monetary Landscape

Zimbabwe's monetary history has been shaped by episodes of instability, redenomination, currency restructuring, and changing public confidence in monetary instruments. That history has created a practical demand for reliability, discipline, transparency, and auditable monetary administration.

The adoption of Zimbabwe Gold reflects an effort to establish a structured and domestically aligned monetary framework. However, even when a national unit of account is defined, the practical operation of that unit in digital environments remains a separate challenge. Payment rails may be fragmented, expensive, slow, or insufficiently programmable. That can limit the real economic effectiveness of the underlying currency.

dZWG is designed to address that gap. It does not seek to replace Zimbabwe Gold. Instead, it extends Zimbabwe Gold into blockchain-based financial infrastructure, allowing the domestic currency to operate in programmable and interoperable digital environments.

---

## 5. Problem Statement

The core problem addressed by dZWG is the absence of a robust, compliant, and auditable digital representation of Zimbabwe Gold for blockchain-native payments and settlement.

In the absence of such a system, digital financial activity tends to default toward foreign-currency stablecoins, fragmented payment intermediaries, informal settlement methods, or systems that lack clear issuance discipline and reserve transparency. This can produce a mismatch between domestic monetary policy, user behavior, and settlement infrastructure.

A second problem is limited programmability. Traditional payment systems often do not provide flexible on-chain automation for payroll, merchant settlement, treasury flows, cross-border coordination, and policy-aware disbursement systems.

A third problem is institutional visibility. Without explicit on-chain controls and governance structures, digital value systems may operate without sufficient auditability, compliance enforcement, or operational clarity.

dZWG is designed to address these problems through a reserve-backed, role-governed, auditable digital ZWG layer.

---

## 6. Why dZWG

The strategic case for dZWG rests on monetary alignment, institutional control, technical programmability, and regional interoperability.

Monetary alignment is fundamental. A Zimbabwean digital currency system intended to support domestic payments and financial operations should remain tied to Zimbabwe Gold rather than defaulting to a foreign-currency base. dZWG preserves that domestic reference unit.

Institutional control is equally important. dZWG is designed with explicit governance, administrative controls, compliance features, reserve discipline, and timelocked upgrades. This allows the system to function as managed financial infrastructure rather than an uncontrolled token system.

Technical programmability provides an additional advantage. A blockchain-native representation of ZWG can support automated and transparent financial workflows, including payroll logic, treasury operations, merchant settlement, programmable disbursements, and interoperable cross-border payment channels.

Regional interoperability strengthens the long-term case. dZWG is intended to operate alongside NADD, AOAk, dZMW, and ACHA as part of a broader African domestic-currency stablecoin framework.

---

## 7. Design Principles

The design of dZWG is governed by several core principles.

The first is monetary integrity. The token is intended to maintain a strict one-to-one relationship with Zimbabwe Gold and is not designed as an algorithmic or floating-value token.

The second is full reserve backing. Circulating supply is intended to remain fully backed by reserves denominated in ZWG, with issuance governed accordingly.

The third is transparency. Administrative actions, supply changes, and protocol state transitions should be visible and auditable on-chain where appropriate.

The fourth is compliance by design. dZWG is intended for real financial use, which requires KYC, AML, sanctions controls, emergency intervention capability, and policy-aware account restrictions.

The fifth is institutional manageability. Governance and operations must be expressible through explicit roles, multisignature controls, timelocks, and auditable change-management practices.

The sixth is interoperability. dZWG is designed for use within a broader EVM-compatible digital financial environment.

---

## 8. System Overview

At a high level, dZWG is a reserve-backed tokenized payment and settlement layer. Authorized roles may mint and burn tokens. Transfers occur on-chain and can be subject to fees, compliance checks, and emergency restrictions. Administrative functions are governed through explicit access control.

The system includes two interdependent dimensions. The on-chain layer manages balances, supply mechanics, administrative controls, compliance logic, and event logging. The off-chain layer manages reserve custody, reconciliation, attestation, compliance records, governance procedures, and redemption settlement.

Institutionally, this means dZWG should be understood as both a smart contract system and an operational financial product.

---

## 9. Technical Architecture

dZWG is implemented as an ERC-20-compatible token using a UUPS upgrade pattern and an ERC-1967 proxy structure. This allows the user-facing address to remain stable while logic upgrades are executed through governed processes.

The primary production deployment network is BNB Chain Mainnet. The design remains EVM-compatible, allowing future expansion or interoperability with other compatible networks if required.

The core architecture includes the following components:

The token core manages balances, transfers, and ERC-20 compatibility.

The upgradeability layer permits controlled logic upgrades through authorized governance.

The access control layer defines administrative and issuer permissions.

The compliance layer supports account restrictions, sanctions flags, freeze controls, and KYC-aware transfer restrictions.

The reserve layer supports reserve-linked issuance discipline and reserve attestation processes.

The fee layer applies basis-point transfer fees and routes them to a designated treasury address.

The redemption layer records redemption requests and processing outcomes.

The event layer provides audit-oriented operational visibility.

---

## 10. Reserve Custody and Asset Policy

dZWG is intended to be fully backed by reserves denominated in Zimbabwe Gold.

Reserves are held in regulated banking institutions within Zimbabwe or approved jurisdictions, in the form of cash or cash-equivalent instruments denominated in ZWG. Permitted reserve assets may include demand deposits, short-duration cash-equivalent instruments, and other highly liquid reserve assets denominated in ZWG. Prohibited reserve assets include speculative instruments, equity instruments, long-duration investments, and unrelated volatile assets.

Reserves are maintained in segregated accounts and are held for the benefit of dZWG holders. They are not intended to be commingled with operating funds, pledged, encumbered, or rehypothecated.

Reserve movement is controlled through multisignature governance. No single individual should have unilateral authority to move reserve assets.

This custody model is central to the institutional credibility of the token. Reserve language is not decorative; it is an operating rule.

---

## 11. Reserve Attestation and Reporting

The reserve governance framework uses layered verification.

Internal reserve reconciliation is performed daily as an operational control. Formal management attestation is conducted weekly. Periodic independent third-party review or assurance procedures may be conducted to validate reserve integrity and governance controls.

Reserve discrepancies, if identified, may trigger immediate suspension of new issuance until resolved. Material discrepancies may also trigger governance escalation, internal investigation, and disclosure procedures.

Institutionally, this means dZWG does not rely only on a broad reserve statement. It relies on reserve administration, reconciliation, and periodic reporting discipline.

---

## 12. Reserve Shortfall Policy

If reserves fall below circulating supply, the system enters an exception condition.

In such circumstances, new issuance is suspended immediately. Governance escalation is triggered, internal reconciliation is performed, and reserve causes are investigated. Material shortfalls may require public disclosure depending on severity, legal requirements, and operating policy.

During a reserve exception event, redemption handling may be adjusted to preserve system integrity and prevent disorderly depletion of reserves.

This policy is essential because reserve backing is meaningful only if the system defines what happens when reserve discipline fails.

---

## 13. Issuance Framework

Token issuance is restricted to authorized issuer roles. Public minting is not permitted.

New dZWG tokens are minted only when corresponding reserve value is established within the custody and governance framework. This ensures that issuance is tied to reserve-backed operational conditions rather than discretionary or speculative supply expansion.

Institutionally, issuance should be understood as a reserve-linked administrative process rather than as a market-driven token generation mechanism.

---

## 14. Redemption Framework

Redemption of dZWG is available to verified participants subject to compliance requirements.

Redemptions may be made directly with the issuer or through authorized intermediaries. Minimum redemption thresholds may apply depending on policy. Redemption requests may be subject to KYC, sanctions checks, account review, and operational validation.

The target redemption settlement time is T+1 to T+2 business days, although actual timing may vary depending on operational conditions, banking hours, jurisdictional factors, and system demand.

Redemption fees may apply under issuer policy.

Redemptions are generally processed in order received, but may be batched for operational efficiency. In stress scenarios, the issuer may adjust processing in order to preserve system integrity, maintain orderly settlement, or comply with regulatory requirements.

---

## 15. Compliance, KYC, AML, and Sanctions Controls

dZWG is designed with explicit compliance controls.

These include tiered KYC logic, blacklist capability, sanctions flags, account freeze functionality, and full pause capability at the system level. Higher transaction volumes may require stronger identity verification.

Personal data and identity records are handled off-chain within compliance systems. On-chain addresses may be linked to off-chain compliance records in accordance with applicable legal and regulatory requirements.

These controls are not incidental. They materially affect use of the token and are part of the institutional design of the system.

---

## 16. Governance and Administrative Control Model

The governance structure of dZWG is role-based.

The issuer role governs minting and burn-related supply actions. The admin role governs compliance controls, parameter changes, treasury settings, and other sensitive system functions. Critical administrative functions are governed through multisignature authorization.

The multisignature operating model is intended to follow a threshold-based pattern, such as three-of-five or four-of-seven approvals, depending on final governance policy. Signers may include operational representatives, treasury representatives, and designated governance participants. Signer rotation and authority updates are governed under internal administrative policy.

This governance framework is intended to reduce unilateral control while preserving administrative responsiveness.

---

## 17. Upgrade and Change Management Policy

dZWG uses a UUPS upgradeability model governed through a timelocked request-and-execute process.

Routine upgrades are subject to a timelock period, typically between twenty-four and seventy-two hours. Critical upgrades may be executed under accelerated procedures if governance policy permits and multisignature approval thresholds are satisfied.

All upgrades are recorded on-chain. Upgrade events should be publicly visible. Governance policy may also require public communication before execution where appropriate.

This structure is intended to prevent silent logic changes and to introduce procedural discipline into upgrade execution.

---

## 18. Fees and Treasury Policy

dZWG includes a transfer fee mechanism expressed in basis points.

Fees are routed to a designated fee collector or treasury address controlled through governance. Certain addresses may be exempt from fees where operationally necessary.

Fee policy is not static by assumption. It is governed. Parameters may be adjusted by authorized governance subject to defined limits and internal controls.

Treasury segregation remains important. Treasury addresses and fee collection are not intended to alter the reserve-backing model. Fees are distinct from reserve assets.

---

## 19. Token Holder Rights and Limitations

Holding dZWG does not grant equity ownership in the issuer. It does not create voting rights, profit participation, dividend rights, or governance rights unless separately and explicitly granted by another framework.

dZWG functions as a digital payment and settlement instrument within the issuer's governance framework.

Holders should not interpret possession of dZWG as ownership of reserve accounts or corporate interests.

---

## 20. Supported Users and Access

dZWG is designed for use by individuals, merchants, enterprises, institutions, and fintech platforms.

Access to certain features or settlement pathways may be restricted based on compliance status, jurisdiction, transaction size, institutional onboarding requirements, or operating policy.

The system is not limited to retail use. It is intended to serve structured operational finance as well.

---

## 21. Jurisdictional Scope

dZWG is primarily intended for Zimbabwe-linked monetary and settlement use cases.

International access may be permitted subject to compliance restrictions, licensing considerations, and jurisdictional policy. Certain jurisdictions may be restricted entirely.

Institutional readers should understand dZWG as a Zimbabwe-focused digital monetary instrument with potentially broader interoperability, not as an unrestricted global consumer token.

---

## 22. Infrastructure Dependency and Network Risk

dZWG currently relies on BNB Chain infrastructure. This introduces dependencies on network availability, validator operation, gas conditions, wallet infrastructure, RPC providers, indexers, and third-party transaction interfaces.

Users and integrators therefore bear blockchain-related risks, including congestion, network instability, interaction mistakes, wallet custody failures, and dependency on external infrastructure providers.

These are normal risks for EVM-native digital financial systems, but they remain material and must be disclosed.

---

## 23. Market Structure and Secondary Trading Disclaimer

If dZWG is listed or traded on secondary markets, those market prices may vary independently of the formal redemption framework.

The issuer does not guarantee that secondary market pricing will always reflect the formal one-to-one reserve-backed model in real time. Market spreads, liquidity conditions, and venue-specific behavior may create temporary divergence.

The reserve-backed redemption framework is therefore distinct from open-market trading conditions.

---

## 24. Security Architecture

The contract architecture includes reentrancy protection, pausable execution controls, role-based access restrictions, multisignature governance, and timelocked upgrade procedures.

OpenZeppelin-based contract modules are used to reduce custom low-level security risk. However, contract security remains only one part of the full risk model. Key management, reserve administration, operational processes, and governance integrity remain equally important.

Institutional security therefore depends on both code quality and operating discipline.

---

## 25. Economic Model and Tokenomics

dZWG is not designed for speculative yield generation, staking inflation, or reflexive price discovery. Its primary economic purpose is to represent Zimbabwe Gold in digital form.

Supply is elastic and expands or contracts through authorized issuance and redemption. There is no fixed hard cap because reserve backing, rather than arbitrary scarcity, is the relevant monetary constraint.

The token does not inherently bear interest or yield unless separately documented under another framework.

---

## 26. Wind-Down and Orderly Termination Framework

If the issuer elects to discontinue dZWG, or if a termination event occurs, the system is intended to enter an orderly wind-down phase.

During wind-down, new issuance ceases permanently. Redemptions remain available for a defined period subject to compliance requirements and operational capability. Governance oversees the reduction of circulating supply and the orderly administration of remaining reserves.

This framework is intended to reduce uncertainty in termination scenarios and to preserve fairness, reserve discipline, and procedural clarity.

---

## 27. Risk Factors and Mitigations

Reserve risk remains material because reserve assets are held off-chain. This is mitigated by segregation, custody policy, reconciliation, and attestation, but it cannot be eliminated purely through smart contracts.

Smart contract risk remains present in any blockchain system. This is mitigated through tested contract architecture, widely used libraries, controlled upgrades, and staged deployment.

Regulatory risk remains relevant because legal treatment of digital financial instruments may evolve. This is mitigated by compliance-aware architecture and adaptable governance.

Operational risk remains significant in issuance, redemption, custody, reconciliation, and key management. This is mitigated by role separation, multisignature controls, and policy-based administration.

Governance risk remains material because administrative roles hold meaningful power. This is mitigated by multisig thresholds, timelocks, disclosure, and internal controls.

---

## 28. Parameter Governance Summary

The table below summarizes key parameters and their governance significance.

| Parameter | Default Value | Governance Control |
|-----------|---------------|--------------------|
| Transfer Fee | 10 basis points | Admin / Governance |
| Mini KYC Threshold | 500 dZWG | Admin / Governance |
| Fee Collector | Governance-set address | Admin / Governance |
| Pause Authority | Enabled | Multisig Governance |
| Upgrade Authority | Multisig-controlled | Timelocked Governance |
| Reserve Signer / Attestation Controls | Governance-set | Admin / Governance |

---

## 29. Deployment and Network Information

dZWG is deployed on BNB Chain Mainnet using an upgradeable proxy architecture.

Name: dZWG  
Symbol: dZWG  
Decimals: 18  
Network: BNB Chain Mainnet  
Upgrade Model: UUPS with ERC-1967 proxy structure

Mainnet proxy address:  
`0xb764383a8A0502c1CF6d58c9de3bA7e5AACdeeA3`

Mainnet implementation address:  
`0x9D596814CcA04A083a470014eacF7eDC2aA531e2`

Default transfer fee parameter:  
10 basis points

Default mini KYC threshold:  
500 dZWG

**Mini KYC Threshold**

The mini KYC threshold is set at 500 dZWG and defines the level below which simplified customer due diligence may apply.

Transactions are evaluated on both a per-transaction basis and a cumulative daily basis.

Where a user:
(i) initiates a single transaction exceeding 500 dZWG; or  
(ii) conducts multiple transactions within a 24-hour period that cumulatively exceed 500 dZWG,  

the user is required to complete full customer due diligence (KYC) prior to further transaction processing.

Transactions at or below 500 dZWG, on both a per-transaction and cumulative daily basis, may be permitted under reduced KYC requirements, subject to ongoing monitoring and compliance controls.

This framework aligns with a risk-based approach to customer due diligence, ensuring proportional compliance for low-value transactions while enforcing enhanced verification for higher-risk activity.

---

## 30. Roadmap and Implementation Path

The development path for dZWG follows a staged infrastructure model.

The first phase is architecture design and contract development.  
The second phase is controlled testnet deployment and operational validation.  
The third phase is mainnet deployment and public on-chain activation.  
The fourth phase is reserve administration, issuance enablement, and wallet integration.  
The fifth phase is enterprise and institutional onboarding.  
The sixth phase is interoperability with other domestic-currency digital assets in the broader ecosystem.  
The seventh phase is continuing audit, governance refinement, and infrastructure hardening.

---

## 31. Technical Appendix

dZWG is implemented as an ERC-20-compatible token using a UUPS upgradeability model and ERC-1967 proxy structure. The contract includes role-based access control, transfer fees, compliance controls, reserve-related logic, and upgrade governance.

Administrative controls include issuer management, treasury parameter updates, sanctions flags, account freezing, blacklist logic, and pause capability.

The system is intentionally designed as governed financial infrastructure rather than as a permissionless or purely decentralized token system.

---

## 32. ASCII Diagrams

```text
+-------------------------+
|       dZWG System       |
+-------------------------+
            |
    +-------+-------+
    |               |
  Users         Enterprises
    |               |
    +-------+-------+
            |
       Payments Layer
```

```text
+-------------------------+
|  Multisig Governance    |
+-------------------------+
| Issuer | Admin | Ops    |
+-------------------------+
            |
    Timelocked Upgrades
```

---

## 33. References

1. OpenZeppelin Contracts Documentation: https://docs.openzeppelin.com/contracts
2. ERC-20 Standard: https://eips.ethereum.org/EIPS/eip-20
3. ERC-1967 Proxy Standard
4. UUPS Upgrade Pattern
5. BNB Chain Documentation
6. Reserve Bank of Zimbabwe: https://www.rbz.co.zw/

---

End of Document
