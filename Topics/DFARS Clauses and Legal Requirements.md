---
title: DFARS Clauses and Legal Requirements
aliases:
  - DFARS
  - DFARS 252.204-7012
  - DFARS 252.204-7021
  - Legal Requirements
tags:
  - cmmc
  - dfars
  - legal
  - compliance
confidence: confirmed
last_verified: 2026-02-20
sources:
  - "[[When is CMMC Required]]"
  - "[[The End of SPRS Scores (sort of)]]"
  - "[[When CMMC Meets Contracts]]"
---

## Summary
Four DFARS clauses form the legal foundation for CMMC: 7012 (CUI protection), 7019 (self-assessment scoring), 7020 (DIBCAC audit authority), and 7021 (CMMC certification). The first three are already enforceable in contracts today; 7021 is in Phase 1 rollout and adds the third-party verification layer.

## Key Facts
- **DFARS 7012** -- already required in contracts with CUI; mandates NIST 800-171 implementation
- **DFARS 7019** -- already required; mandates NIST 800-171 self-assessment score submission to SPRS
- **DFARS 7020** -- already required; gives DoD (DIBCAC) the right to audit your compliance. Has been in contracts **since 2020** -- [[DIBCAC and DCMA Assessments|DIBCAC]] (under DCMA) is the entity that exercises this audit authority
- **DFARS 7021** -- Phase 1 rollout underway; requires third-party or self-assessment CMMC certification
- CMMC (via 7021) is **completely separate** from DFARS 7020 audits -- a DIBCAC audit under 7020 covers all of DFARS 7012 (flowdown, incident reporting, cloud computing), not just NIST 800-171
- 7021 sits **on top of** 7012/7019 -- it does not replace them
- CMMC is the verification mechanism added by 7021, not a new set of controls

## How It Works
### The DFARS Clause Stack

The four clauses work together as a stack:

| Clause | What It Does | Status |
|---|---|---|
| **DFARS 252.204-7012** | CUI protection -- requires NIST 800-171 implementation | **Already required** in contracts with CUI |
| **DFARS 252.204-7019** | Self-assessment -- requires NIST 800-171 assessment score in SPRS | **Already required** |
| **DFARS 252.204-7020** | DIBCAC authority -- gives DoD the right to audit you | **Already required** |
| **DFARS 252.204-7021** | CMMC certification -- requires third-party or self-assessment certification | **Phase 1 rollout underway** |

### How They Relate
7012 establishes the **what** (implement NIST 800-171 to protect CUI). 7019 establishes the **reporting** (submit your score to SPRS). 7020 establishes the **enforcement** (DoD can come check). 7021 adds the **verification** (prove it through CMMC certification).

You cannot comply with 7021 without first complying with 7012 and 7019. CMMC does not introduce new controls -- it verifies you actually implemented the ones 7012 already requires.

## Decision Criteria
- **Contract contains CUI** --> DFARS 7012 applies, NIST 800-171 is mandatory today
- **7019 in contract** --> You must have a current self-assessment score in SPRS
- **7020 in contract** --> DoD can audit your implementation at any time
- **7021 in contract** --> You need CMMC certification (Level 2 for CUI)
- **7021 not in your contract yet** --> Prepare anyway; it is being added to contracts now (see [[Phase Rollout and Contract Language]])

## Common Misconceptions
| Misconception | Reality | Source |
|---|---|---|
| CMMC replaces DFARS 7012 | 7021 and CMMC sit on top of 7012/7019 -- they do not replace them | [[When is CMMC Required]] |
| You only need to worry about compliance when 7021 appears | 7012 already requires NIST 800-171 implementation for CUI contracts -- you should already be compliant | [[When is CMMC Required]] |
| CMMC is a new set of controls | CMMC is a verification mechanism; the controls are NIST 800-171, already required under 7012 | [[When is CMMC Required]] |
| The FAR overhaul kills CMMC | CMMC is codified at 32 CFR (not 48 CFR) with a statutory basis in FY20 NDAA Section 1648 -- the FAR overhaul cannot change a different title of the CFR | [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] |

### DFARS Clauses as Basis for False Claims Act Enforcement

