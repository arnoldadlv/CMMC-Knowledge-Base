---
title: Scoping and Assessment Boundaries
aliases:
  - CMMC Scoping
  - Assessment Boundaries
  - CUI Scope
tags:
  - cmmc
  - scoping
  - boundaries
  - assessment
confidence: debated
last_verified: 2026-02-20
sources:
  - "[[Scoping ESP and CRM Confusion]]"
  - "[[Community Sentiment and Common Frustrations]]"
  - "[[CMMC Enclaves by Industry]]"
---

## Summary
Scoping and defining assessment boundaries is the most debated and contentious area of CMMC implementation. ESP scoping is consistently the number one technical pain point in the practitioner community, with even assessors disagreeing on how to handle classification. Getting the boundary right determines cost, complexity, and assessment outcome.

## Key Facts
- ESP scoping is consistently the **#1 technical pain point** in the CMMC practitioner community
- Even **assessors disagree** on how to handle ESP scoping -- there is no standardized approach
- There is **no published CRM validation method** from the CMMC ecosystem
- Vendors provide **inconsistent or no CRMs** (Customer Responsibility Matrices), leaving OSCs to guess
- The line between "ESP" and "tool" is blurry and contested among practitioners and assessors
- ESP scoping chaos is one of the areas where the community feels guidance is most underspecified

## How It Works

### ESP Scoping -- The Core Problem

> "ESP involvement is most complicated aspect of scoping, which is the most complicated thing about CMMC." -- Glenda, Lead CCA ([[Scoping ESP and CRM Confusion]])

ESP (External Service Provider) scoping is the most debated topic across all CMMC community channels. The fundamental issues:

1. **No standardized approach to ESP classification** -- practitioners must make judgment calls about what constitutes an ESP vs. a simple tool
2. **No published CRM validation method** -- even when vendors provide CRMs, there is no official process to verify they are accurate or complete
3. **Vendors provide inconsistent CRMs** -- some vendors provide detailed CRMs, some provide minimal ones, and many provide none at all
4. **The ESP/tool boundary is contested** -- whether a given service is an ESP (requiring scoping and CRM) or just a tool is not clearly defined, and assessors disagree

