---
title: CMMC Levels and Framework Structure
aliases:
  - CMMC Levels
  - CMMC Framework
  - Certification Levels
tags:
  - cmmc
  - framework
  - certification-levels
confidence: confirmed
last_verified: 2026-02-20
sources:
  - "[[When is CMMC Required]]"
  - "[[CMMC Phase 1 - What Comes Next]]"
  - "[[Defense Contractors are Betting Their Companies on THIS Assumption About CMMC Phase 1]]"
  - "[[Where Cybersecurity Meets Legal]]"
---

## Summary
CMMC adds a verification layer on top of the existing NIST 800-171 requirements -- it does not introduce new controls. The framework replaced an older 5-level model with the current 3-level structure, and the vast majority of companies that need Level 2 certification are not yet self-educating or preparing.

## Key Facts
- CMMC is a **verification mechanism**, not a new framework -- it sits on top of DFARS 7012/7019 requirements that already mandate NIST 800-171
- The old CMMC model had 5 levels; the current model has 3 levels (Level 1: FCI self-assessment, Level 2: CUI third-party assessment, Level 3: advanced)
- **The 96% problem**: The most engaged CMMC community (Cooey COE Discord) represents only 2-4% of companies that need Level 2 -- the other 96% are not self-educating
- Companies are still scoring themselves using the outdated 5-level framework (e.g., scoring "88" for Level 1)
- Companies whose MSP told them "we've got you covered" without any real compliance work are part of the massive risk pool
- Companies that think commercial M365 is sufficient for CUI handling represent a common misunderstanding
- **Level 2 conditional status** (with open POA&M items) is a fully valid certification for contract award purposes, as long as items comply with CMMC policy for allowable open items
- As of October 2025, over **450 Level 2 certifications** existed -- all obtained voluntarily before any contract required it
- **Level 3** requires only selected requirements from NIST SP 800-172, not the full publication -- the specific requirements are listed in 32 CFR 170 section 170.14
- Level 3 is assessed by DIBCAC (government assessors), not C3PAOs; you must achieve Level 2 before pursuing Level 3

*(Source: [[CMMC Phase 1 - What Comes Next]], Summit 7, November 2025)*

- **Phase 1 does NOT mean only Level 1** -- Level 2 requirements are appearing in Phase 1 solicitations (e.g., Navy NAVSEA semiconductor RFI, Army Corps of Engineers GBSD Sentinel facilities)
- Risk appetite for requiring higher CMMC levels varies by individual program manager, component, and service branch -- it is not a monolithic DoD decision
- The phased rollout contains no prohibition on Level 2 or Level 2 C3PAO requirements during Phase 1

*(Source: [[CMMC Requirements Are Starting To Show Up]], Summit 7, October 2025)*

## How It Works
### Level 1 -- Federal Contract Information (FCI)
- Self-assessment may apply for contracts that handle FCI but not CUI

### Level 2 -- Controlled Unclassified Information (CUI)
- Requires third-party C3PAO assessment for contracts containing CUI
- Based on NIST SP 800-171 controls
- Certification valid for 3 years with annual affirmation required in years 2 and 3

**CUI Categories Triggering Level 2 Certification (per January 2025 DoD Memo, Attachment 1):**

The January 2025 DoD memo on implementing CMMC identifies five specific CUI categories under the National Archives CUI Registry Defense Organizational Index Grouping that establish Level 2 **certification** (not self-assessment) as the **minimum** assessment requirement:

1. **CTI** -- Controlled Technical Information
2. **DCISI** -- DoD Critical Infrastructure Security Information
3. **NNPI** -- Naval Nuclear Propulsion Information
4. **PSI** -- Privileged Safety Information
5. **UCNID** -- Unclassified Controlled Nuclear Information related to Defense

An estimated **50-60% of all DIB data** likely falls into the CTI category alone. This means a majority of defense contractors handling CUI are potentially subject to the Level 2 certification requirement rather than self-assessment, depending on program manager discretion during Phase 1. Other CUI categories outside this defense grouping may require Level 2 self-assessment rather than full certification.

*(Source: [[Defense Contractors are Betting Their Companies on THIS Assumption About CMMC Phase 1]], Summit 7, September 2025)*

### Level 3 -- Advanced CUI Protection
- Applies to contractors handling the most sensitive CUI (e.g., Golden Dome programs)
- Verifies implementation of selected requirements from NIST SP 800-172 per 32 CFR 170.14
- Assessed by DIBCAC, not C3PAOs
- DIBCAC is already running Level 3 pilots and accepting scheduling requests as of late 2025
- Requires Level 2 certification as a prerequisite

*(Source: [[CMMC Phase 1 - What Comes Next]], Summit 7, November 2025)*

### Relationship to Existing Requirements
CMMC does not replace DFARS 7012 -- it adds a certification requirement on top. Companies already handling CUI are already required to implement NIST 800-171 under DFARS 7012. CMMC (via [[DFARS Clauses and Legal Requirements|DFARS 7021]]) adds the third-party verification that companies actually did what they claimed.

### The "Compliance Is Security" Argument

Mike McGlachlin (cybersecurity attorney, former senior CI adviser for US Cyber Command) pushes back on the common complaint that "compliance is not security":