The DFARS cybersecurity clauses form the legal foundation for [[False Claims Act and DOJ Enforcement|FCA enforcement]]:
- **DFARS 7012** requirements (NIST 800-171 implementation, FedRAMP for cloud, incident reporting) are the specific obligations whose violation triggers FCA liability
- **DFARS 7008** (solicitation provision) makes contractors aware they are agreeing to comply with 7012 before signing
- **DFARS 7019/7020** (SPRS scoring) creates a documented, trackable representation of compliance that can be proven false
- In the 2025 FCA settlement, the company's admissions mapped exactly to specific DFARS 7012 paragraphs: paragraphs C-G (cloud/incident reporting) and paragraph B (800-171 implementation)
- Submitting a SPRS score is a "knowing" representation to the government -- if that score is false, it is a false claim

*(Source: [[DOJ vs Small Defense Contractors]], Summit 7, April 2025)*

### DFARS 7012 Compliance as Material to Contract

The [[Aerojet Rocketdyne]] precedent established that cybersecurity compliance under DFARS 7012 is **material to the contract**. This means submitting invoices without complying with DFARS 7012 constitutes a false claim to the government under the [[False Claims Act and DOJ Enforcement|False Claims Act]]. This is an **existing contractual requirement** -- it is not CMMC-specific. The obligation to implement security controls specified in NIST SP 800-171 to protect DoD information has applied to DoD contracts, subcontracts, and similar contractual instruments **since 2017** and will continue under the CMMC program. CMMC is just the verification mechanism for requirements that have been in contracts for years.

*(Source: [[FCA Whistleblower Strikes Again]], Summit 7, December 2025)*

### Subcontractor Flowdown Requirements (32 CFR 170)

Per 32 CFR 170 section 170.23A3, CMMC requirements flow down to subcontractors:
- If a subcontractor will process, store, or transmit CUI in performance of the subcontract, and the associated prime contract has a requirement for **CMMC Level 2 C3PAO**, then CMMC Level 2 C3PAO is the **minimum requirement** for the subcontractor
- The simplest test: if your prime requires CMMC Level 2 C3PAO, you require it too
- If your prime is Lockheed, BAE, HII, Northrop, RTX, or any major prime, the answer is almost certainly yes -- they will handle CUI requiring that level of assurance
- Even if CMMC assessment requirements are waived for a contract, the underlying cybersecurity clauses (**FAR 52.204-21**, **DFARS 7012**, **DFARS 7020**) remain in full effect

