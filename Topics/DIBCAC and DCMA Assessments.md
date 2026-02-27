---
title: DIBCAC and DCMA Assessments
aliases:
  - DIBCAC
  - DCMA
  - Defense Industrial Base Cybersecurity Assessment Center
  - Government Assessments
tags:
  - cmmc
  - dibcac
  - dcma
  - assessment
confidence: confirmed
last_verified: 2026-02-20
sources:
  - "[[DIBCAC Assessment Requirements]]"
---

## Summary
DIBCAC (Defense Industrial Base Cybersecurity Assessment Center), part of DCMA (Defense Contract Management Agency), conducts in-person audits of defense contractors' compliance with [[DFARS Clauses and Legal Requirements|DFARS 252.204-7012]] -- completely separate from the CMMC assessment process. Since October 2025, at least half a dozen contractors have received official audit notices. Many of these companies assumed they would only need CMMC Level 1 self-assessment, but DIBCAC assesses full NIST 800-171 compliance plus all other paragraphs of DFARS 7012 including flowdown, incident reporting, and cloud computing requirements.

*(Source: [[DIBCAC Assessment Requirements]], Summit 7, November 2025)*

## Key Facts
- [[DFARS Clauses and Legal Requirements|DFARS 252.204-7020]] has been in contracts since **2020**, giving DoD the right to audit contractor cybersecurity compliance at any time
- DIBCAC is part of DCMA (Defense Contract Management Agency) -- these are **government auditors**, not third-party C3PAOs
- At least **half a dozen** contractors received DIBCAC audit notices since October 2025
- DIBCAC provides **90 calendar days notice** (including holidays) before the in-person audit begins
- **2 weeks** to acknowledge receipt of the notice
- **5 weeks** prior to assessment: pre-coordination phone call
- **2 weeks** prior to assessment: all artifacts due (submitted via DoD Safe)
- **1 week** prior to assessment: DIBCAC verifies receipt of documents
- Assessment runs **Monday through Friday, 8:00 AM to 4:30 PM** for a full week
- Results provided within **60 days** after the end of assessment
- DIBCAC works very closely with the **Department of Justice (DOJ)** -- per DODIG reports and DIBCAC's own statements
- DIBCAC is not gracious with granting timeline extensions -- their resources and time are very limited
- DIBCAC audits cover **all of DFARS 7012**, not just NIST 800-171 -- this includes flowdown to subcontractors, incident reporting, cloud computing, and damage assessment
- You can have a **perfect 110 SPRS score** and still have massive DIBCAC violations because of non-compliance with other 7012 paragraphs

*(Source: [[DIBCAC Assessment Requirements]], Summit 7, November 2025)*

## How It Works

### The DIBCAC Audit Notice
When DIBCAC decides to audit you, they send an email that starts a 90-calendar-day clock. The email includes a pre-assessment item checklist outlining everything they want to see. You have two weeks to acknowledge receipt.

### Pre-Assessment Checklist
DIBCAC's pre-assessment checklist requires the following:

**1. Re-run your self-assessment and upload a new SPRS score**
- Conduct a new self-assessment per the DoD Assessment Methodology
- Upload the updated score into [[SPRS and Annual Affirmation|SPRS]]
- If there is a significant disparity between your old and new scores, that will raise red flags -- especially since DIBCAC will be there in weeks to verify your work

**2. System Security Plans (SSPs)**
- Provide SSPs for **all systems** relevant to the assessment
- SSPs must include a description of how each of the **110 security requirements** is implemented
- Simply copying and pasting the requirement verbiage from NIST SP 800-171 is **not acceptable**
- DIBCAC explicitly states that **NIST SP 800-171A** is "the primary and authoritative source of guidance for organizations conducting such assessments" -- SSPs must address 171A assessment objective level, not just the 171 requirement text
- All CAGE codes supported by each SSP must be listed
- Any open POA&M items must be provided

**3. Network topology diagram and enterprise overview briefing**
The diagram/briefing must clearly delineate:
- Security boundaries
- Cybersecurity stack
- SIEM (Security Event and Information Management) system
- Connections to other systems and networks
- Cloud connections and data flow
- Wireless systems
- Dedicated point-to-point connections
- MLS clouds
- High-level IP address schema
- Critical network services
- Vulnerability scanning methodology
- Authentication methodology
- Enterprise logging methodology
- Remote access methods
- Web browsing and web content filtering
- DNS, VoIP, video systems
- Any other relevant information for assessors to determine CUI protection posture

**4. Flowdown demonstration**
- Demonstrate how the organization manages contractual flowdown of [[DFARS Clauses and Legal Requirements|DFARS 7012]] to subcontractors
- DIBCAC will use a **sample of contracts** to verify that enterprise policies, procedures, and requirements flow down to the contract level
- You can have a perfect 110 score and still have massive violations if you have not flowed 7012 down to follow the flow of CUI to subcontractors

**5. Verify compliance with other 7012 paragraphs**
- Cloud computing requirements (FedRAMP Moderate equivalency)
- Cyber incident reporting
- Cyber incident damage assessment activities