### Key Asset Classifications
- **CUI Assets** -- systems that process, store, or transmit CUI (always in scope)
- **Security Protection Assets (SPA)** -- assets providing security functions for CUI but not processing CUI themselves
- **Security Protection Data (SPD)** -- data related to the security of CUI assets (e.g., admin credentials, security logs). Admin passwords to your CUI environment are SPD -- if a vendor holds those credentials on their infrastructure, they are handling SPD, which changes their classification. ([[Scoping ESP and CRM Confusion]])
- **Contractor Risk Managed Assets (CRMA)** -- assets that can but do not process CUI. **Use with extreme caution** -- see the CRMA Trap section below
- **Specialized Assets** -- OT, IoT, test equipment, government property, restricted information systems that process CUI but cannot meet all 110 controls. A risk-based security approach is permitted; does not require alignment to all 110 CMMC practices. Critical for manufacturing (CNC machines on Windows XP/2000/MS-DOS) and regulated research (lab equipment). *(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

### The CRMA Trap

> [!warning] CRMAs Are "A Damn Dirty Trap"
> Daniel Acreage (Summit 7) strongly cautions against relying on the CRMA classification. During an assessment, if the assessor looks at your security policies around a CRMA asset and determines the policies are insufficient, they can challenge the CRMA classification and require the asset to be assessed against all 110 CMMC controls. If you classified it as CRMA and did not implement those controls, the asset will fail and you get dinged on your assessment.

**Recommendation**: Stick with CUI assets, SPAs, and Specialized Assets as your primary classifications. Only use CRMA if you are fully prepared to defend the classification and have robust policies demonstrating the asset truly cannot process, store, or transmit CUI. *(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

### How to Approach Scoping
1. **List all external services** that touch your environment
2. **For each service, ask:** Does this provider process, store, or transmit CUI or SPD on their assets?
3. **If yes** --> they are an [[ESP (External Service Provider) Classification|ESP]] --> determine if they are a SPA --> if SPA, get their [[CRM (Customer Responsibility Matrix)|CRM]]
4. **If no** --> it is a tool, not an ESP --> document why in your [[SSP Development|SSP]]
5. **For each CRM received** --> map their responsibilities against your controls --> document gaps that are YOUR responsibility

When in doubt, document your reasoning. Since there is no published CRM validation method, your best defense is documenting why something is or is not an ESP, and how you validated the CRM you received. ([[Scoping ESP and CRM Confusion]])

### Impact on Assessment
Getting ESP scoping wrong has cascading effects:
- Underscoping means controls are not being applied to systems that should be assessed
- Overscoping increases cost and complexity unnecessarily
- Missing CRMs means the assessor cannot validate the shared responsibility model
- Assessor disagreement means the same environment might pass or fail depending on who assesses it

## Decision Criteria
- **Using any external service that processes, stores, or transmits CUI?** --> Likely an ESP requiring scoping and a CRM
- **Vendor provides a CRM?** --> Use it as a starting point, but verify it covers all relevant controls
- **Vendor does NOT provide a CRM?** --> You must create one yourself or push the vendor to provide one -- this is a significant documentation effort
- **Unsure if something is an ESP or a tool?** --> Err on the side of classifying it as an ESP and scoping it in; better to overscope than underscope

## Common Scoping Mistakes

| Mistake | Why It Is Wrong | Source |
|---|---|---|
| Treating all cloud tools as ESPs | Only services that handle SPD/CUI qualify | [[Scoping ESP and CRM Confusion]] |
| Ignoring SPD in vendor environments | Admin creds on vendor infrastructure = SPD | [[Scoping ESP and CRM Confusion]] |
| Not getting a CRM from your ESP | Required for SPA ESPs; assessment will flag this | [[Scoping ESP and CRM Confusion]] |
| Assuming your MSP handles everything | Your MSP may be an ESP -- they need a CRM too | [[Scoping ESP and CRM Confusion]] |
| Scoping too broadly | More assets in scope = more controls to implement = more cost | [[Scoping ESP and CRM Confusion]] |
| Scoping too narrowly | Missing assets means your assessment boundary is wrong | [[Scoping ESP and CRM Confusion]] |
| Classifying assets as CRMA to avoid controls | Assessors can challenge CRMA classification and require full 110-control assessment -- "a damn dirty trap" | [[CMMC Enclaves by Industry]] |
| Ignoring specialized assets | OT, CNC machines, test equipment, and lab systems can be classified as specialized assets with a risk-based approach -- they do not need all 110 controls | [[CMMC Enclaves by Industry]] |

## Common Misconceptions
| Misconception | Reality | Source |
|---|---|---|
| ESP scoping has clear rules | There is no standardized approach; even assessors disagree on classification | [[Community Sentiment and Common Frustrations]] |
| Vendors always provide CRMs | Many vendors provide inconsistent or no CRMs, leaving OSCs to figure it out | [[Community Sentiment and Common Frustrations]] |
| The ESP vs. tool distinction is obvious | The line is blurry and contested -- this is the most debated topic in the community | [[Community Sentiment and Common Frustrations]] |
| All cloud tools are ESPs | Only services that handle SPD or CUI qualify as ESPs | [[Scoping ESP and CRM Confusion]] |
| Only CUI matters for scoping | Admin credentials (SPD) on vendor infrastructure also affect scope | [[Scoping ESP and CRM Confusion]] |

### CUI Flowdown Tension with Subcontractors

CMMC places flowdown responsibility squarely on primes, but this creates significant tension with subcontractors -- particularly small "widget makers" who argue they do not need CUI. The dynamic plays out as follows:

- **Primes are responsible** for ensuring subs that handle CUI are at the appropriate CMMC level
- **Subs push back** -- "All I make is widgets. I don't need CUI. Why do I need Level 2?"
- **The government's position:** "Not my problem" -- the prime must resolve this
- The government often **does not clearly identify what CUI** contractors will receive at the beginning of a contract, making flowdown decisions harder

**Workarounds for indispensable subs that cannot achieve Level 2:**
- Keep the sub at **Level 1** by restructuring what information flows to them
- Share CUI only on the **prime's Level 2 system** -- the sub accesses CUI through the prime's environment rather than their own
- Use **paper documents** instead of electronic transmission (not best practice, but observed in the field)
- Some primes accept subs who are **actively working toward Level 2** and making reasonable progress, with patience for the certification backlog

However, primes are increasingly taking a hard line: "Get Level 2 or we'll find someone else." Raidos told one 50-person subcontractor they would be removed from the supplier list if not certified by October. CMMC is **agnostic of company size** -- it trumps all small business set-asides. See [[DFARS Clauses and Legal Requirements#CMMC Agnostic of Company Size and Set-Asides]] for more detail.

*(Source: [[When CMMC Meets Contracts]], Summit 7, February 2026)*

### Encrypted CUI Remains CUI -- Scoping Implications (DoD FAQ Clarification)

DoD FAQs have clarified that **encrypted CUI remains CUI**, which means encryption alone does **not** create logical separation and does **not** take assets out of scope:

- Any system transmitting, routing, or forwarding encrypted CUI packets is still a **CUI asset**
- Encryption does not prevent a data transfer -- it only obscures the content; the data still moved from asset A to asset B
- **Logical separation requires preventing data transfers entirely**, not just encrypting them
- To achieve out-of-scope status, you must be able to **stop data from moving** from one asset to another

**Practical Example -- VDI + FIPS Printer + VPN Network:**
A virtual desktop sends a FIPS-encrypted print job over a VPN tunnel to a FIPS-validated printer. Under the new interpretation, **all three components are CUI assets** (VDI, network, printer). However, the network transport layer may only need 2-3 NIST 800-171 requirements:
- **3.13.11** (FIPS validated encryption) -- inherited from the VDI that wrapped the packets
- **3.13.10** (key management) -- satisfied by ensuring the network component never has decryption keys
- **3.13.16** (data at rest) -- translates to "don't do packet capture on these encrypted streams"

> [!tip] CUI Asset ≠ 110 Controls
> Ryan Bonner (Defcert): "People immediately hear CUI asset and think 110/320. If you frame it correctly and understand the data flow, it's actually maybe not as painful as you think." The real art is determining how many requirements actually apply to each in-scope component based on its role in the data flow.

**Zero Trust as Emerging Paradigm:**
Zero trust browsers and configured devices that prevent data transfers could mean two computers on the same network have totally different asset determinations based on how they handle whether data can leave and where it can go. The external boundary could shift from the network perimeter to the individual device or even application/file directory level.

*(Source: [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]], Summit 7, January 2026)*

### Security Cameras as CUI Assets

Security cameras become CUI assets when their footage could allow someone to derive knowledge from CUI displayed on screens or documents:

- **The test:** If the camera resolution and angle allow someone to zoom in on recorded footage and read CUI from a screen or document, the footage becomes CUI
- **Rule of thumb:** Do not point a video camera at any area where you would not allow a camera phone -- if you would not let someone hold a phone up to a screen and record, that area should not be in camera range
- **Safe placements:** Perimeter entry/exit points, barriers/passage points, loading docks, key safety areas
- **Risky placements:** Engineer cubicle areas, workstations processing CUI
- **Reference:** Department of the Navy's distinction between "casual access" and "detailed visual access" for export control (NNPI) -- if you have the ability to study and derive knowledge, it is a problem

*(Source: [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]], Summit 7, January 2026)*

## Open Questions / Debates
- **What exactly qualifies as an ESP?** The community has no consensus. Some argue any SaaS tool that touches CUI data flow is an ESP; others argue only services that process or store CUI directly qualify. Assessors split on this.
- **How should CRMs be validated?** No published method exists. Some practitioners argue the OSC must independently verify vendor CRM claims; others accept vendor CRMs at face value. This is a gap in the CMMC ecosystem.
- **How should primes handle indispensable subs who refuse Level 2?** The tension between flowdown requirements and the reality of sole-source widget makers has no clean resolution. Various workarounds exist (keeping subs at L1, using the prime's L2 system, paper documents) but none are ideal. *(Source: [[When CMMC Meets Contracts]], February 2026)*
- **How far does zero trust scoping go?** If zero trust browsers/devices can prevent data transfers at the application level, could two machines on the same network have completely different asset determinations? This paradigm is promising but not yet validated by assessors at scale. *(Source: [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]], January 2026)*

## Related Topics
- [[Enclaves and Architecture Strategies]] -- enclave scoping, asset type classifications, data flow analysis as scoping prerequisite
- [[ESP (External Service Provider) Classification]] -- how to classify external services as ESPs or tools
- [[CRM (Customer Responsibility Matrix)]] -- documenting shared responsibilities with ESPs
- [[SSP Development]] -- the SSP must reflect accurate scoping
- [[FIPS 140-2 and 140-3 Compliance]] -- FIPS requirements apply to all systems within the scoped boundary
- [[Reassessment and Significant Changes]] -- Boundary changes can trigger reassessment
- [[Market Dynamics and Service Needs]] -- ESP scoping chaos is a key service opportunity
- [[Assessment Process and Timeline]] -- Scoping determines what the C3PAO will assess
- [[Export Control and CUI Distinctions]] -- export control access restrictions affecting scoping decisions
- [[GCC High vs Commercial M365]] -- GCC High tenant as the CUI boundary foundation

## Sources
- [[Community Sentiment and Common Frustrations]] -- ESP scoping as #1 pain point, assessor disagreement, lack of CRM validation method, vendor inconsistency, ESP/tool boundary debate
- [[Scoping ESP and CRM Confusion]] -- core scoping problem, Glenda quote, asset classifications, SPD test, common scoping mistakes, how-to approach for ESP scoping
- [[When CMMC Meets Contracts]] -- CUI flowdown tension with widget-maker subs, workarounds (keep at L1, prime's L2 system, paper), primes taking hard line on sub compliance, CMMC agnostic of company size
- [[CMMC Enclaves by Industry]] -- Specialized asset classification (OT, CNC, test equipment), CRMA trap (assessor can upgrade to full 110-control assessment), data flow analysis as scoping prerequisite, supplier enclave boundary complexity
- [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]] -- Encrypted CUI remains CUI (DoD FAQ), logical separation requires preventing data transfers, VDI+printer+network practical scoping example (all three CUI assets but network needs only 2-3 controls), zero trust browser/device paradigm, security cameras as CUI assets (detailed visual access test), CUI asset ≠ 110 controls
