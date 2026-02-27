---
title: FedRAMP Requirements
aliases:
  - FedRAMP
  - Federal Risk and Authorization Management Program
  - FedRAMP Moderate
tags:
  - cmmc
  - fedramp
  - cloud
  - compliance
confidence: confirmed
last_verified: 2026-02-20
sources:
  - "[[When is FedRAMP Required]]"
  - "[[The CUI Hotline - Weekly CMMC Q&A Livestream!]]"
---

## Summary
FedRAMP authorization is required when a cloud service processes, stores, or transmits CUI. If the service never touches CUI, FedRAMP is not required -- even if the tool is part of your security stack. This is a common source of confusion, particularly around MFA solutions and security tools.

## Key Facts
- **The CUI test**: Does this cloud service process, store, or transmit CUI? If yes, FedRAMP required. If no, FedRAMP not required.
- **MFA solutions** that never touch CUI do **not** require FedRAMP (confirmed by CyberNorris + Liatris, credentialed practitioners)
- Crypto for **authentication** (MFA) is different from crypto for **CUI protection** -- MFA validates identity, it does not handle controlled data
- Security tools (SIEM agents, vulnerability scanners, EDR) that do not process/store/transmit CUI do not need FedRAMP versions
- If a security tool ingests logs containing CUI or has access to CUI-bearing systems that expose the data, FedRAMP may apply
- GCC High users **must** obtain the FedRAMP [[CRM (Customer Responsibility Matrix)|CRM]] from Microsoft to write their [[SSP Development|SSP]] -- non-negotiable for assessment
- The safe bet is to align with FedRAMP requirements now rather than wait for explicit DoD guidance

## How It Works
### The CUI Test
A cloud service provider (CSP) needs FedRAMP authorization when it handles CUI on behalf of a federal agency or a contractor subject to DFARS 7012. The single determining question:

**Does this cloud service process, store, or transmit CUI?**
- **Yes** --> FedRAMP required
- **No** --> FedRAMP not required

### MFA Solutions
MFA providers like Okta are one of the most frequently asked questions. The community consensus:
- MFA solutions that never touch CUI do **not** require FedRAMP
- The cryptographic operations in MFA verify **authenticity** (proving who you are), not **CUI confidentiality**
- This is a fundamentally different requirement than encrypting CUI at rest or in transit

### Security Tools
Security tools in your environment that do not process, store, or transmit CUI do not need FedRAMP versions. This includes:
- SIEM agents
- Vulnerability scanners
- EDR solutions

**However**, if a security tool ingests logs that contain CUI or has access to CUI-bearing systems in a way that exposes the data, the calculus changes. This is a [[Scoping and Assessment Boundaries|scoping question]].

### GCC High and the FedRAMP CRM
If your organization is on GCC High:
1. You need the FedRAMP CRM from Microsoft
2. Without it, you cannot properly document shared responsibilities in your SSP
3. Many companies get stopped at [[Assessment Process and Timeline|Phase 1]] because their SSP does not adequately address CRM references
4. The CRM is available through the FedRAMP package but must be specifically requested

## Decision Criteria
- **Cloud service processes CUI** --> FedRAMP required
- **Cloud service is MFA only, never touches CUI** --> FedRAMP not required
- **Security tool does not ingest CUI or CUI-bearing logs** --> FedRAMP not required
- **Security tool has access to CUI data** --> FedRAMP may be required; evaluate as a scoping question
- **On GCC High** --> Get the FedRAMP CRM from Microsoft; it is required for your SSP
- **Edge case with no clear answer** --> Align with FedRAMP now; "If and when DoD provides an answer it's very safe to believe they'll follow suit with FedRAMP." -- Uncouth, CCP

## Common Misconceptions
| Misconception | Reality | Source |
|---|---|---|
| "All our cloud tools need FedRAMP" | Only tools that handle CUI require FedRAMP | [[When is FedRAMP Required]] |
| "Okta needs to be FedRAMP authorized" | Not if it never touches CUI -- MFA validates identity, not CUI | [[When is FedRAMP Required]] |
| "We can skip FedRAMP because we're small" | Size does not matter -- CUI handling is the determining factor | [[When is FedRAMP Required]] |
| "Our antivirus needs FedRAMP" | Only if it processes/stores CUI (unlikely for most AV tools) | [[When is FedRAMP Required]] |
| "We're on GCC High so we're covered" | You still need the CRM to properly document your SSP | [[When is FedRAMP Required]] |

## Case Study: Weapons Manufacturer in M365 Commercial

A large, household-name weapons manufacturer was operating in **M365 commercial** (not GCC or GCC High) while handling ITAR-controlled technical data packages. During a CMMC-related conversation about cloud providers, Summit 7 showed the company's IT team Microsoft's contractual terms, which make clear that Microsoft commercial does not guarantee ITAR data sovereignty -- Microsoft will not prove that data has not been released to non-US persons or accessed from outside the United States (e.g., during disaster recovery operations).

The IT team initially believed they were compliant. Summit 7 recommended they bring their **trade compliance team** into the conversation. About 30 seconds into the follow-up meeting, the trade compliance team reviewed the Microsoft terms and the ITAR crosswalk and immediately stated: "No, we're actually in violation and we need to hang up the call right now and we need to go remediate things."

This case illustrates:
- **The IT-trade compliance silo**: IT teams often do not coordinate with trade compliance on cloud infrastructure decisions
- **Commercial cloud is insufficient for ITAR**: M365 commercial does not provide the contractual guarantees required for [[Export Control and CUI Distinctions|ITAR data sovereignty]]
- **CMMC as a catalyst**: This violation would likely never have been discovered without CMMC driving conversations about cloud data sovereignty
- **Dual liability**: The company faced both potential DFARS 7012/CUI violations and ITAR export control violations simultaneously

*(Source: [[The Intersection of CMMC & Export Control]], Summit 7, October 2025)*

## Open Questions / Debates
There remains ambiguity in some edge cases around FedRAMP applicability. The general community expectation is that DoD guidance, when it arrives, will align with FedRAMP requirements. As Uncouth (CCP) noted: "If and when DoD provides an answer it's very safe to believe they'll follow suit with FedRAMP."

The safe approach is to align with FedRAMP requirements now rather than wait for explicit DoD guidance that may take months or years to materialize.

## Related Topics
- [[CRM (Customer Responsibility Matrix)]] -- GCC High FedRAMP CRM required for SSP documentation
- [[ESP (External Service Provider) Classification]] -- FedRAMP applies when cloud ESPs handle CUI
- [[Scoping and Assessment Boundaries]] -- FedRAMP applicability is a scoping question
- [[SSP Development]] -- CRM from FedRAMP package needed for SSP
- [[DFARS Clauses and Legal Requirements]] -- DFARS 7012 is the legal basis for CUI cloud requirements
- [[CMMC Levels and Framework Structure]] -- FedRAMP required for cloud services handling CUI at Level 2
- [[Reassessment and Significant Changes]] -- FedRAMP significant change definitions used as proxy for CMMC

## Sources
- [[When is FedRAMP Required]] -- CUI test rule, MFA exemption, security tool guidance, GCC High CRM requirement, community expectations, common mistakes table
