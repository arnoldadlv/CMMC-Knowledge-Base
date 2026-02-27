---
title: SPRS and Annual Affirmation
aliases:
  - SPRS
  - SPRS Score
  - Supplier Performance Risk System
  - Annual Affirmation
tags:
  - cmmc
  - sprs
  - affirmation
  - compliance
confidence: confirmed
last_verified: 2026-02-20
sources:
  - "[[SPRS and Annual Affirmation Requirements]]"
  - "[[The End of SPRS Scores (sort of)]]"
  - "[[DOJ vs Small Defense Contractors]]"
---

## Summary
SPRS has three separate tabs for different compliance obligations (800-171, CMMC L2 Self, and CMMC L2 C3PAO), and after a C3PAO assessment you are still required to perform annual self-assessment and affirmation in years 2 and 3. Your CAGE code hierarchy in SAM.gov must be correct before SPRS will work at all, and forgetting annual affirmation causes your certification to lapse.

## Key Facts
- SPRS has **three separate tabs**: 800-171 (for DFARS 7012/7019), CMMC L2 Self (self-assessment results), and CMMC L2 C3PAO (third-party assessment results)
- The 800-171 tab is still required even after a C3PAO assessment -- it must be maintained for DFARS 7012/7019 compliance and cannot be older than **3 years**
- C3PAO certification is valid for 3 years but requires **annual self-assessment and affirmation** in years 2 and 3
- The C3PAO uploads the assessment score, but the **Affirming Official** at your organization must take action to make the certification official
- Your **CAGE code hierarchy in SAM.gov** must be correct before SPRS will associate assessments with your organization
- If your Level 1 environment differs from your Level 2 environment, you must **separately self-assess and affirm Level 1 annually**
- Per Glenda (Lead CCA): "Hint: that's a lot of work, so try to put all your FCI in your L2 environment."

## How It Works

### The Three SPRS Tabs

| Tab | Purpose | Who Maintains It |
|---|---|---|
| **800-171** | NIST 800-171 self-assessment score for DFARS 7012/7019 compliance | The OSC (you) |
| **CMMC L2 Self** | CMMC Level 2 self-assessment results | The OSC (you) |
| **CMMC L2 C3PAO** | CMMC Level 2 C3PAO assessment results | C3PAO uploads; Affirming Official takes action |

### After C3PAO Assessment
1. **C3PAO uploads** your assessment score to the CMMC L2 C3PAO tab
2. **Affirming Official** must take action -- this is a named individual at your organization who certifies the results
3. The Affirming Official's action is what makes the certification official in SPRS

### Annual Affirmation Workflow (Years 1-3)

**Year 1:** C3PAO assessment completed and uploaded to SPRS. Affirming Official takes action.

**Year 2:** Conduct an annual self-assessment of your NIST 800-171 controls. Submit an affirmation in SPRS confirming continued compliance. This is separate from the C3PAO certification.

**Year 3:** Same as Year 2 -- self-assess and affirm again. Begin planning for reassessment if your certification is expiring.

### CAGE Code and SAM.gov Prerequisites
Before submitting anything to SPRS:
1. Verify your CAGE code is active and correct in SAM.gov
2. Confirm the organizational hierarchy (parent/child relationships) is accurate
3. Ensure your Affirming Official has the proper access and roles

## Decision Criteria
- **After C3PAO assessment** --> Affirming Official must take action in SPRS to finalize certification
- **Every year after initial certification** --> Must conduct self-assessment and submit annual affirmation
- **Have separate L1 and L2 environments?** --> Must separately self-assess and affirm Level 1 annually
- **SPRS not working?** --> Check CAGE code hierarchy in SAM.gov first
- **SPRS score older than 3 years on 800-171 tab?** --> Must update; score is expired for DFARS 7012/7019 purposes