*(Source: [[Primes Can't Waive CMMC]], Summit 7, December 2025)*

### Key Timeline of DFARS Cyber Clauses
- **2016:** DFARS 252.204-7012 revised to require NIST SP 800-171; DFARS 252.204-7008 provision added to solicitations
- **2020:** DFARS 252.204-7019 and 7020 created (SPRS scoring and DIBCAC audit authority)
- **March 2021:** CMMC 1.0 paused for strategic review, but 7019/7020 remained in effect
- **November 2024:** CMMC 2.0 final rule published; DFARS 7021 created
- **December 2024:** CMMC program goes into effect (voluntary assessments)
- **November 2025:** DFARS 7021 contract clause language becomes effective (Phase 1)

*(Source: [[DOJ vs Small Defense Contractors]], Summit 7, April 2025; [[CMMC Phase 1 - What Comes Next]], November 2025)*

### SPRS Score and FedRAMP Gap Issue

A growing problem for contractors who meet all 110 NIST 800-171 controls but do **not** meet [[FedRAMP Requirements|FedRAMP]] requirements (e.g., hosting CUI in a non-FedRAMP Moderate cloud). SPRS has no checkbox to indicate FedRAMP compliance status, so what score do you submit? According to Don Stern (DLA Piper), there is no one-size-fits-all answer, but several approaches exist:

- **Submit 109** -- give yourself one point lower as a heads-up to the government that something is not fully met
- **Add proposal language** -- include a disclosure in proposals (drafted by counsel) putting the government on notice of the gap
- **Document via POA&M** -- internally document the gap and your plan to remediate

The critical principle: **do not bury your head in the sand.** Transparency with the government about your compliance posture is essential. Claiming a perfect 110 while knowingly failing FedRAMP requirements creates [[False Claims Act and DOJ Enforcement|False Claims Act]] exposure.

A contributing factor: in October 2024, **Microsoft pulled FedRAMP authorization from M365 Commercial**. A 60,000-person defense contractor discovered they were non-compliant as a result. Many companies remain unaware of this change because cloud vendors do not proactively notify customers of FedRAMP status changes.

*(Source: [[When CMMC Meets Contracts]], Summit 7, February 2026)*

### CMMC Agnostic of Company Size and Set-Asides

CMMC requirements **trump small business set-asides** -- SBA, veteran-owned, disabled, minority, woman-owned, and all other set-aside categories. If the data goes and the clause goes, CMMC applies regardless of company size or set-aside status. The burden of implementation and certification can cost smaller organizations hundreds of thousands of dollars over a multi-year process. This is expected to drive **potentially 40% or more of companies to exit the defense supply chain**, preferring commercial work until the [[DFARS Clauses and Legal Requirements#FAR CUI Rule|FAR CUI rule]] extends requirements to all federal work.

*(Source: [[When CMMC Meets Contracts]], Summit 7, February 2026)*

### FAR CUI Rule

The FAR CUI rule is expected to extend cybersecurity requirements beyond DoD to **all federal work**. This has been described as the "white whale" of the CUI program for 10 years. A proposed rule was published in January 2025. The final rule is expected to be included in the omnibus FAR overhaul rulemaking (see [[Waivers and Class Deviations#Revolutionary FAR Overhaul|Revolutionary FAR Overhaul]]). When enacted, companies that exit DoD work to avoid CMMC will find they cannot escape cybersecurity requirements in the broader federal market either.

*(Source: [[When CMMC Meets Contracts]], Summit 7, February 2026; [[The End of SPRS Scores (sort of)]], Summit 7, February 2026)*

### 2026 FAR Overhaul and Clause Renumbering

In August 2025, the Office of Federal Procurement Policy launched the **Revolutionary FAR Overhaul (RFO)** -- the first major overhaul and largest single update to the FAR in its 40-year history. The goal is to rewrite the FAR in plain language and eliminate up to one-third of its content. The policy basis comes from Executive Order 14275 ("Restoring Common Sense to Federal Procurement"), EO 14265, and OMB Memo M-25-26.

As of **February 1, 2026**, 38 DFARS class deviations went into effect. The key changes to cybersecurity clauses:

| Original | New | What Changed |
|---|---|---|
| **FAR 52.204-21** | **FAR 52.240-93** | Same title ("Basic Safeguarding of Covered Contractor Information Systems"), same 15 requirements, different number |
| **DFARS 252.204-7019** | *Deleted entirely* | Provision no longer exists |
| **DFARS 252.204-7020** | **DFARS 252.204-7997** | Same title ("NIST SP 800-171 DoD Assessment Requirements"), but basic self-assessment requirement **removed**. Medium and high assessments unchanged. |
| **DFARS 252.204-7012** | *No change* | Unchanged |
| **DFARS 252.204-7021** | *No change* | CMMC clause unchanged |
| **DFARS 252.204-7025** | *No change* | CMMC provision unchanged |

**Why it happened:** The basic self-assessment under old 7019/7020 was redundant with the CMMC Level 2 self-assessment under 7021. Now only CMMC score uploads apply when applicable. This removes a source of confusion where contractors had two overlapping assessment obligations.

**The "ghost clauses" problem:** CMMC still references FAR 52.204-21, which is now 52.240-93. These references will not be normalized until rulemaking completes -- probably 2+ years. CCP instructors must teach with approved materials that reference the old (now dead) clause numbers. Contractors will see 7997 in solicitations and contracts, but **cannot Google it** because the class deviation text has not been incorporated into Title 48 of the CFR through rulemaking.

*(Source: [[The End of SPRS Scores (sort of)]], Summit 7, February 2026)*

### CIRCIA Rule Revival -- DHS Duplicating DFARS 7012

The **Cyber Incident Reporting for Critical Infrastructure Act (CIRCIA)** is back after disappearing following an extended comment period. Key facts:

- Originated after the 2021 Colonial Pipeline attack -- directed DHS to create incident reporting rules for all 16 critical infrastructure sectors
- Produced a **450-page proposed rule** that, for the defense industrial base sector, **completely duplicated** the incident reporting obligations already in DFARS 7012
- DHS and DoD have had **zero coordination** on this issue -- despite defense contractors being the most affected "covered entities" under the rule
- DHS is conducting new town halls, including a **DIB-specific town hall on March 19, 2026** at 12:00 Eastern
- The simple fix would be for DHS to accept existing DoD-mandated incident reporting rather than requiring defense contractors to report twice
- The rule is a DHS rule, not a DoD rule -- yet more defense contractors are affected as covered entities than any other sector

*(Source: [[The CUI Hotline - Weekly CMMC Q&A Livestream!]], Summit 7, February 2026)*

### FAR Overhaul Does NOT Kill CMMC

The FAR/DFARS overhaul removing basic self-assessments from DFARS 7020 has led some to conclude CMMC is "on the chopping block." This is incorrect:

- **CMMC is codified at 32 CFR** (Part 170) -- the FAR and DFARS are at **48 CFR**. The FAR overhaul cannot change a different title of the Code of Federal Regulations.
- **Statutory basis**: The CMMC program is required by the **FY20 NDAA Section 1648** -- this is a statutory requirement that has been in place since 2020
- The FAR overhaul preserves anything with a statutory requirement -- CMMC has one
- **DFARS 7021** (CMMC certification clause) and **DFARS 7025** (CMMC provision) are **unchanged** by the overhaul
- The removal of basic self-assessments from 7020 was specifically to eliminate redundancy with CMMC Level 2 self-assessments -- same scoring, same assessment, same requirements under two different clauses

*(Source: [[The CUI Hotline - Weekly CMMC Q&A Livestream!]], Summit 7, February 2026)*

## Open Questions / Debates

- **Does pausing CMMC 1.0 reduce FCA exposure?** No. The 2025 FCA settlement covered 2018-2023, a period when CMMC was paused but DFARS 7012/7019/7020 remained fully in effect. CMMC's status is irrelevant to DFARS 7012 compliance obligations. *(Source: [[DOJ vs Small Defense Contractors]], April 2025)*

## Related Topics
- [[CMMC Levels and Framework Structure]] -- the certification levels that 7021 requires
- [[Phase Rollout and Contract Language]] -- how and when 7021 is appearing in contracts
- [[Assessment Process and Timeline]] -- what the 7021 certification process looks like
- [[False Claims Act and DOJ Enforcement]] -- how DFARS clauses form the basis for FCA claims
- [[SPRS and Annual Affirmation]] -- SPRS scoring as a trackable compliance representation

## Sources
- [[When is CMMC Required]] -- complete DFARS clause stack breakdown, how clauses relate, enforcement status
- [[DOJ vs Small Defense Contractors]] -- DFARS clauses as basis for FCA enforcement, specific paragraph references from settlement admissions, clause timeline
- [[CMMC Phase 1 - What Comes Next]] -- DFARS 7012 as the underlying requirement CMMC verifies, FAR 52.204-21 for Level 1
- [[FCA Whistleblower Strikes Again]] -- DFARS 7012 compliance as material to contract (Aerojet Rocketdyne precedent), invoices without compliance = false claim
- [[Primes Can't Waive CMMC]] -- 32 CFR 170 section 170.23A3 subcontractor flowdown, FAR 52.204-21 and DFARS 7012/7020 remain even if CMMC waived
- [[DIBCAC Assessment Requirements]] -- DFARS 7020 audit authority exercised by DIBCAC (under DCMA), separation of CMMC assessments from 7020 audits, 7020 in effect since 2020
- [[When CMMC Meets Contracts]] -- SPRS score + FedRAMP gap issue, M365 Commercial FedRAMP loss (October 2024), CMMC trumps small business set-asides, supply chain consolidation (40%+ potentially exiting), FAR CUI rule coming
- [[The End of SPRS Scores (sort of)]] -- FAR overhaul clause renumbering (52.204-21 to 52.240-93, 7020 to 7997), 7019 deletion, 38 DFARS class deviations (February 1, 2026), ghost clauses problem, FAR CUI rule in omnibus
- [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] -- CIRCIA rule revival (DHS duplicating DFARS 7012 obligations, March 19 town hall, zero DoD/DHS coordination), FAR overhaul does NOT kill CMMC (32 CFR vs 48 CFR, statutory basis FY20 NDAA Section 1648, DFARS 7021/7025 unchanged)
