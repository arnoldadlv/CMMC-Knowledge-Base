---
title: CMMC Case Studies
aliases:
  - Case Studies
  - Real-World Examples
  - DOJ Cases
tags:
  - cmmc
  - reference
  - case-studies
  - enforcement
last_verified: 2026-02-20
---

## Overview

Real-world examples of CMMC enforcement actions, assessment experiences, and implementation outcomes. Each case study includes specific numbers, dates, and outcomes where available.

## DOJ Enforcement Actions

### Small Defense Contractor FCA Settlement (March 2025)

**Company Profile:** ~150 employees, contracts with U.S. Army and Air Force, standard DFARS 7012/7019/7020 clauses

**Settlement:** $4.6 million plus interest

**Key Details:**
- Submitted [[SPRS and Annual Affirmation|SPRS]] score of **104** (max 110); actual score was **negative 142**
- Third-party consultant revealed the true score in summer 2022; company **did not update** their SPRS score
- Head of security left in January 2023 and filed whistleblower complaint
- DOJ served subpoena within 60 days of the whistleblower complaint
- Company gradually rebuilt score: 57 (June 2023) --> 82 (October 2023) --> 110 (Spring 2024)
- Despite achieving perfect score by 2024, settled for $4.6M for violations between 2018-2023

**What They Admitted:**
1. Used third-party email host without FedRAMP Moderate compliance (DFARS 7012 paragraphs C-G)
2. Had not fully implemented NIST SP 800-171 controls (DFARS 7012 paragraph B)
3. Had no consolidated SSP from 2018-2021
4. Submitted false SPRS score of 104; knew actual score was -142; did not update until after subpoena

**Payment Terms:** $1M within 14 days; $3.6M within 60 days. No payment plan.

**Whistleblower Outcome:** $851,000 (18.5% of settlement); company also paid $198,000 for whistleblower's legal fees

**Context:**
- Comparable to Verizon's $4.1M GSA FCA settlement (2023) -- FCA penalties do not scale by company size
- ~100 similar cases pending in the DOJ system
- Summit 7: "The things they admitted to as part of the settlement is every company... This is you right now."

*(Source: [[DOJ vs Small Defense Contractors]], Summit 7, April 2025)*

See [[False Claims Act and DOJ Enforcement]] for full analysis.

---

### All Five Cybersecurity FCA Settlements in 2025

| # | Company | Date | Settlement | Whistleblower Payout | Key Details |
|---|---|---|---|---|---|
| 1 | **Morse Corp** | March 2025 | $4.6M | ~$851K (18.5%) + $198K legal fees | ~150 employees; false SPRS score (104 vs. actual -142); head of security blew whistle |
| 2 | **Raytheon/Nightwing** | May 2025 | $8.4M | ~$1.5M | Major prime/spinoff |
| 3 | **AeroTurbine** | July 2025 | $1.75M | N/A (self-reported) | PE firm committed the violation; company self-reported non-compliance |
| 4 | **Georgia Tech Research Corp** | September 2025 | $875K | $21K | University research corporation |
| 5 | **Swiss Automation (Illinois Precision)** | December 2025 | $421K | $65K | ~300 employees; quality manager whistleblower; fine from handful of purchase orders for machined DoD parts |

**Summary:**
- 4 out of 5 cases had whistleblowers who received payouts
- Companies ranged from ~150 employees to major primes -- the DOJ does not discriminate by company size
- AeroTurbine self-reported after its PE firm was identified as the source of the violation
- Swiss Automation's fine exceeded the value of the original purchase orders -- this is the nature of treble damages under the FCA
- The DOJ obtained over **$2.9 billion** in total FCA settlements and judgments in fiscal year 2025 (all categories); cybersecurity is a small but rapidly growing fraction

*(Source: [[FCA Whistleblower Strikes Again]], Summit 7, December 2025)*

See [[False Claims Act and DOJ Enforcement]] for full analysis.

---