## Common Misconceptions
| Misconception | Reality | Source |
|---|---|---|
| C3PAO assessment means you're done for 3 years | You must still perform annual self-assessment and affirmation in years 2 and 3 | [[SPRS and Annual Affirmation Requirements]] |
| Only the C3PAO tab matters after assessment | The 800-171 tab must still be maintained for DFARS 7012/7019 compliance | [[SPRS and Annual Affirmation Requirements]] |
| SPRS will just work once you log in | Your CAGE code hierarchy in SAM.gov must be correct first, or SPRS won't associate your scores properly | [[SPRS and Annual Affirmation Requirements]] |
| L1 FCI is automatically covered by L2 certification | If your L1 environment differs from L2, you need separate annual self-assessment and affirmation for Level 1 | [[SPRS and Annual Affirmation Requirements]] |
| Anyone at the organization can affirm | A designated Affirming Official with proper access and roles must take the action | [[SPRS and Annual Affirmation Requirements]] |
| A false SPRS score is not a big deal if you fix it later | A company submitted 104 when their actual score was -142; even after achieving a perfect 110, they still paid $4.6M in FCA settlement for the years the false score was in place | [[DOJ vs Small Defense Contractors]] |
| You can submit a SPRS score without an SSP | You cannot calculate a valid score without an SSP; DFARS 7019/7020 require it. The FCA case company admitted having no SSP from 2018-2021. | [[DOJ vs Small Defense Contractors]] |
| A low SPRS score under CMMC still gives you some status | Under CMMC, any score below 88 means you have no status at all -- you have failed, unlike old DFARS 7020 where negative scores were acceptable | [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] |

### Senior Official for SPRS/CMMC Affirmation

The senior official who signs the SPRS submission or CMMC affirmation should **not** be the same person who conducted the assessment. Per Don Stern (DLA Piper), the affirmation should come from someone with oversight -- typically at the CISO level, directly below the CISO, or president level (for smaller companies) -- who can provide **one layer of objectivity**. This person should be able to say: "This isn't my baby -- I looked at it objectively, met with the team, and understand what was done and why." This additional layer of objectivity is helpful if compliance questions arise later and is considered good practice, though not a strict legal requirement.

*(Source: [[When CMMC Meets Contracts]], Summit 7, February 2026)*

### SPRS Score and FedRAMP Gap Issue

If an organization meets all 110 NIST 800-171 controls but does **not** meet [[FedRAMP Requirements|FedRAMP]] requirements, there is no straightforward mechanism in SPRS to report that gap. SPRS has no checkbox for FedRAMP compliance status. Options include submitting a score of 109 as a heads-up, adding proposal language disclosing the gap, or documenting the gap internally via POA&M. The key principle: do not bury your head in the sand. See [[DFARS Clauses and Legal Requirements#SPRS Score and FedRAMP Gap Issue]] for full details.

*(Source: [[When CMMC Meets Contracts]], Summit 7, February 2026)*

### Basic Self-Assessment Requirement Removed (February 2026)

As of **February 1, 2026**, the requirement to conduct basic self-assessments and upload scores to SPRS under DFARS 7019/7020 has been **removed** via class deviation. DFARS 7019 was deleted entirely, and DFARS 7020 was renumbered to DFARS 252.204-7997 with all references to basic self-assessments stripped out. The SPRS upload is no longer required for the basic self-assessment -- only **CMMC score uploads** apply when applicable. Medium and high assessments conducted by [[DIBCAC and DCMA Assessments|DIBCAC]] remain unchanged.

This resolves the redundancy between the basic self-assessment (old 7019/7020) and the CMMC Level 2 self-assessment (under 7021). Contractors no longer need to maintain two overlapping assessment scores.

*(Source: [[The End of SPRS Scores (sort of)]], Summit 7, February 2026)*

### Minimum Score Under CMMC -- The 88 Threshold

Under CMMC (DFARS 7021), SPRS scoring rules are significantly stricter than under the old DFARS 7020 basic self-assessment:

- **Minimum viable score: 88** -- this is the threshold for **conditional status** under CMMC
- **Below 88 = no status at all** -- you have not merely received a bad score; you have **failed** your self-assessment and have no CMMC status whatsoever
- Under the old DFARS 7020, organizations could enter **negative scores** (e.g., -150, -200) or scores as low as 12 and still be awarded contracts -- this is no longer viable under CMMC
- **88-109**: Conditional self-assessment status (must close POA&M items within 180 days)
- **110**: Final status (all controls fully implemented)
- Primes will likely begin requiring a minimum score of 88 as well, since anything below that means the subcontractor has no CMMC status and cannot be awarded contracts with DFARS 7021

*(Source: [[The CUI Hotline - Weekly CMMC Q&A Livestream!]], Summit 7, February 2026)*

### Not All Paths to 88 Are Valid

> [!warning] Invalid Scoring Paths to 88
> There are multiple ways to mathematically arrive at an 88 score, but **not all of them are compliant**. Per 32 CFR, specific 5-point and 3-point controls **must** be met -- you cannot simply pick any combination of controls that adds up to 88.

- The DoD Assessment Methodology workbook does **not** include the minimum scoring column -- you must reference 32 CFR and the CAP to understand which controls are mandatory
- Submitting an 88 that was reached through non-compliant control combinations means **misrepresenting your conditional CMMC status** to primes and DoD
- This creates **False Claims Act exposure** -- you are "knowingly" representing your compliance posture when you submit to SPRS
- Subs with SPRS scores below 88 are already being dropped by primes -- GDIT example: a subcontractor with a score below 88 lost work and had millions more on the line with 90 days to get compliant

*(Source: [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]], Summit 7, January 2026)*

### SPRS Score Sharing Strategy

Guidance on when and how to share your SPRS score with external parties:

- **DoD acquisition personnel already have access** to your SPRS score in PIEE -- if they ask you for it, they just want you to do their job for them
- **Proactive sharing in bids**: If you have an 88+ score with all 5-point and 3-point controls met, **leverage it** -- advocate for SPRS score to be a technical evaluation factor on the contract
- **Prime/sub sharing**: Share under NDA; treat your score as a **trade secret** since it represents a competitive advantage
- **Competitors cannot reverse-engineer** which specific controls are met or unmet from the score alone (unless it is -203 or 110)
- Some contractors are **deliberately quiet** about their Level 2 certification -- their strategy is to become a sole supplier while competitors deprioritize compliance

*(Source: [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]], Summit 7, January 2026)*

