---
title: Assessment Process and Timeline
aliases:
  - CMMC Assessment
  - Assessment Timeline
  - Certification Process
tags:
  - cmmc
  - assessment
  - timeline
  - certification
confidence: confirmed
last_verified: 2026-02-20
sources:
  - "[[CMMC Assessment Process - What to Expect]]"
  - "[[What to Know From a C3PAO]]"
  - "[[CMMC Phase 1 - What Comes Next]]"
  - "[[Getting CMMC Executive Buy-In with Jeff Smedley]]"
---

## Summary
The CMMC Level 2 assessment is a two-phase process: document review (Phase 1) followed by evidence collection and interviews (Phase 2). Many companies are getting stopped at Phase 1 before they ever reach Phase 2. A mock assessment is strongly recommended before the real thing, as it follows the same format without the risk of a failed record in SPRS.

## Key Facts
- Assessment validity: **3 years**
- Annual requirement in years 2 and 3: self-assessment affirmation in SPRS
- Evidence retention: **6 years** for ALL CMMC assessments (including failed ones)
- Mock assessments do **not** get reported to SPRS -- they are a risk-free dry run
- The C3PAO **cannot consult** during the assessment -- advisory and assessment services must be strictly separated
- A Phase 1 stop gets recorded in the CMMC Assessment Process (CAP)
- A Phase 2 failure is worse than a Phase 1 stop -- it is a documented failure, not a postponement

## How It Works
### Phase 1 -- Document Review
The assessment team reviews your documentation package:
- [[SSP Development|System Security Plan (SSP)]]
- Policies and procedures
- Network diagrams and data flow documentation
- Asset inventory and scoping documentation
- [[CRM (Customer Responsibility Matrix)|CRM]] references and [[ESP (External Service Provider) Classification|ESP]] documentation

> "Lots are getting stopped in Phase 2. Converted to mock or paused." -- Glenda, Lead CCA

Many companies do not make it past Phase 1. If documentation is not ready, the assessment gets postponed or cancelled in the CAP.

A **Phase 1 stop** means:
- The assessment is postponed or cancelled
- This gets recorded in the CAP
- You must fix your documentation before trying again

### Phase 2 -- Evidence and Interviews
If Phase 1 passes, the assessment team moves to:
- Reviewing technical evidence (screenshots, configurations, logs)
- Interviewing key personnel (IT staff, management, users)
- Validating that controls are actually implemented as documented
- Spot-checking systems and configurations

A **Phase 2 failure** means:
- You did not achieve even conditional Level 2 status
- This is a documented failure, not a postponement

### What Assessment Teams Look For
1. **SSP completeness** -- Does every control have a narrative describing how it is implemented?
2. **Evidence alignment** -- Does the evidence match what the SSP claims?
3. **Personnel knowledge** -- Can your people explain what they do and why?
4. **CRM references** -- Are shared responsibilities with your CSP properly documented?
5. **Scoping accuracy** -- Is the assessment boundary correct and well-defined?

### Annual Affirmation
After your C3PAO assessment, you are not done for 3 years. In years 2 and 3 you must:
1. Conduct an annual self-assessment
2. Submit an affirmation in SPRS

### Mock Assessments
A mock assessment:
- Follows the same format as a real assessment
- Identifies gaps before they become failures
- Does **not** get reported to SPRS
- Can be conducted by a C3PAO (but a different team than who will do your real assessment)

## Decision Criteria
- **Ready for assessment?** --> Get a mock assessment first; there is no downside and massive upside
- **Failed Phase 1?** --> Fix documentation before reattempting; the stop is recorded in the CAP
- **Passed Phase 1?** --> Ensure evidence matches SSP narratives and train personnel for interviews
- **Passed certification?** --> Submit annual affirmation in SPRS for years 2 and 3; retain evidence for 6 years

## Common Misconceptions
| Misconception | Reality | Source |
|---|---|---|
| You can wing the assessment if your tech is solid | Many failures come from documentation gaps (SSP, CRM), not technical controls | [[CMMC Assessment Process - What to Expect]] |
| A failed Phase 1 is no big deal | Phase 1 stops are recorded in the CAP and require remediation before retrying | [[CMMC Assessment Process - What to Expect]] |
| Evidence only needs to be kept for the certification period | Evidence must be retained for **6 years** for all CMMC assessments | [[CMMC Assessment Process - What to Expect]] |
| Your assessor can help you fix issues during the assessment | The C3PAO cannot consult during the assessment -- strict separation of concerns | [[CMMC Assessment Process - What to Expect]] |

## Common Reasons for Failure
- SSP is a template with generic language, not tailored to the actual environment
- Evidence does not match SSP narratives
- Personnel cannot explain their own security procedures during interviews
- Scoping is wrong -- assets are missing or misclassified
- [[ESP (External Service Provider) Classification|ESP]]/[[CRM (Customer Responsibility Matrix)|CRM]] documentation is absent or incomplete
- FIPS is "enabled" but not properly validated