### Jeff Smedley's Company: $1 Billion Acquisition with CMMC Readiness (February 2024)

**Company Profile:** Large DoD contractor, PE-owned (Arlington Capital), 20+ year history, went through two acquisitions

**Key Details:**
- Jeff Smedley served as CIO and FSO for 20 years
- After acquisition by Arlington Capital, identified CMMC certification as a **value differentiator** for the next sale
- Used the **JSVA (Joint Surveillance Voluntary Assessment)** program -- a dual assessment combining DIBCAC/DCMA-driven assessment with C3PAO assessment
- JSVA provided both a high-confidence SPRS score and CMMC Version 2 Level 2 certification simultaneously
- Was approximately the **7th company to achieve CMMC certification** -- an extreme early adopter
- Company sold in **February 2024 for $1 billion**
- The acquiring company made **"distinct reference to CMMC readiness"** as a valuation multiplier

**Key Takeaway:** CMMC readiness was explicitly cited as contributing to a billion-dollar valuation. This is the strongest documented case of CMMC as a revenue enabler rather than a cost center.

**Executive Buy-In Strategy Used:**
- Framed CMMC as value creation for PE owners, not compliance burden
- Engaged BD team with question: "What would it mean if we can move the needle on gross profit 3-5% and grow net profit 1-3%?"
- Partnered with CFO to structure costs as one-time add-backs (no EBITDA impact)
- Led by example: personally mastered the Level 2 assessment guide, ran artifacts during DIBCAC/C3PAO assessment

*(Source: [[Getting CMMC Executive Buy-In with Jeff Smedley]], Summit 7, July 2025)*

See [[Market Dynamics and Service Needs]] for related analysis on CMMC as competitive advantage.

## Export Control Violations

### Dual-Use Company with Foreign National Access

**Company Profile:** Large company with both military and commercial divisions; global workforce including Chinese nationals

**Key Details:**
- Company had a **military division** and a **commercial division**
- The commercial division employed **Chinese nationals** and other foreign nationals (China, Hong Kong, etc.)
- Without proper **IT access controls**, those foreign nationals allegedly had access to documents, data, and information related to military programs
- China is an actively competing adversary from a defense industrial base perspective
- The accessed data could provide the Chinese defense industrial base a **reverse engineering advantage** on U.S. military technology
- Company ended up under a **consent agreement** with the Department of State

**Root Cause:** Desire for maximum innovation and collaboration across divisions led to insufficient access segmentation between commercial (foreign national accessible) and military (US persons only) data environments.

**Relevance to CMMC:** The Access Control family (NIST 800-171 3.1.x) in CMMC -- controlling which devices, people, and service accounts can access controlled data -- directly addresses this failure pattern. Companies with dual-use operations must ensure IT access controls enforce ITAR nationality-based restrictions, not just CUI role-based restrictions.

*(Source: [[The Intersection of CMMC & Export Control]], Summit 7, October 2025)*

---

### Weapons Manufacturer in Wrong Cloud Environment

**Company Profile:** Large, household-name weapons manufacturer; handles ITAR-controlled technical data packages

**Key Details:**
- Company was operating in **M365 commercial** -- not GCC or GCC High
- IT team believed they were compliant
- Summit 7 showed the IT team **Microsoft's contractual terms** regarding ITAR data sovereignty
- Microsoft commercial does not guarantee that data has not been released to non-US persons or accessed from outside the US (e.g., during disaster recovery)
- Summit 7 recommended bringing the **trade compliance team** into the conversation
- **"About 30 seconds into the follow-up meeting"**, trade compliance reviewed the Microsoft terms and the ITAR crosswalk and stated: "No, we're actually in violation and we need to hang up the call right now and we need to go remediate things."

**Root Cause:** IT and trade compliance operating in silos. Trade compliance handled licensing and classification but never examined the cloud infrastructure. IT managed cloud services but did not understand ITAR data sovereignty requirements.

