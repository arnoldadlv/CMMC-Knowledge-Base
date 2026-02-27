---
title: ESP (External Service Provider) Classification
aliases:
  - ESP
  - External Service Provider
  - Service Provider Classification
tags:
  - cmmc
  - esp
  - service-providers
  - scoping
confidence: debated
last_verified: 2026-02-20
sources:
  - "[[Scoping ESP and CRM Confusion]]"
  - "[[When is FedRAMP Required]]"
  - "[[The CUI Hotline - Weekly CMMC Q&A Livestream!]]"
---

## Summary
An ESP (External Service Provider) is an external organization providing a **service** -- not a product -- that processes, stores, or transmits Security Protection Data (SPD) or CUI on their assets. The distinction between an ESP and a tool is one of the most debated topics in CMMC, and the classification directly determines whether you need a [[CRM (Customer Responsibility Matrix)|CRM]] from that vendor.

## Key Facts
- An ESP is a **service**, not a product or tool
- The determining question: **Does the external provider operate assets that handle your SPD or CUI?**
- A product or tool you install and manage yourself is **not** an ESP
- Admin passwords to your CUI environment are **Security Protection Data (SPD)** -- if a vendor holds those credentials on their infrastructure, they are handling SPD
- ESP that is a **Security Protection Asset (SPA)** must produce a CRM
- SPA that is **not** an ESP does not need a CRM
- Summit 7 leads the **MSP Collective**, an initiative attempting to standardize the ESP assessment approach

## How It Works
### The SPD Test
The key test for ESP classification centers on Security Protection Data:

1. **Does this external provider process, store, or transmit CUI on their assets?** --> If yes, they are an ESP
2. **Does this external provider hold admin credentials to your CUI environment on their infrastructure?** --> If yes, those credentials are SPD, and the provider may be an ESP
3. **Do you self-host the tool and no data leaves your boundary?** --> If yes, it is a tool, not an ESP

Admin passwords to your CUI environment are SPD. This is a critical and often-missed point. A vendor that holds your admin credentials on their cloud platform is handling SPD, which can elevate them from "just a tool" to an ESP.

### The NinjaOne/RMM Example
One of the most contentious Discord discussions demonstrates the ESP vs. tool distinction:

**Is a Remote Monitoring and Management (RMM) tool like NinjaOne an ESP, or just a tool?**

- If NinjaOne's **cloud platform holds admin credentials** to your CUI environment --> those are SPD --> NinjaOne may be an ESP
- If you **self-host the RMM** and no data leaves your boundary --> it is a tool, not an ESP

The classification depends entirely on where the data (including credentials) resides and who operates the infrastructure.

### ESP Classification Flow
1. List all external services touching your environment
2. For each, apply the SPD test
3. If classified as ESP --> determine if it is a SPA
4. If ESP + SPA --> require a CRM from the vendor
5. If not an ESP --> document the reasoning in your [[SSP Development|SSP]]

## Decision Criteria
- **Vendor's cloud platform holds your admin creds** --> Likely an ESP; apply the full SPD test
- **You self-host the tool entirely** --> Likely a tool, not an ESP; document reasoning in SSP
- **Vendor processes CUI on their infrastructure** --> Definitely an ESP; get a CRM
- **Vendor provides a security service (SPA) as an ESP** --> CRM is required
- **Unsure** --> Document your reasoning for the classification; there is no published CRM validation method yet

## Common Misconceptions
| Misconception | Reality | Source |
|---|---|---|
| All cloud tools are ESPs | Only services that handle SPD or CUI on the vendor's assets qualify | [[Scoping ESP and CRM Confusion]] |
| A product you manage is an ESP | A product/tool you install and manage yourself is not an ESP -- the provider must operate assets handling your SPD/CUI | [[Scoping ESP and CRM Confusion]] |
| RMM tools are always ESPs | Depends on deployment: cloud-hosted with your admin creds = likely ESP; self-hosted = tool | [[Scoping ESP and CRM Confusion]] |
| Only CUI matters for ESP classification | Admin credentials (SPD) on vendor infrastructure also trigger ESP classification | [[Scoping ESP and CRM Confusion]] |
| Your MSP is just a vendor, not an ESP | If your MSP holds admin creds or touches CUI/SPD on their infrastructure, they are an ESP and need a CRM | [[Scoping ESP and CRM Confusion]] |
| ESPs need their own Level 2 certification | ESPs are not subcontractors and do not need their own certification -- but they show up to your assessment and are judged as part of your boundary | [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] |
| DFARS 7012 flows down to ESPs | ESPs are extensions of your support team, not contract executors -- no DFARS 7012 flowdown, but independent ESP requirements apply | [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] |

### ESP Flowdown and Certification Status

ESPs are **not subcontractors** on defense contracts and therefore do **not** have DFARS 7012 flowdown requirements in the traditional sense:

