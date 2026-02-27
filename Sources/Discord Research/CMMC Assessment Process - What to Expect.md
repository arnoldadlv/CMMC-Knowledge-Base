---
title: CMMC Assessment Process - What to Expect
tags:
  - cmmc
  - assessment
  - c3pao
  - phase-1
  - phase-2
  - discord-research
source: Cooey COE Discord - #assessments channel, 50+ relevant threads
date: 2026-02-20
---

# CMMC Assessment Process — What to Expect

## Key Takeaway

The CMMC Level 2 assessment is a **two-phase process**: document review (Phase 1) followed by evidence collection and interviews (Phase 2). Many companies are getting stopped at Phase 1 before they ever reach Phase 2. A mock assessment is strongly recommended before the real thing.

---

## The Two Phases

### Phase 1 — Document Review

The assessment team reviews your documentation package:
- System Security Plan (SSP)
- Policies and procedures
- Network diagrams and data flow documentation
- Asset inventory and scoping documentation
- CRM references and ESP documentation

> [!danger] Phase 1 Is Where Many Get Stopped
> "Lots are getting stopped in Phase 2. Converted to mock or paused."
> — Glenda, Lead CCA
>
> Many companies don't even make it past Phase 1. If your documentation isn't ready, the assessment gets postponed or cancelled in the CMMC Assessment Process (CAP).

A **Phase 1 stop** means:
- The assessment is postponed or cancelled
- This gets recorded in the CAP
- You need to fix your documentation before trying again

### Phase 2 — Evidence and Interviews

If Phase 1 passes, the assessment team moves to:
- Reviewing technical evidence (screenshots, configurations, logs)
- Interviewing key personnel (IT staff, management, users)
- Validating that controls are actually implemented as documented
- Spot-checking systems and configurations

A **Phase 2 failure** means:
- You did not achieve even **conditional** Level 2 status
- This is worse than a Phase 1 stop because it's a documented failure, not a postponement

## Mock Assessments — Your Safety Net

> [!tip] Mock Assessments Don't Go Into SPRS
> Mock assessments protect you. They give you the experience of a real assessment without the risk of a failed record in SPRS. Use them.

A mock assessment:
- Follows the same format as a real assessment
- Identifies gaps before they become failures
- Does **not** get reported to SPRS
- Can be conducted by a C3PAO (but a different team than who will do your real assessment)

## The C3PAO Firewall

> [!warning] No Consulting During Assessment
> The C3PAO **cannot consult** during the assessment. This is a strict separation of concerns. If your assessor starts giving advice, that's a red flag. Advisory services and assessment services must be separate.

## Timeline and Validity

| Item | Duration |
|------|----------|
| Assessment validity | **3 years** |
| Annual requirement (years 2 & 3) | Self-assessment affirmation |
| Evidence retention | **6 years** for ALL CMMC assessments |

> [!important] 6-Year Evidence Retention
> Keep your evidence for **6 years**. This applies to all CMMC assessments — not just the ones you pass. If you get audited or there's a dispute, you need that documentation trail.

### Annual Affirmation

After your C3PAO assessment, you're not done for 3 years. In years 2 and 3 you must:
1. Conduct an annual self-assessment
2. Submit an affirmation in SPRS

See [[SPRS and Annual Affirmation Requirements]] for the detailed process.

## What Assessment Teams Look For

Based on Discord discussions from assessors and companies that have been through the process:

1. **SSP completeness** — Does every control have a narrative that describes how it's implemented?
2. **Evidence alignment** — Does the evidence match what the SSP claims?
3. **Personnel knowledge** — Can your people actually explain what they do and why?
4. **CRM references** — Are shared responsibilities with your CSP properly documented?
5. **Scoping accuracy** — Is the assessment boundary correct and well-defined?

## Common Reasons for Failure

- SSP is a template with generic language, not tailored to the actual environment
- Evidence doesn't match SSP narratives
- Personnel can't explain their own security procedures during interviews
- Scoping is wrong — assets are missing or misclassified
- ESP/CRM documentation is absent or incomplete (see [[Scoping ESP and CRM Confusion]])
- FIPS is "enabled" but not properly validated

## Preparing for Success

1. **Get a mock assessment first** — no downside, massive upside
2. **Write your SSP to YOUR environment** — not a template
3. **Train your people** — they'll be interviewed
4. **Collect evidence continuously** — don't scramble the week before
5. **Validate your scoping** — see [[Scoping ESP and CRM Confusion]]
6. **Understand the CRM** — see [[When is FedRAMP Required]]

## Related Articles

- [[SPRS and Annual Affirmation Requirements]]
- [[Scoping ESP and CRM Confusion]]
- [[When is FedRAMP Required]]
- [[When is CMMC Required]]
- [[Reassessment and Significant Changes]]
- [[Community Sentiment and Common Frustrations]]