### JSVA Program (Joint Surveillance Voluntary Assessment)
- A dual assessment combining DIBCAC/DCMA-driven assessment alongside a C3PAO assessment
- Provides both a **high-confidence on-site SPRS score** and a **C3PAO CMMC Version 2 Level 2 certification** simultaneously
- Described as "bang for the buck" by Jeff Smedley, who used this program
- Available during the early/voluntary assessment period; allowed early adopters to get maximum value from a single assessment effort

*(Source: [[Getting CMMC Executive Buy-In with Jeff Smedley]], Summit 7, July 2025)*

### False Starts (Market Rollout Data)
- During the voluntary market rollout (2025), **25-40% of companies** that signed up for assessments were told to come back later -- they were not ready
- These "false starts" happen in Phase 1 of the assessment (readiness/sniff test) and are **not tracked** as failures by the government or Cyber AB
- Example: companies showing up without an SSP, or signing up thinking the assessment would be conversational rather than evidence-based
- One C3PAO: "We want you to pass, but we can't just let you pass"
- Actual assessment **failure rates remain in single-digit percentages** -- the false start filter keeps the failure rate low

*(Source: [[CMMC Phase 1 - What Comes Next]], Summit 7, November 2025)*

### What C3PAOs Look For (Fernando Machado Perspective)

