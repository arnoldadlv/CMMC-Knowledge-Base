---
title: Reassessment and Significant Changes
aliases:
  - Reassessment
  - Significant Changes
  - CMMC Renewal
  - Triennial Assessment
tags:
  - cmmc
  - reassessment
  - significant-changes
  - maintenance
confidence: confirmed
last_verified: 2026-02-20
sources:
  - "[[Reassessment and Significant Changes]]"
---

## Summary
Significant architectural or boundary changes to your assessed environment require a new assessment under 32 CFR 170, but the enforcement mechanism is weak, the definition of "significant" is borrowed from FedRAMP, and there is a practical paradox when migrating tools. Organizations must decide how conservatively to interpret the requirement given that no assessor is actively checking whether reassessment should have been triggered between certification cycles.

## Key Facts
- Per 32 CFR 170, reassessment is required when there are **significant architectural or boundary changes** to the assessed environment
- There is **no CMMC-specific definition** of "significant" -- community guidance is to follow FedRAMP's definitions of "major change"
- Reassessment for significant changes is expected to be **"infrequent and conducted by DoD"** per the final rule
- There is **no enforcement mechanism** for self-reporting significant changes between certification cycles
- Per Cuipacabra (CCP): "There is no assessor who is going to refuse to certify you because you didn't undergo reassessment 2 years ago."
- Tool migration creates a **paradox**: you are temporarily operating outside your assessed scope during any transition
- The safe approach is to treat any change to a Security Protection Asset as potentially significant and document your rationale

## How It Works

### When Reassessment Is Triggered
Per 32 CFR 170, reassessment is required for significant architectural or boundary changes:
- **Network expansions** -- adding new segments, sites, or subnets to the CUI boundary
- **Mergers and acquisitions** -- absorbing another company's environment into your assessed scope
- **Major tool swaps** -- replacing a core security tool (e.g., swapping ThreatLocker for a different EDR)
- **Cloud migration** -- moving from on-prem to cloud, or changing cloud environments
- **Boundary changes** -- expanding or contracting what's in scope for CUI

### What Counts as "Significant" (FedRAMP Definitions)
Since there is no CMMC-specific definition, use FedRAMP's definitions of major change as the best available framework. This includes changes to:
- Security boundary
- Authentication mechanisms
- Encryption methods
- Core infrastructure components

### The Gray Area -- Tool Swaps
Swapping a security tool (e.g., ThreatLocker to another EDR) falls into a gray area. Key questions: Is it "significant" if the replacement serves the same function? What if the new tool is also FedRAMP authorized? What if it is NOT? The safe approach: treat any change to a Security Protection Asset as potentially significant and document your rationale.

### The Enforcement Problem
The practical reality is that reassessment for significant changes is expected to be "infrequent and conducted by DoD" per the final rule. There is no enforcement mechanism for self-reporting significant changes, and no assessor is checking whether you should have triggered a reassessment between certification cycles. This creates a compliance gray zone where organizations must decide how conservatively to interpret the requirement.

### The Migration Paradox
Migrating tools means you are temporarily operating outside your assessed scope. You assessed with Tool A, you are now running Tool B, but you have not been assessed with Tool B yet. This is unavoidable during any tool migration:
1. You are assessed with your current environment (Tool A)
2. You decide to migrate to Tool B
3. During migration, you are running Tool B without it having been part of your assessment
4. After migration, your environment no longer matches what was assessed

**Best practice:** Document the change, assess whether it rises to "significant" using FedRAMP definitions, and if it does, plan for reassessment. If it does not, document your rationale.

## Decision Criteria

### Changes That Likely Require Reassessment
- Adding a new physical site to your CUI boundary
- Merging with another company and integrating their systems
- Migrating from on-prem to cloud (or vice versa)
- Changing your authentication architecture (e.g., switching identity providers)

### Changes That Likely Do NOT Require Reassessment
- Patching or updating existing tools (same product, new version)
- Adding users within the existing boundary
- Routine configuration changes that don't affect the boundary
- Replacing a tool with an equivalent that serves the same function (document this)

### When In Doubt
1. Reference FedRAMP's significant change definitions
2. Document your reasoning
3. Consult with your C3PAO (outside of assessment -- advisory capacity)
4. Err on the side of transparency in your annual affirmation

## Common Misconceptions
| Misconception | Reality | Source |
|---|---|---|
| Any tool change triggers reassessment | Replacing a tool with a functional equivalent likely does not require reassessment -- but document the rationale | [[Reassessment and Significant Changes]] |
| Reassessment is actively enforced between cycles | There is no enforcement mechanism for self-reporting significant changes; no assessor checks for missed reassessments | [[Reassessment and Significant Changes]] |
| You can ignore changes until your next triennial assessment | Per 32 CFR 170, significant changes do require reassessment even mid-cycle -- the lack of enforcement does not eliminate the requirement | [[Reassessment and Significant Changes]] |
| Tool migration is a clean break | During migration you are temporarily operating outside your assessed scope -- this is an unavoidable paradox that must be documented | [[Reassessment and Significant Changes]] |
| One parent CAGE code covers all child CAGE codes | Each CAGE code must be individually tied to the certification in EMAS -- a parent CAGE code does not inherit to children | [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] |
| Switching MSPs is not a significant change | Firing your MSP is an easy justification for significant change -- it fundamentally alters the assessed environment and likely triggers re-certification ($40-70K) | [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] |