## Open Questions / Debates
- Whether the annual affirmation process will be rigorously enforced or become a rubber-stamp exercise remains to be seen
- The relationship between the 800-171 tab score and CMMC L2 certification status is a source of ongoing confusion in the community

### False SPRS Score Consequences (FCA Case Study)

A 2025 [[False Claims Act and DOJ Enforcement|FCA settlement]] demonstrated the severe consequences of submitting a false SPRS score:
- Company submitted a score of **104** to SPRS when their actual score was **negative 142**
- A third-party consultant revealed the true score in summer 2022; the company **did not update** until after receiving a DOJ subpoena in 2023
- You **cannot have a valid SPRS score without an SSP** -- the company admitted to having no consolidated SSP from 2018-2021
- The score discrepancy was a central element of the $4.6 million settlement
- Summit 7 commentary: submitting a score to SPRS means you are "knowingly" representing your compliance posture to the government

*(Source: [[DOJ vs Small Defense Contractors]], Summit 7, April 2025)*

## Related Topics
- [[Assessment Process and Timeline]] -- The C3PAO assessment that feeds into SPRS
- [[Reassessment and Significant Changes]] -- When changes trigger the need for a new assessment
- [[DFARS Clauses and Legal Requirements]] -- The DFARS 7012/7019 requirements that drive the 800-171 tab
- [[CMMC Levels and Framework Structure]] -- Understanding L1 vs L2 and their separate obligations
- [[False Claims Act and DOJ Enforcement]] -- FCA consequences of false SPRS scores

## Sources
- [[SPRS and Annual Affirmation Requirements]] -- Three SPRS tabs, annual affirmation workflow, CAGE code prerequisites, common mistakes, Affirming Official process
- [[DOJ vs Small Defense Contractors]] -- False SPRS score consequences (104 vs. -142), FCA settlement case study, no SSP = no valid score
- [[When CMMC Meets Contracts]] -- Senior official guidance (not the person who conducted assessment, one layer of objectivity), SPRS score + FedRAMP gap issue
- [[The End of SPRS Scores (sort of)]] -- Basic self-assessment requirement removed via class deviation (February 2026), SPRS upload no longer required for basic, only CMMC scores
- [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] -- Minimum SPRS score of 88 under CMMC for conditional status, below 88 = no status (failed), negative scores no longer viable, primes likely to require 88 minimum
- [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]] -- Not all paths to 88 are valid (specific 5pt/3pt controls required per 32 CFR), GDIT sub dropped for score below 88, SPRS score sharing strategy (DoD already has access, leverage in bids, share under NDA, treat as trade secret), some contractors quietly leveraging certification as sole supplier strategy