- **CMMC is a "rising tide lifts all ships" mechanism** -- it is not designed to stop a targeted nation-state attack from China or Russia (which has essentially unlimited resources). It is designed to establish a **baseline** across the entire DIB.
- **"Compliance is absolutely security"** -- "if you're not complying with a specific framework, you are inherently going to be insecure." CMMC is not a panacea but it is categorically better than doing nothing.
- The origin story matters: CMMC traces back to EO 13556 (defining CUI) → NIST 800-171 → DFARS 7012 → the GAO report that said self-attestation was "wholly insufficient because everybody's lying" → CMMC as "a knee-jerk reaction to failure on the part of the DIB to actually secure these covered defense networks"
- **MFA alone eliminates ~90% of attacks**: credential theft/reuse is the primary attack vector. MFA, a basic CMMC control, takes out that entire threat stream.
- **National security mindset**: "When you get into the defense industrial base, you're essentially in a walled garden... your business is national security. You should be focusing on delivering capabilities to war fighters. If that's not the mindset of defense contractors, you should not be in the defense industrial base."

*(Source: [[Where Cybersecurity Meets Legal]], Summit 7, February 2026)*

## Decision Criteria
- **Do you handle CUI?** --> Level 2 certification will be required when DFARS 7021 appears in your contract
- **Do you handle only FCI?** --> Level 1 self-assessment may apply
- **No DoD contracts?** --> CMMC is not required
- See [[Phase Rollout and Contract Language]] for when 7021 is appearing in contracts

## Common Misconceptions
| Misconception | Reality | Source |
|---|---|---|
| CMMC introduces new security controls | CMMC is a verification mechanism -- the controls (NIST 800-171) are already required under DFARS 7012 | [[When is CMMC Required]] |
| Commercial M365 is sufficient for CUI | Commercial M365 does not meet CUI handling requirements -- GCC High or equivalent is needed | [[When is CMMC Required]] |
| "My MSP says we're covered" | Many MSPs claim compliance without doing real compliance work -- this is part of the 96% problem | [[When is CMMC Required]] |
| "Compliance is not security" | Compliance is absolutely security -- without a framework baseline, organizations are inherently insecure. CMMC is not a panacea but it is categorically better than nothing. The "rising tide lifts all ships" argument. | [[Where Cybersecurity Meets Legal]] |
| The old 5-level framework still applies | CMMC was revised to a 3-level model; companies scoring on the old 5-level system are using outdated criteria. Per Discord community: "It's concerning to me how companies are still acknowledging five levels of CMMC." | [[When is CMMC Required]], [[Community Sentiment and Common Frustrations]] |
| Conditional (POA&M) status means you cannot win contracts | Conditional status with allowable open items is a fully valid CMMC Level 2 status for contract award purposes | [[CMMC Phase 1 - What Comes Next]] |
| Level 3 requires all of NIST SP 800-172 | Only selected requirements from SP 800-172 are required, as listed in 32 CFR 170.14 | [[CMMC Phase 1 - What Comes Next]] |

## Open Questions / Debates

- **Level 3 in Phase 1:** Summit 7 predicts Level 3 requirements could appear in Phase 1 contracts despite the phased rollout plan suggesting Phase 2. The Golden Dome memo and political climate may accelerate this. DIBCAC is already running Level 3 pilots. *(Source: [[CMMC Phase 1 - What Comes Next]], November 2025)*
- **Self-assessment vs. certification during Phase 1:** Some DoD components may opt for self-assessment to bend the rules, while others may require full C3PAO certification even in Phase 1. It will be highly situational. *(Source: [[CMMC Phase 1 - What Comes Next]], November 2025)*

## Related Topics
- [[DFARS Clauses and Legal Requirements]] -- the legal foundation CMMC builds on
- [[Phase Rollout and Contract Language]] -- when CMMC requirements appear in contracts
- [[Assessment Process and Timeline]] -- how the Level 2 C3PAO assessment works
- [[FedRAMP Requirements]] -- cloud service requirements for CUI handling
- [[DIBCAC and DCMA Assessments]] -- Level 3 assessed by DIBCAC; Level 2 assessed by C3PAOs
- [[SPRS and Annual Affirmation]] -- SPRS score requirements for Level 2 self-assessment and certification
- [[FIPS 140-2 and 140-3 Compliance]] -- FIPS required for Level 2 CUI protection
- [[Market Dynamics and Service Needs]] -- the 96% DIB readiness gap and market opportunity

## Sources
- [[When is CMMC Required]] -- DFARS clause stack, the 96% problem, framework structure, Level 1 vs Level 2 criteria
- [[Community Sentiment and Common Frustrations]] -- Persistent confusion about 5 levels vs 3 levels even among educated practitioners
- [[CMMC Phase 1 - What Comes Next]] -- Level model refresher, Level 3 details (32 CFR 170.14), conditional vs. final status, Level 2 certification growth numbers
- [[CMMC Requirements Are Starting To Show Up]] -- Level 2 appearing in Phase 1 solicitations, risk appetite varies by PM/component/service
- [[Defense Contractors are Betting Their Companies on THIS Assumption About CMMC Phase 1]] -- CUI categories triggering Level 2 certification (CTI, DCISI, NNPI, PSI, UCNID), January 2025 memo Attachment 1 guidance, 50-60% of DIB data estimated as CTI
- [[Where Cybersecurity Meets Legal]] -- "Compliance is absolutely security" argument, CMMC as rising tide baseline, national security mindset for DIB, CMMC origin story (EO 13556 → NIST 800-171 → DFARS 7012 → GAO report → CMMC), MFA eliminating 90% of attacks