**Relevance to CMMC:** CMMC-driven conversations about [[FedRAMP Requirements|cloud data sovereignty]] were the catalyst that uncovered this export control violation. Without CMMC, the IT team and trade compliance team would have continued operating independently, unaware of the violation.

*(Source: [[The Intersection of CMMC & Export Control]], Summit 7, October 2025)*

---

### Government Overmarking ITAR on Non-ITAR Documents

**Situation:** Government contractor received documents from the U.S. government marked as CUI with ITAR as the control reason

**Key Details:**
- The contractor (a subcontractor in this case) received documents marked **CUI with ITAR export control** as the control parameter
- Upon analysis, the documents contained **financial and programmatic information** -- not technical data or technology
- A proper jurisdiction and classification analysis showed the content did not meet ITAR definitions
- Best case, the data was **EAR-controlled**; potentially not export-controlled at all (**EAR99**)
- The company had to work through the prime contractor to educate the government that export control markings require actual analysis against ITAR and EAR definitions -- they cannot simply be applied as labels
- Government employees were **"rounding up to be safe"**, applying ITAR markings without performing the required jurisdiction/classification analysis

**Impact:** The overmarking created unnecessary compliance burden on the subcontractor, who was now subject to ITAR access and handling restrictions for documents that did not warrant them. The company had to invest time and resources to challenge the markings through the prime-to-government chain.

**Relevance to CMMC:** This case highlights the interaction between CUI marking accuracy and export control compliance. Overmarked documents force contractors into more restrictive handling requirements than necessary, increasing costs and complexity. Contractors should verify the accuracy of CUI control parameters -- particularly when export control is cited as the reason -- rather than accepting all markings at face value.

*(Source: [[The Intersection of CMMC & Export Control]], Summit 7, October 2025)*

---

## Assessment Experiences

### Top 2 Failed Controls (Fernando Machado, C3PAO Perspective)

**Assessor Profile:** Fernando Machado -- provisional assessor #8, 29th authorized C3PAO (authorized in 2022), booked out 8 months as of December 2024

**Most Common Failures:**