Fernando Machado (provisional assessor #8, 29th authorized C3PAO) describes what separates successful and unsuccessful assessments:

**Successful Companies Consistently Have:**
- Well-established **policies, procedures, artifacts, and work instructions**
- SSPs documented to the **assessment objective level** (SP 800-171A -- 320 criteria, not just the 110 controls)
- A **document traceability matrix** -- do not dump a pile of documents without explaining how they connect to each other
- A **CRM from their ESPs** clearly delineating shared responsibilities
- Companies achieving perfect 110 scores consistently use **good consultants and ESPs with [[DIBCAC]] experience**

**Common Red Flags C3PAOs Catch:**
- **Templated policies** with brackets like "insert company name here" or university names from downloaded templates
- **Abnormally short SSPs** -- a 12-page SSP will not make it past the gate
- Controls not addressed to the **assessment objective level** (171A, not just 171)
- Non-[[FedRAMP Requirements|FedRAMP Moderate]] cloud providers (e.g., Microsoft 365 Commercial instead of [[GCC High]])
- "Our MSP will handle everything" -- a red flag indicating the OSC does not understand shared responsibility

**"False Starts" (Pre-Assessment Rejections):**
- Fernando's team has turned companies away before assessment for: abnormally short SSPs, controls not at assessment objective level, and non-FedRAMP Moderate cloud providers
- These mirror the broader 25-40% false start rate documented during the voluntary assessment period

**Top 2 Failed Controls:**
1. **FIPS validated cryptography** -- firewalls implemented with the latest firmware but not put into FIPS mode with the correct firmware
2. **Multi-factor authentication (MFA)** -- not a reluctance issue but a **scoping misunderstanding** (MFA applied in one area but not another, especially firewalls); organizations do not realize MFA applies to privileged/non-privileged accounts across network and local access

**The Biggest Hurdle Is Non-Technical:**
- The biggest assessment hurdle is **documentation, not technology** -- companies implement technical controls but fail to document them
- "If it's all in your head, you're probably not going to pass" -- short answer no, long answer also no
- SP 800-171 and 171A are structured with documentation requirements followed by technical configurations; you need both

*(Source: [[What to Know From a C3PAO]], Summit 7, December 2024)*

### Implementation Timeline (Ground Zero to Certified)
- For a 100-person company starting from ground zero (no SSP, no prior compliance work): **12-18 months** is a realistic roadmap
- Technical buildout is only part of the challenge -- **organizational and cultural adoption** is the "long pull in the tent"
- Cost benchmark: **$100,000 per 100 employees** for ground-zero implementation
- Aggressive timelines are possible with the right partners, but cultural buy-in takes time regardless
- Common pitfall: executives think IT can fix this in "a month, couple months" -- this dramatically underestimates the effort

*(Source: [[Getting CMMC Executive Buy-In with Jeff Smedley]], Summit 7, July 2025)*

### NAVAIR PALT Analysis -- Realistic Timeline Assessment

Analysis of 1,070 NAVAIR contract opportunities from the December 2025 Long Range Acquisition Forecast reveals that the average solicitation-to-award window is **far shorter** than most companies' implementation timelines.

**The mismatch:**
- Average PALT across all NAVAIR opportunities: **3.34 quarters (~10 months)**
- Contracts under $2M (294 opportunities): **2.7 quarters (~8 months)**
- Implementation timeline from ground zero: **12-18 months** (per Jeff Smedley's benchmark)
- Result: the typical PALT window is **shorter than the typical implementation timeline**

**Why 8-10 months is not realistic for most organizations:**
- Summit 7's Jason states: "Eight months is not realistic for 85% of the organizations that I've spoken to in the past 90 days"
- The bottleneck is not technology -- it is decisions, budgets, organizational buy-in, and procurement timelines
- Internal procurement to engage a consultant or MSP alone can consume one quarter (~3 months) of the available window
- Project kickoffs, backlogs, and organizational adoption consume additional months
- The net available implementation time after internal overhead is often 5-6 months at best

**35% of opportunities have an award window of 6 months or less** -- making it essentially impossible for organizations starting from scratch to achieve certification in time.

**Contract option years as a surprise trigger:** Many companies are overlooking the fact that existing contracts with option years exercised after 48 CFR goes into effect may require CMMC certification. Unlike new solicitations where a company can choose whether to bid, option year requirements hit existing work where contractors have staff, infrastructure, and revenue at stake. This is described as "the thing that a lot of people are snoozing on."

*(Source: [[No CMMC, No Contract - Why You're Already Too Late for NAVAIR]], Summit 7, February 2026; [[Defense Contractors are Betting Their Companies on THIS Assumption About CMMC Phase 1]], Summit 7, September 2025)*

### The "10-Minute Assessment" Myth

A LinkedIn post celebrating an 11-minute CMMC assessment sparked industry debate. Ryan Bonner (Defcert, 74+ client certifications) debunked this claim:

- **It is physically impossible** to comprehend 320 assessment objectives in 10 minutes -- the human brain cannot process the information that fast
- What likely happened: the organization submitted comprehensive visual evidence of all 320 objectives to the C3PAO **weeks in advance**. The C3PAO reviewed everything pre-assessment, arriving at most conclusions from documented evidence. The "assessment" was only the cleanup of leftover questions.
- Even with perfect pre-submitted evidence, **demonstrations, physical walkthroughs, ESP interviews, and clarification questions** take far more than 10 minutes
- A 10-minute assessment effectively means **no demonstrations were provided** and no physical walkthroughs were counted in the elapsed time
- Promoting such a short assessment timeline is counterproductive -- it calls into question the due diligence and thoroughness of the assessment itself
- **Realistic minimum** even for a well-prepared cloud-native enclave: a full workday (8+ hours), with many assessments spilling into additional days

*(Source: [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]], Summit 7, January 2026)*

## Open Questions / Debates

- **Will false start rates improve as the market matures?** During the voluntary period, 25-40% of companies were not ready. As CMMC becomes required, more unprepared companies will attempt assessments, potentially increasing the false start rate. *(Source: [[CMMC Phase 1 - What Comes Next]], November 2025)*
- **Is 12-18 months realistic for all company sizes?** Jeff Smedley's benchmark is for ~100-person companies. Larger organizations may take longer due to cultural complexity; very small shops may go faster technically but struggle with cultural adoption. *(Source: [[Getting CMMC Executive Buy-In with Jeff Smedley]], July 2025)*
- **Can the PALT window realistically accommodate CMMC preparation?** NAVAIR data suggests 85%+ of organizations cannot achieve certification within the average solicitation-to-award window, especially for contracts under $50M. This raises the question of whether DoD acquisition timelines and CMMC requirements are fundamentally misaligned for most of the DIB. *(Source: [[No CMMC, No Contract - Why You're Already Too Late for NAVAIR]], February 2026)*

## Related Topics
- [[SSP Development]] -- the document that makes or breaks Phase 1
- [[C3PAO Ecosystem and Capacity]] -- the organizations that conduct assessments
- [[Scoping and Assessment Boundaries]] -- getting the assessment boundary right
- [[CRM (Customer Responsibility Matrix)]] -- shared responsibility documentation
- [[ESP (External Service Provider) Classification]] -- ESP documentation requirements
- [[Market Dynamics and Service Needs]] -- cost estimates and executive buy-in strategies
- [[DFARS Clauses and Legal Requirements]] -- DFARS clauses verified through the assessment process

## Sources
- [[CMMC Assessment Process - What to Expect]] -- two-phase process details, mock assessments, C3PAO firewall, timeline/validity, common failure reasons, assessment team priorities
- [[CMMC Phase 1 - What Comes Next]] -- False start data (25-40%), single-digit failure rates, assessment capacity numbers
- [[Getting CMMC Executive Buy-In with Jeff Smedley]] -- JSVA program details, 12-18 month implementation timeline, $100K/100 employees cost benchmark, cultural adoption as long pole
- [[What to Know From a C3PAO]] -- C3PAO assessment perspective (Fernando Machado), top 2 failed controls (FIPS and MFA), false start examples, documentation as biggest hurdle, assessment objective level requirements
- [[No CMMC, No Contract - Why You're Already Too Late for NAVAIR]] -- PALT analysis showing 8-10 month average windows vs. 12-18 month implementation timelines, 85% of organizations cannot achieve certification in typical PALT window, internal procurement overhead consuming available time
- [[Defense Contractors are Betting Their Companies on THIS Assumption About CMMC Phase 1]] -- Contract option years as surprise trigger for CMMC requirements, timing pressure beyond new solicitations
- [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]] -- 10-minute assessment debunked (pre-submitted evidence ≠ fast assessment), minimum realistic timeline even for prepared orgs, 74+ client certifications data point
