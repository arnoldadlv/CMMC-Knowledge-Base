---
title: Community Sentiment and Common Frustrations
tags:
  - cmmc
  - community
  - sentiment
  - misconceptions
  - discord-research
source: Cooey COE Discord - Cross-channel sentiment analysis
date: 2026-02-20
---

# Community Sentiment and Common Frustrations

## Key Takeaway

The CMMC practitioner community is frustrated by **vague guidance, ESP scoping chaos, FIPS breakage, and the gap between RMF expectations and CMMC reality**. DIB readiness is alarmingly low, and common misconceptions persist even among experienced practitioners. Understanding these pain points reveals where the market needs the most help.

---

## Top Pain Points

### 1. Vague and Inconsistent Guidance

> "It's concerning to me how companies are still acknowledging five levels of CMMC."

Many companies are still operating on outdated information — using the old 5-level framework, confusing CMMC 1.0 with 2.0, and not understanding which controls actually apply to them. Even within the Discord community (the most educated 2-4% of DIB), basic confusion persists.

### 2. ESP Scoping — The #1 Technical Pain Point

Even **assessors disagree** on how to handle ESP scoping. This is consistently the most debated topic across all channels.

Key frustrations:
- No standardized approach to ESP classification
- No published CRM validation method
- Vendors provide inconsistent (or no) CRMs
- The line between "ESP" and "tool" is blurry and contested

See [[Scoping ESP and CRM Confusion]] for the full breakdown.

### 3. FIPS Mode Breaks Things

Enabling FIPS mode — a hard requirement for CUI protection — causes real-world breakage across common enterprise tools:

| System | FIPS Issue |
|--------|-----------|
| **PLM systems** | Product Lifecycle Management tools often break under FIPS enforcement |
| **VMware Horizon** | VDI environments experience compatibility issues |
| **Intune MDM** | Registry key confusion — FIPS enforcement through MDM policies isn't straightforward |
| **Legacy applications** | Many older apps use non-FIPS cryptographic libraries and break silently |

This isn't a documentation problem — it's a real engineering challenge that requires testing and remediation.

### 4. RMF vs. CMMC Expectations Mismatch

> "Can we please explain to assessors that everything you may have seen working for the DoD or with RMF is NOT expected in CMMC?"

Some assessors come from Risk Management Framework (RMF) backgrounds and apply those expectations to CMMC assessments. The problem: RMF and CMMC have different scopes, different rigor levels, and different baseline assumptions. What's expected in a DoD RMF environment is often overkill or misapplied in a CMMC Level 2 context.

### 5. Low DIB Readiness

The gap between where companies ARE and where they need to BE is enormous:
- Companies scoring themselves at "88" for Level 1 using the **wrong framework**
- Organizations that think buying GCC High = compliance
- MSPs telling clients they're "covered" without doing real compliance work
- The 96% who aren't even self-educating

### 6. Cost and Complexity for SMBs

The cumulative cost of CMMC compliance crushes small businesses:
- PLM system hardening for FIPS
- GCC High migration (licensing + implementation)
- Multiple assessments (mock + real)
- ESP/CRM documentation effort
- Ongoing monitoring and annual affirmation
- Consultant fees for SSP writing and gap analysis

A 30-person machine shop with a $2M DoD contract faces a compliance bill that can easily exceed $100K.

### 7. Mobile Code (3.13.13) — The Most Confusing Control

> "One of the hardest requirements to explain as a consultant and one of the hardest to evaluate as an assessor."

Control 3.13.13 (mobile code) generates more confusion per word than almost any other NIST 800-171 requirement. Consultants struggle to explain it, assessors struggle to evaluate it, and companies have no idea what's expected.

---

## Common Misconceptions — Corrected

These misconceptions appear repeatedly across Discord. Each one has been corrected by credentialed community members:

> [!success] 802.1x Is NOT Required for 3.1.1
> Despite what some consultants and assessors claim, **802.1x network access control is not a requirement** for satisfying control 3.1.1. There are multiple valid approaches to limiting system access.

> [!success] Windows Hello PIN IS MFA
> Windows Hello for Business with PIN sign-in **qualifies as MFA**:
> - **Something you have** — the specific device (TPM-bound credential)
> - **Something you know** — the PIN
>
> This is a legitimate two-factor combination. Assessors who challenge this are wrong.

> [!success] Wireless Can Be N/A If CUI Is FIPS-Encrypted Through VPN
> If all CUI traffic over wireless is **FIPS-encrypted through a VPN**, certain wireless-specific controls can legitimately be marked as Not Applicable. The encryption satisfies the protection requirement regardless of the transport medium.

---

## What This Means for Service Providers

The community frustrations map directly to service opportunities:

| Frustration       | Service Need                                                 |
| ----------------- | ------------------------------------------------------------ |
| Vague guidance    | Expert consulting that translates requirements into action   |
| ESP scoping chaos | Scoping services with ESP classification and CRM acquisition |
| FIPS breakage     | Engineering services for FIPS implementation and testing     |
| Low DIB readiness | End-to-end compliance programs for the 96%                   |
| SMB cost pressure | Right-sized compliance packages, not enterprise overkill     |
| Misconceptions    | Training and education for both OSCs and assessors           |

## The Sentiment Summary

The CMMC community is **cautiously committed but deeply frustrated**. They believe in the mission (protecting CUI) but feel the execution is:
- Underspecified in critical areas (ESP scoping, CRM validation)
- Over-specified in areas that don't matter as much
- Misaligned between what assessors expect and what the rule actually requires
- Financially punishing for the small businesses that make up most of the DIB

The companies that survive this transition will be the ones who start early, get expert help, and don't try to shortcut the process.

## Related Articles

- [[Scoping ESP and CRM Confusion]]
- [[When is CMMC Required]]
- [[When is FedRAMP Required]]
- [[CMMC Assessment Process - What to Expect]]
- [[SPRS and Annual Affirmation Requirements]]
- [[Reassessment and Significant Changes]]