1. **FIPS Validated Cryptography (#1)**
   - Firewalls implemented with the latest firmware but not put into FIPS mode with the correct firmware
   - The technology is deployed but the FIPS validation is not enabled or not properly configured
   - Companies check the FIPS box but do not verify actual FIPS operational mode

2. **Multi-Factor Authentication (#2)**
   - Not a reluctance issue but a **scoping misunderstanding**
   - MFA applied in one area but not another -- especially firewalls
   - Organizations do not realize MFA applies to both privileged and non-privileged accounts across network and local access
   - Partial implementation creates assessment failures

**Common Documentation Red Flags:**
- **Templated policies** with brackets like "insert company name here" or university names from downloaded templates
- **Abnormally short SSPs** -- a 12-page SSP will not make it past the gate
- Controls not addressed to the **assessment objective level** (SP 800-171A -- 320 criteria, not just the 110 controls)
- Non-FedRAMP Moderate cloud providers (e.g., Microsoft 365 Commercial instead of GCC High)
- "Our MSP will handle everything" -- a red flag indicating the OSC does not understand shared responsibility

**Phase 1 Documentation Failures:**
- Companies showing up without an SSP or with SSPs that are templates with minimal tailoring
- No document traceability matrix -- dumping a pile of documents without explaining how they connect to each other
- Missing CRM from ESPs clearly delineating shared responsibilities
- During the voluntary market rollout (2025), **25-40% of companies** that signed up for assessments were told to come back later -- they were not ready
- These "false starts" happen in Phase 1 of the assessment (readiness/sniff test) and are **not tracked** as failures by the government or Cyber AB
- One C3PAO: "We want you to pass, but we can't just let you pass" -- the readiness gaps were so severe they could not even accept payment to run the assessment

**The Biggest Hurdle Is Non-Technical:**
- The biggest assessment hurdle is **documentation, not technology** -- companies implement technical controls but fail to document them
- "If it's all in your head, you're probably not going to pass" -- short answer no, long answer also no
- SP 800-171 and 171A are structured with documentation requirements followed by technical configurations; you need both

*(Source: [[What to Know From a C3PAO]], Summit 7, December 2024; [[CMMC Phase 1 - What Comes Next]], Summit 7, November 2025)*

---

### Assessor Disagreements on ESP Scoping

**Issue:** Different C3PAOs may disagree on how to classify and scope ESPs (External Service Providers), particularly when evaluating shared responsibility boundaries.

**Common Friction Points:**
- Whether a hosted enclave provider qualifies as an ESP requiring FedRAMP Moderate compliance
- How to handle CRMAs (Contractor Risk Managed Assets) -- some assessors accept the classification; others challenge it and require assessment against all 110 controls
- Encrypted print job scoping -- whether a FIPS 140 encrypted print path (e.g., Printer Logic) keeps the intermediary network out of scope is still debated by assessors
- Whether on-prem license servers accessed via site-to-site VPN from GCC High are in scope (Summit 7 argues they are not CUI assets and should be out of scope)

**Recommendation:** Ensure your C3PAO and consultant are talking to each other before the assessment -- the time to discover disagreements is not during the assessment itself.

*(Source: [[What to Know From a C3PAO]], Summit 7, December 2024; [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

## Contract Impact Examples

### NAVAIR PALT Analysis -- The Solicitation-to-Award Window (February 2026)

**Data Source:** NAVAIR Long Range Acquisition Forecast (LRAF), published December 2025

**Scope:** 1,676 total contract opportunities; 1,070 with calculable PALT (Procurement Administrative Lead Time) -- both estimated solicitation date and contract award date listed

**Methodology:**
- Best-case scenario counting: solicitations assumed at start of quarter, awards assumed at end of quarter
- Quarters counted inclusively (Q1 to Q2 = two quarters, not one)
- Covers all contract types: repairs, redesigns, prototypes, full life cycle support (C-130s, drones, missiles, helicopters, weapons systems)
- Contract values from $700K to multi-billion

**Findings by Contract Value:**

| Contract Value | Opportunities | Average PALT | Average Months | Assessment |
|---|---|---|---|---|
| Under $2M | 294 | 2.7 quarters | ~8 months | Not realistic for 85% of organizations |
| $2M -- $7.5M | 86 | 3.3 quarters | ~9 months | Still well under a year |
| $7.5M -- $50M | 92 | 3.34 quarters | ~9 months | No improvement despite larger award size |
| $50M -- $100M | 23 | 3.4 quarters | ~9.5 months | Company-defining contracts with minimal time |
| $100M -- $250M | 15 | 5.1 quarters | ~15 months | First comfortable window |
| $250M -- $1B | 11 | 3.8 quarters | ~11.5 months | Drops back down |
| Over $1B | 7 | 5.1 quarters | ~15 months | 15 months for billion-dollar complexity |
| **All (classified + unclassified)** | **1,070** | **3.34 quarters** | **~10 months** | **Less than a year on average** |
| All unclassified | 550 | 3.1 quarters | ~9 months | Classified contracts bump average up slightly |

**Key Observations:**
- **35% of all opportunities** have an award window of 6 months or less
- **30% of solicitations** anticipated in Q2 2026; **32% of contract awards** anticipated in Q2 2026
- Smaller contracts = less time = disproportionate impact on small businesses
- The $100M -- $250M range is the only category where the timeline exceeds 12 months -- and it drops back down for $250M -- $1B
- Internal procurement timelines (budget approvals, vendor selection, kickoffs) consume approximately one quarter before implementation begins
- Even with generous counting methodology, the numbers leave most companies insufficient time to achieve certification from a standing start

**Subcontractor Dimension:**
- All PALT data reflects **prime-to-DoD** award timelines; subcontractors face additional compression as primes impose their own deadlines
- Primes are requiring certification evidence to even view classified solicitations -- subcontractors without certification are locked out at the information stage
- Subcontractors may have no visibility into the PALT window for their specific programs

**Strategic Implication:** PALT analysis demonstrates that waiting for a solicitation to begin CMMC preparation is a losing strategy for the vast majority of NAVAIR contractors. Companies must begin implementation before seeing the requirement or accept that they will be unable to compete for most opportunities.

*(Source: [[No CMMC, No Contract - Why You're Already Too Late for NAVAIR]], Summit 7, February 2026)*

See [[Phase Rollout and Contract Language]] for the full PALT analysis and Phase 1 discretion discussion. See [[Assessment Process and Timeline]] for why 8-10 months is insufficient for most organizations.

## Implementation Case Studies

### Construction Company: 570 CUI Files (Thought Only 20 People Needed Access)

**Company Profile:** Large construction company

**Initial Assumption:** The CIO planned a 20-person enclave based on gut feeling about who needed CUI access.

**Discovery Process:** After running distribution statement searches across their M365 commercial tenant and on-prem file systems, they found **570 files from DoD distribution statements alone** -- and that was only what Microsoft could OCR through PDFs, email, and standard Office attachments. It did not include AutoCAD, SolidWorks, or Revit files.

**Actual CUI Footprint:** Far larger than 20 people -- the data flow analysis revealed that CUI had spread across the organization much more widely than initially believed.

**Key Takeaway:** Without data flow analysis, gut estimates of CUI scope are almost always wrong. The search prevented the painful "second ask" to executives six months later when they would have discovered the enclave needed to be much larger than originally planned.

**Search Methodology Used:**
- CUI banner markings
- DoD clauses
- DoD distribution statements (Parts B through F)

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

---

### University HPC Closet Discovery (Shadow IT in Research Environment)

**Institution Profile:** Top-10 US university

**Discovery:** The university CIO's office received a call after discovering **two high-performance compute on-prem environments** doing highly regulated research that the CIO's office did not know existed.

**Root Cause:** A researcher or grad student had set up the HPC systems in a closet with power supplies -- zero NIST 800-171 controls applied. Research contracts are often awarded directly to the researcher, who then spins up infrastructure (or signs up for AWS commercial with a Gmail account) with zero oversight or controls.

**Shadow IT Dimension:** One large research institute has approximately 200 labs, none managed exactly the same way. Universities are reluctant to confront researchers because they bring research grant money -- finding the balance between enabling research and enforcing compliance is "a lot easier said than done."

**Recommendation:** Do NOT let individual departments spin up their own enclaves -- enclave management must sit under the CIO's office with centralized oversight. The strategy is to roll as much compliance as possible into the cloud and limit physical protection requirements on-prem.

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

---

### Manufacturing Company Buying eBay Scuzzy Drives for Legacy CNC Machines

**Company Profile:** Manufacturing company with legacy laser cutting systems

**Challenge:** CNC machines running Windows XP, Windows 2000, or MS-DOS cannot meet all 110 CMMC controls but still process CUI (technical drawings, manufacturing specifications).

**Workaround:** The company has to buy scuzzy drives off eBay with auto-buy alerts just to keep the laser cutting systems alive. These systems are end-of-life but cannot be replaced without replacing the entire CNC machine -- a capital expenditure often running into hundreds of thousands of dollars.

**CMMC Solution:** CNC machines and similar equipment can be classified as **specialized assets** with a risk-based security approach under the CMMC L2 scoping guidance. Specialized assets (OT, IoT, test equipment, government property, restricted info systems) do **not** require all 110 controls.

**Proactive Recommendation:** Seek DoD CIO exemptions for EOL systems now and have them on file for your assessor. Rev 3 may be "a little bit more heavy-hitting" on specialized asset requirements, so document exemptions early.

**Related Challenge:** Revit releases yearly versions with only 3 years of support, but DoD requires records retention of data created in older versions. The same proactive exemption strategy applies to EOL software required for records retention.

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*
