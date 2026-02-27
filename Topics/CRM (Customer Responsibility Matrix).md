---
title: CRM (Customer Responsibility Matrix)
aliases:
  - CRM
  - Customer Responsibility Matrix
  - Shared Responsibility
tags:
  - cmmc
  - crm
  - shared-responsibility
  - service-providers
confidence: debated
last_verified: 2026-02-20
sources:
  - "[[Scoping ESP and CRM Confusion]]"
  - "[[When is FedRAMP Required]]"
---

## Summary
A Customer Responsibility Matrix (CRM) documents the shared responsibility between you and your [[ESP (External Service Provider) Classification|ESP]]. It clarifies what security controls the ESP implements, what remains your responsibility, and how the handoff points work. Getting CRMs from vendors is inconsistent -- "the wild wild west" -- with no published validation method yet.

## Key Facts
- A CRM is required from any ESP that is classified as a **Security Protection Asset (SPA)**
- A SPA that is **not** an ESP does not need a CRM
- There is **no published method for validating a CRM yet**
- CRM references in your [[SSP Development|SSP]] are one of the things assessment teams specifically look for
- Without a CRM, you cannot properly document shared responsibilities in your SSP
- Many companies get stopped at [[Assessment Process and Timeline|Phase 1]] because their SSP does not adequately address CRM references
- If your organization is on **GCC High**, you need the FedRAMP CRM from Microsoft to write your SSP -- this is non-negotiable for assessment

## How It Works
### What a CRM Contains
A CRM documents for each relevant security control:
- What the ESP implements on their side
- What security controls remain YOUR responsibility
- How the handoff points work between the ESP's environment and yours

### The CRM Rule
- ESP that is a **SPA** --> must produce a CRM
- SPA that is **not** an ESP --> does not need a CRM

### Getting CRMs from Vendors
The current state of CRM availability is inconsistent. Real-world experiences from practitioners:

| Vendor | CRM Experience |
|---|---|
| Microsoft (GCC High) | Available via FedRAMP package -- must request it |
| Arctic Wolf | Assessors had trouble getting them to show up for interviews |
| Large SaaS vendors | Some provide CRMs proactively, others require escalation |
| Small/niche vendors | Often do not know what a CRM is |

### GCC High FedRAMP CRM
If your organization uses GCC High, the Microsoft FedRAMP CRM is essential:
- It is available through the FedRAMP package but must be specifically requested
- Without it, you cannot properly document shared responsibilities in your SSP
- Many companies get stopped at Phase 1 of assessment because CRM references are missing or inadequate

### Using a CRM
Once you have a CRM from your ESP:
1. Map the ESP's responsibilities against your NIST 800-171 controls
2. Identify gaps that remain YOUR responsibility
3. Document both the ESP's coverage and your remaining obligations in your SSP
4. Retain the CRM as evidence for your assessment

### MSP Collective
Summit 7 leads the **MSP Collective**, an initiative to standardize the ESP assessment approach and bring consistency to how MSPs and ESPs are evaluated. This is still evolving but aims to address the current inconsistency in CRM availability and validation.

## Decision Criteria
- **Your ESP is a SPA** --> You need a CRM from them
- **Your SPA is not an ESP** --> No CRM needed
- **Vendor will not provide a CRM** --> Escalate; document your attempts; this may affect your assessment
- **Vendor does not know what a CRM is** --> Common with small/niche vendors; you may need to educate them or find an alternative
- **Using GCC High** --> Request the FedRAMP CRM from Microsoft; it is required for your SSP

## Common Misconceptions
| Misconception | Reality | Source |
|---|---|---|
| CRMs are optional nice-to-haves | CRM references are specifically checked during assessment; missing CRMs can stop you at Phase 1 | [[CMMC Assessment Process - What to Expect]] |
| All vendors readily provide CRMs | It is "the wild wild west" -- some vendors provide them easily, others refuse or do not know what they are | [[Scoping ESP and CRM Confusion]] |
| Being on GCC High means you are fully covered | You still need the CRM to properly document shared responsibilities in your SSP | [[When is FedRAMP Required]] |
| Every external service needs a CRM | Only ESPs that are SPAs need to produce a CRM | [[Scoping ESP and CRM Confusion]] |

## Open Questions / Debates
There is **no published method for validating a CRM yet**. This means:
- Companies must take vendor-provided CRMs at face value or do their own due diligence
- Assessment teams have no standardized way to verify CRM accuracy
- The MSP Collective (led by Summit 7) is working to bring consistency, but the approach is still evolving
- Your best defense is documenting your reasoning for how you validated the CRM you received

## Related Topics
- [[ESP (External Service Provider) Classification]] -- ESPs that are SPAs must produce CRMs
- [[SSP Development]] -- CRM references must be included in the SSP
- [[Scoping and Assessment Boundaries]] -- CRMs are part of the scoping process
- [[Assessment Process and Timeline]] -- CRM completeness is checked during assessment
- [[FedRAMP Requirements]] -- GCC High FedRAMP CRM requirement

## Sources
- [[Scoping ESP and CRM Confusion]] -- CRM definition, CRM requirements for SPA ESPs, vendor CRM experiences, MSP Collective, CRM validation gap
- [[When is FedRAMP Required]] -- GCC High FedRAMP CRM requirement, CRM needed for SSP documentation