**6. List of Subject Matter Experts (SMEs)**
DIBCAC wants to interview SMEs for each security family in NIST SP 800-171, including:
- Network administrator and security engineer
- Personnel with audit and accountability responsibilities
- Cybersecurity and IT policy oversight team
- Account management personnel
- Personnel with information security responsibilities
- System developers
- Personnel with access enforcement responsibilities
- Risk assessment team
- Incident response team
- Senior Information Security Officer (SISO)
- HR personnel adjacent to security functions
- Physical security specialist/manager
- Configuration management team
- Enterprise services lead
- Active Directory administrator

### How DIBCAC Differs from CMMC
| Aspect | CMMC Assessment | DIBCAC Audit |
|---|---|---|
| **Scope** | NIST SP 800-171 implementation only | All of DFARS 7012 -- 800-171 plus flowdown, incident reporting, cloud computing, damage assessment |
| **Conducted by** | C3PAO (third-party) | DIBCAC (government, part of DCMA) |
| **Terminology** | "Assessment" | "Audit" |
| **Relationship** | You are the customer of the C3PAO | DIBCAC is your customer's enforcement arm -- no leverage |
| **Extensions** | Negotiable with C3PAO | DIBCAC is not gracious with extensions |
| **Flowdown** | Not in scope | Explicitly in scope -- will sample contracts |
| **DOJ coordination** | Not directly | DIBCAC works closely with DOJ |

You can have a perfect CMMC Level 2 certification (all 110 controls met) and still fail a DIBCAC audit because CMMC only covers one paragraph of DFARS 7012 (the NIST 800-171 paragraph), while DIBCAC covers the entire clause.

*(Source: [[DIBCAC Assessment Requirements]], Summit 7, November 2025)*

## Decision Criteria
- **You have DFARS 7020 in your contracts** --> DIBCAC can audit you at any time with 90 days notice
- **You handle CUI under DFARS 7012** --> You are subject to DIBCAC audits regardless of your CMMC status or level
- **You have a CMMC Level 2 C3PAO certification** --> DIBCAC may be **less interested** in auditing you, as the C3PAO cert provides some assurance. Having the cert may deter DIBCAC from targeting you.
- **You only planned for CMMC Level 1** --> Double-check your math. If you have DFARS 7012 in your contracts, you have full 800-171 obligations that DIBCAC can audit regardless of your CMMC level expectations.
- **Your MSP "handles" your compliance** --> If your MSP is not prepared to sit at the table for 5 days answering DIBCAC questions and does not have a service level agreement covering this, that is your problem -- not theirs.

## Common Misconceptions
| Misconception | Reality | Source |
|---|---|---|
| "I only need CMMC Level 1" | If DFARS 7012 is in your contracts and you handle CUI, you have full 800-171 obligations that DIBCAC can audit regardless of your CMMC level | [[DIBCAC Assessment Requirements]] |
| "CMMC covers everything DIBCAC would look at" | CMMC only assesses 800-171. DIBCAC audits all of DFARS 7012 including flowdown, incident reporting, cloud computing, and damage assessment. You can have a perfect 110 and still have massive DIBCAC violations. | [[DIBCAC Assessment Requirements]] |
| "DIBCAC won't come knocking" | At least half a dozen contractors received audit notices since October 2025. DFARS 7020 has been in contracts since 2020. | [[DIBCAC Assessment Requirements]] |
| "My MSP handles this" | If your MSP cannot sit at a table for 5 days answering DIBCAC questions with no extension, that is your problem. Do you have a service level agreement that covers this? | [[DIBCAC Assessment Requirements]] |
| "I have time to prepare" | You get 90 calendar days including holidays. The pre-coordination call is at 5 weeks out. That leaves roughly 35 days from notification to having everything in order. | [[DIBCAC Assessment Requirements]] |

## Open Questions / Debates
- **Will DIBCAC audit frequency increase?** The flurry of notices since October 2025 may signal increased enforcement activity, but DIBCAC has limited auditor capacity -- which is why the CMMC third-party system exists. *(Source: [[DIBCAC Assessment Requirements]], November 2025)*
- **Does a C3PAO certification guarantee DIBCAC will not audit you?** Summit 7 reports hearing that DIBCAC is less interested in companies with C3PAO certifications, but this is not a guarantee -- it may only reduce priority. *(Source: [[DIBCAC Assessment Requirements]], November 2025)*

## Related Topics
- [[DFARS Clauses and Legal Requirements]] -- DFARS 7012 and 7020 are the legal basis for DIBCAC audits
- [[CMMC Levels and Framework Structure]] -- CMMC vs. DIBCAC scope
- [[SSP Development]] -- SSP requirements for DIBCAC are more stringent (must address 171A objectives)
- [[SPRS and Annual Affirmation]] -- DIBCAC requires a fresh self-assessment and SPRS upload
- [[False Claims Act and DOJ Enforcement]] -- DIBCAC works closely with DOJ
- [[Assessment Process and Timeline]] -- CMMC assessment process for comparison

## Sources
- [[DIBCAC Assessment Requirements]] -- Full DIBCAC audit process, pre-assessment checklist, timeline, SME requirements, scope differences from CMMC, flowdown requirements, consequences, DOJ coordination