### M&A Timing and Significant Change (Legal Perspective)

Don Stern (DLA Piper) emphasizes that M&A activity and CMMC assessments must be coordinated carefully:

- **Push the assessment out 3 months post-acquisition** -- if your IT team is scheduling a CMMC assessment and leadership is contemplating an acquisition, push the assessment past the closing date to allow integration. This avoids the significant change question popping up within months of certification.
- **CMMC is a company problem, not an IT problem** -- business leadership, legal, IT, and management must all be in the same room when planning M&A alongside CMMC. IT may not know that leadership is contemplating an acquisition, and leadership may not realize the CMMC timing implications.
- **Significant change appears unmanageable at scale** -- requiring reassessment for every acquisition seems unmanageable for CyberAB, particularly given current waiting lists for assessments. It remains to be seen how strictly this will be enforced.
- **C3PAO ties cage code in EMAS** -- the C3PAO must tie a cage code to the assessment in the EMAS system. If you acquire a new company with a new cage code, the question becomes: do you wait? What happens to performance on existing contracts? What happens to imminent contract awards during the gap? These questions remain unanswered.

*(Source: [[When CMMC Meets Contracts]], Summit 7, February 2026)*

### Firing Your MSP as a Significant Change

Switching managed service providers after certification is a significant change that likely triggers re-certification:

- Your SPRS/CMMC score is likely tied to controls that your MSP implements on your behalf -- firing the MSP could drop your score from 88 (minimum viable) to a negative number
- **Switching MSPs is an "easy justification"** for significant change under 32 CFR 170 -- the MSP's departure fundamentally alters the assessed environment
- **Re-certification cost: $40,000-$70,000** depending on size and scope
- MSP partnership is a **three-year commitment minimum** aligned to the certification lifecycle
- Plan any MSP transition before your renewal window -- there is a small window to offboard and onboard between certification cycles

*(Source: [[The CUI Hotline - Weekly CMMC Q&A Livestream!]], Summit 7, February 2026)*

### CAGE Code Certification Issue

Each CAGE code must be individually tied to the certification in the EMAS package -- a parent CAGE code does **not** automatically cover child CAGE codes:

- A C3PAO incorrectly told a client that the parent-level CAGE code would "inherit all cage codes below it" -- only the primary CAGE code was listed in EMAS
- When the organization tried to bid a contract under a child CAGE code (an unpopulated joint venture in the same environment), they were told that CAGE code was not CMMC certified
- The organization must now go back to the C3PAO for either a resubmission of the EMAS package or a delta review
- From DoD's perspective, they cannot verify that additional CAGE codes share the same environment -- adding CAGE codes after certification creates assurance gaps
- **Risk of gaming**: Some organizations might try to get one environment certified and then add CAGE codes afterward, which is why DoD requires each CAGE code to be explicitly tied to the assessment

*(Source: [[The CUI Hotline - Weekly CMMC Q&A Livestream!]], Summit 7, February 2026)*

## Open Questions / Debates
- **What exactly counts as "significant"?** No CMMC-specific definition exists. FedRAMP definitions are used as a proxy, but they were designed for a different context. The community debates whether replacing a tool with a functional equivalent (e.g., swapping one FedRAMP-authorized EDR for another) rises to "significant."
- **Will enforcement ever become real?** The final rule says reassessment is "infrequent and conducted by DoD," but the lack of a self-reporting mechanism means the requirement is largely honor-system based. Some practitioners argue this will change as the program matures.
- **Is the significant change definition workable for M&A?** Don Stern describes the current definition as "loosely defined" and the reassessment requirement for acquisitions as seemingly "unmanageable" for CyberAB given current assessment backlogs. The DoD has been issuing FAQ updates, but more clarity on M&A-specific significant change guidance is needed. *(Source: [[When CMMC Meets Contracts]], February 2026)*

## Related Topics
- [[SPRS and Annual Affirmation]] -- Annual affirmation obligations between assessments
- [[Assessment Process and Timeline]] -- The C3PAO assessment process that produces the initial certification
- [[FedRAMP Requirements]] -- FedRAMP's significant change definitions used as a proxy for CMMC
- [[Scoping and Assessment Boundaries]] -- Understanding what's in scope and how boundary changes affect reassessment; boundary changes as primary trigger for reassessment

## Sources
- [[Reassessment and Significant Changes]] -- Trigger definitions, FedRAMP proxy definitions, enforcement weakness, migration paradox, practical guidance on what does/does not require reassessment
- [[When CMMC Meets Contracts]] -- M&A timing advice (push assessment 3 months post-acquisition), significant change seems unmanageable at scale, C3PAO/EMAS/cage code issue, CMMC as company problem not IT problem
- [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] -- Firing MSP as significant change trigger ($40-70K re-certification), CAGE code certification issue (parent does not inherit to children, each must be in EMAS), three-year MSP commitment minimum