- An ESP is an **extension of your support team**, not an entity executing the contract -- they do not need their own Level 2 certification
- There is **no certification requirement** for ESPs/MSPs under the current CMMC final rule (32 CFR 170)
- However, ESPs **do show up to your assessment** -- the C3PAO judges the ESP's controls as part of your certification boundary, not separately
- If your ESP/MSP **fails** their portion of the assessment, **you fail** -- they are judged as one certification boundary with you

**DoD originally wanted ESP certification.** The proposed rule for 32 CFR 170 included a requirement for ESPs to achieve their own certification. DoD backed down from this position to accommodate industry concerns, but Summit 7 anticipates this will eventually return: "Anything that they wanted they'll probably end up getting in the long run."

**Some MSPs are voluntarily getting certified** -- either because they are defense contractors themselves or because they want to differentiate in the market. This is a good question to ask when vetting an MSP: do they walk the walk, or are they just "pinky promising" everything will be okay?

*(Source: [[The CUI Hotline - Weekly CMMC Q&A Livestream!]], Summit 7, February 2026)*

### MSP Vetting as Critical Risk Management

Selecting the wrong MSP is one of the highest-risk decisions a company can make in the CMMC journey:

- **MSPs without an SRM** cannot demonstrate what they are responsible for during an assessment -- an MSP employee on Reddit was discovered asking who is responsible for talking to the assessor, revealing the MSP had no SRM and had lost their only CCP
- **"Trunk slammers"** -- the MSP industry term for providers who pad their portfolio with as many clients as possible without specializing in regulated defense work
- **MSPs forcing clients to pay out remainder of contract terms** before switching to a CMMC-capable MSP -- if CMMC is not built into the contract, the client may be trapped
- **Firing your MSP triggers significant change** -- if you have already been certified, switching MSPs likely triggers re-certification ($40,000-$70,000 depending on size and scope)
- MSP partnership is a **three-year commitment minimum** aligned to the certification lifecycle -- make the decision carefully and plan any transition before your renewal window

*(Source: [[The CUI Hotline - Weekly CMMC Q&A Livestream!]], Summit 7, February 2026)*

### MSSP CRM Synthesis -- Who Is Responsible for What?

When an MSSP deploys and manages a security stack (e.g., CrowdStrike) on your behalf, the CRM responsibility chain works as follows:

- **The MSSP should synthesize** all underlying tool CRMs into a single CRM for the end client -- you should not have to hunt down CRMs from every tool in their stack
- **Watch for pass-through services**: Know whether the MSSP staffs their own SOC or outsources to the tool vendor's managed service (e.g., CrowdStrike Falcon Complete). There must be a **direct line of responsibility** to how requirements are met
- **Assessment day test**: Ensure someone in the room can intelligently explain how the security stack works end-to-end. If no one can speak to "how the sausage gets made," you have a problem
- **FedRAMP question remains**: CRMs do not show whether underlying tools meet FedRAMP Moderate or equivalent -- this requires separate due diligence with your MSSP
- **If your MSSP cannot synthesize this for you**, they are probably not the right partner -- you should not have to reverse-engineer their tool usage

*(Source: [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]], Summit 7, January 2026)*

## Open Questions / Debates
The ESP vs. tool line remains one of the most contentious areas in CMMC. Even assessors disagree on specific cases. The NinjaOne/RMM question exemplifies this: reasonable practitioners can arrive at different conclusions depending on how they interpret "processing SPD on their assets."

Summit 7's **MSP Collective** is attempting to standardize the ESP assessment approach, but the effort is still evolving. Until there is clearer guidance or a published validation method, companies must document their reasoning and be prepared to defend their classification decisions during assessment.

## Related Topics
- [[Scoping and Assessment Boundaries]] -- ESP classification is the hardest part of scoping
- [[CRM (Customer Responsibility Matrix)]] -- required from ESPs that are SPAs
- [[SSP Development]] -- ESP documentation and classification reasoning must be in the SSP
- [[FedRAMP Requirements]] -- FedRAMP applies when cloud ESPs handle CUI

## Sources
- [[Scoping ESP and CRM Confusion]] -- ESP definition, ESP vs. tool debate, the SPD test, NinjaOne/RMM example, MSP Collective initiative
- [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] -- ESPs not subcontractors (no flowdown, no own cert required), DoD originally wanted ESP certification (backed down), MSPs voluntarily certifying, MSP vetting risks (trunk slammers, no SRM, Reddit horror story), firing MSP triggers significant change ($40-70K re-certification), three-year commitment minimum
- [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]] -- MSSP CRM synthesis responsibility (MSSP should consolidate all tool CRMs), pass-through service awareness (SOC staffing vs outsourced MDR), assessment day readiness (someone must explain the stack), FedRAMP not on CRMs
