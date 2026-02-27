---
title: When is FedRAMP Required
tags:
  - cmmc
  - fedramp
  - cui
  - scoping
  - discord-research
source: Cooey COE Discord - 482 matches across FedRAMP discussions
date: 2026-02-20
---

# When is FedRAMP Required

## Key Takeaway

FedRAMP authorization is required when a cloud service **processes, stores, or transmits CUI**. If the service never touches CUI, FedRAMP is not required — even if the tool is part of your security stack.

---

## The Rule

A cloud service provider (CSP) needs FedRAMP authorization when it handles CUI on behalf of a federal agency or a contractor subject to DFARS 7012. The determining factor is whether CUI flows through, resides in, or is processed by that cloud environment.

> [!important] The CUI Test
> Ask one question: **Does this cloud service process, store, or transmit CUI?**
> - **Yes** → FedRAMP required
> - **No** → FedRAMP not required

## MFA Solutions — A Common Point of Confusion

One of the most frequently asked questions on Discord is whether MFA providers like Okta need to be FedRAMP authorized.

The community consensus, confirmed by multiple credentialed practitioners:

- **MFA solutions that never touch CUI do NOT require FedRAMP** (CyberNorris + Liatris confirmed)
- The cryptographic operations in MFA are verifying **authenticity** (proving who you are), not protecting **CUI confidentiality**
- This is a fundamentally different requirement than encrypting CUI at rest or in transit

> [!tip] Key Distinction
> Crypto for **authentication** ≠ crypto for **CUI protection**. MFA validates identity — it doesn't handle controlled data.

## Security Tools That Don't Handle CUI

Security tools in your environment (SIEM agents, vulnerability scanners, EDR) that **do not process, store, or transmit CUI** do not need FedRAMP versions. However, if a security tool ingests logs that contain CUI or has access to CUI-bearing systems in a way that exposes the data, the calculus changes.

This is a scoping question — see [[Scoping ESP and CRM Confusion]] for how to determine what's in and out.

## GCC High and the FedRAMP CRM

If your organization is on **GCC High**, you need the FedRAMP Customer Responsibility Matrix (CRM) from Microsoft to write your SSP. This is non-negotiable for assessment.

> [!warning] Don't Skip the CRM
> Without the CRM, you cannot properly document shared responsibilities in your SSP. Many companies get stopped at Phase 1 of their assessment because their SSP doesn't adequately address CRM references. See [[CMMC Assessment Process - What to Expect]] for what happens when Phase 1 documentation is insufficient.

For guidance on obtaining and using the CRM, see [[Scoping ESP and CRM Confusion]].

## What the Community Expects from DoD

There remains ambiguity in some edge cases. The general community expectation:

> "If and when DoD provides an answer it's very safe to believe they'll follow suit with FedRAMP."
> — Uncouth, CCP

The safe bet is to align with FedRAMP requirements now rather than wait for explicit DoD guidance that may take months or years to materialize.

## Common Mistakes

| Mistake                                   | Reality                                                      |
| ----------------------------------------- | ------------------------------------------------------------ |
| "All our cloud tools need FedRAMP"        | Only tools that handle CUI                                   |
| "Okta needs to be FedRAMP authorized"     | Not if it never touches CUI                                  |
| "We can skip FedRAMP because we're small" | Size doesn't matter — CUI handling does                      |
| "Our antivirus needs FedRAMP"             | Only if it processes/stores CUI (unlikely for most AV tools) |
| "We're on GCC High so we're covered"      | You still need the CRM to properly document your SSP         |

## Related Articles

- [[Scoping ESP and CRM Confusion]]
- [[CMMC Assessment Process - What to Expect]]
- [[When is CMMC Required]]
- [[SPRS and Annual Affirmation Requirements]]
- [[Community Sentiment and Common Frustrations]]
