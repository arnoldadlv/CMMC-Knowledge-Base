---
title: SSP Development
aliases:
  - SSP
  - System Security Plan
  - Security Plan
tags:
  - cmmc
  - ssp
  - documentation
  - assessment
confidence: confirmed
last_verified: 2026-02-20
sources:
  - "[[CMMC Assessment Process - What to Expect]]"
  - "[[Scoping ESP and CRM Confusion]]"
  - "[[What to Know From a C3PAO]]"
  - "[[Where Cybersecurity Meets Legal]]"
---

## Summary
The System Security Plan (SSP) is the single most critical document in CMMC assessment -- it is the first thing reviewed in Phase 1 and the primary reason companies get stopped before reaching Phase 2. Every control must have a narrative describing how it is implemented in YOUR specific environment, not generic template language.

## Key Facts
- SSP completeness is the **#1 thing assessment teams look for** -- every control needs a narrative describing how it is implemented
- A template SSP with generic language is one of the **most common reasons for failure**
- Evidence must **align with SSP narratives** -- if your SSP claims something, you need evidence proving it
- SSP must include [[CRM (Customer Responsibility Matrix)|CRM]] references documenting shared responsibilities with your CSP
- SSP must address [[Scoping and Assessment Boundaries|scoping]] -- the assessment boundary must be correct and well-defined
- Without the CRM from your ESP (e.g., Microsoft GCC High FedRAMP CRM), you cannot properly document shared responsibilities in your SSP

## How It Works
### What Makes a Good SSP
A good SSP is written to YOUR environment, not copied from a template. For each NIST 800-171 control, the SSP must describe:
1. **How** the control is implemented in your specific environment
2. **Who** is responsible for the control (your team vs. your ESP via the CRM)
3. **What evidence** supports the implementation claim
4. **Where** the control applies within your assessment boundary

### Common SSP Failures
Based on assessor and practitioner discussions:
- SSP is a **template with generic language** not tailored to the actual environment
- **Evidence does not match** SSP narratives -- what you claim and what you can prove diverge
- **CRM references are absent or incomplete** -- shared responsibilities with ESPs are not documented
- **Scoping errors** in the SSP -- assets are missing or misclassified in the assessment boundary
- [[ESP (External Service Provider) Classification|ESP]] documentation is missing from the SSP
- **Not even an SSP at all** -- real story: a company delivered a **20-slide PowerPoint deck** to their C3PAO assessor and said "this is my SSP." The assessor had to send them away, adding months of delay to find help and get back in line for a new assessment date. *(Source: [[Where Cybersecurity Meets Legal]], Summit 7, February 2026)*

### SSP and the Assessment
The SSP is reviewed in [[Assessment Process and Timeline|Phase 1]] of the assessment. If the SSP is inadequate:
- The assessment may be stopped at Phase 1
- This gets recorded in the CMMC Assessment Process (CAP)
- You must fix the SSP before attempting again

In Phase 2, the assessment team validates that controls are actually implemented as the SSP documents them -- through evidence review, interviews, and spot-checks.

## Decision Criteria
- **Writing your SSP** --> Write it to your environment, not from a template; include CRM references and scoping documentation
- **Preparing for assessment** --> Verify every SSP narrative has matching evidence; train personnel to explain what the SSP describes
- **Using an ESP (e.g., GCC High)** --> Get the CRM and map shared responsibilities into your SSP control narratives
- **Unsure about scoping** --> Get scoping right first, then write the SSP -- the SSP must reflect an accurate assessment boundary

## Common Misconceptions
| Misconception | Reality | Source |
|---|---|---|
| A purchased SSP template is sufficient | Templates with generic language are one of the top failure reasons -- the SSP must be tailored to your environment | [[CMMC Assessment Process - What to Expect]] |
| The SSP only matters for Phase 2 | The SSP is reviewed in Phase 1; many companies get stopped before ever reaching Phase 2 | [[CMMC Assessment Process - What to Expect]] |
| You can skip CRM documentation in the SSP | CRM references are one of the things assessment teams specifically look for | [[CMMC Assessment Process - What to Expect]] |

### C3PAO Assessment Perspective on SSPs (Fernando Machado)

Fernando Machado (provisional assessor #8, 29th authorized C3PAO) describes what his assessment team looks for in SSPs and the most common failures:

- SSPs should be documented to the **assessment objective level** -- this means SP 800-171A with its **320 criteria**, not just the 110 controls in SP 800-171
- A **12-page SSP will not pass** -- abnormally short SSPs are a reason C3PAOs turn companies away before the assessment even begins
- Simply copy-pasting the control text from 171 is **not acceptable** -- the SSP must describe how each control is implemented in YOUR environment
- A **document traceability matrix** is recommended -- do not dump a pile of documents without explaining how they relate to each other and to the controls
- **Templated SSPs** are caught immediately -- brackets with "insert company name here" or university names from downloaded templates are dead giveaways that the SSP has not been tailored
- Companies that consistently achieve perfect 110 scores have SSPs prepared by consultants and ESPs with [[DIBCAC]] experience

*(Source: [[What to Know From a C3PAO]], Summit 7, December 2024)*

### DIBCAC SSP Requirements
[[DIBCAC and DCMA Assessments|DIBCAC]] has specific and heightened SSP expectations that go beyond typical CMMC assessment preparation:
- DIBCAC **specifically rejects** SSPs that simply copy and paste NIST SP 800-171 requirement verbiage -- this is explicitly called out as unacceptable in their pre-assessment checklist
- SSPs must address requirements at the **NIST SP 800-171A assessment objective level**, not just the 171 requirement text -- DIBCAC explicitly cites 171A as "the primary and authoritative source of guidance for organizations conducting such assessments"
- Brief, minimal SSPs (e.g., 12-page SSPs) are not going to pass a DIBCAC audit -- the level of detail required to address 171A objectives for all 110 requirements is substantial
- SSPs must cover **all systems** relevant to the assessment, with all supporting CAGE codes listed

*(Source: [[DIBCAC Assessment Requirements]], Summit 7, November 2025)*

## Open Questions / Debates
<!-- Where experts disagree - both sides documented with attribution -->

## Related Topics
- [[Assessment Process and Timeline]] -- SSP is the centerpiece of Phase 1 document review
- [[CRM (Customer Responsibility Matrix)]] -- CRM must be referenced in SSP for shared responsibilities
- [[Scoping and Assessment Boundaries]] -- SSP must reflect the correct assessment boundary
- [[ESP (External Service Provider) Classification]] -- ESP documentation feeds into the SSP
- [[FedRAMP Requirements]] -- GCC High CRM from FedRAMP package needed for SSP

## Sources
- [[CMMC Assessment Process - What to Expect]] -- SSP completeness as assessment criteria, common SSP failures, Phase 1 documentation review
- [[Scoping ESP and CRM Confusion]] -- CRM and ESP documentation requirements for SSP
- [[What to Know From a C3PAO]] -- SSP assessment objective level requirement (171A/320 criteria), 12-page SSP failure, template detection, document traceability matrix recommendation
- [[DIBCAC Assessment Requirements]] -- DIBCAC rejects copy/paste SSPs, requires 171A assessment objective level detail, cites 171A as authoritative source
- [[Where Cybersecurity Meets Legal]] -- 20-slide PowerPoint SSP real story, SSP readiness as root cause of assessment suspensions
