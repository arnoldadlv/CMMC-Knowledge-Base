---
title: Scoping ESP and CRM Confusion
tags:
  - cmmc
  - scoping
  - esp
  - crm
  - msp
  - discord-research
source: Cooey COE Discord - ESP/CRM/scoping discussions across multiple channels
date: 2026-02-20
---

# Scoping, ESP, and CRM Confusion

## Key Takeaway

ESP scoping is the **single most complicated aspect of CMMC** — even assessors disagree on how to handle it. The distinction between an ESP (a service) and a product/tool is critical, and getting the Customer Responsibility Matrix (CRM) from your vendors is inconsistent at best.

---

## The Core Problem

> "ESP involvement is most complicated aspect of scoping, which is the most complicated thing about CMMC."
> — Glenda, Lead CCA

This isn't hyperbole. Scoping determines your entire assessment boundary — what's in, what's out, who's responsible for what. Get scoping wrong and everything downstream (SSP, evidence, controls implementation) is built on a bad foundation.

## Key Definitions

### ESP — External Service Provider

An ESP is a **service**, not a product. The distinction matters:

- ESP = an external organization providing a **service** that processes, stores, or transmits Security Protection Data (SPD) or CUI
- A product or tool you install and manage yourself is **not** an ESP
- The question is: **does the external provider operate assets that handle your SPD or CUI?**

### CRM — Customer Responsibility Matrix

A CRM documents the **shared responsibility** between you and your ESP. It clarifies:
- What security controls the ESP implements on their side
- What security controls remain YOUR responsibility
- How the handoff points work

### SPA — Security Protection Asset

Assets that provide security functions for CUI but don't process CUI themselves.

## The ESP vs. Tool Debate

One of the most contentious Discord discussions revolves around where the line is between an ESP and a tool:

> [!question] The NinjaOne/RMM Question
> Is a Remote Monitoring and Management (RMM) tool like NinjaOne an ESP, or just a tool?
>
> The key question: **Do they process, store, or transmit SPD on their assets?**
>
> - If NinjaOne's cloud platform holds admin credentials to your CUI environment → those are SPD (Security Protection Data) → they may be an ESP
> - If you self-host the RMM and no data leaves your boundary → it's a tool, not an ESP

### The SPD Test

> [!important] Admin Passwords = SPD
> Admin passwords to your CUI environment are **Security Protection Data**. If a vendor holds those credentials on their infrastructure, they're handling SPD — which changes their classification.

## The CRM Problem

### ESPs That Are SPA Must Produce a CRM

The rule:
- ESP that is a **Security Protection Asset (SPA)** → must produce a CRM
- SPA that is **not** an ESP → does not need a CRM

### Getting CRMs Is Inconsistent

> [!warning] The Wild West
> "It is the wild wild west out there" when it comes to CRM validation.
>
> There is **no published method for validating a CRM yet**. Some vendors provide them easily, others refuse or don't know what you're talking about.

Real-world CRM experiences from Discord:

| Vendor | CRM Experience |
|--------|---------------|
| Microsoft (GCC High) | Available via FedRAMP package — must request it |
| Arctic Wolf | Assessors had trouble getting them to show up for interviews |
| Large SaaS vendors | Some provide CRMs proactively, others require escalation |
| Small/niche vendors | Often don't know what a CRM is |

### The MSP Collective

Summit 7 leads the **MSP Collective**, an initiative attempting to standardize the ESP assessment approach. This is an effort to bring consistency to how MSPs and ESPs are evaluated, but it's still evolving.

## Common Scoping Mistakes

| Mistake | Why It's Wrong |
|---------|---------------|
| Treating all cloud tools as ESPs | Only services that handle SPD/CUI qualify |
| Ignoring SPD in vendor environments | Admin creds on vendor infrastructure = SPD |
| Not getting a CRM from your ESP | Required for SPA ESPs; assessment will flag this |
| Assuming your MSP handles everything | Your MSP may be an ESP — they need a CRM too |
| Scoping too broadly | More assets in scope = more controls to implement = more cost |
| Scoping too narrowly | Missing assets means your assessment boundary is wrong |

## How to Approach ESP Scoping

1. **List all external services** that touch your environment
2. **For each service, ask:** Does this provider process, store, or transmit CUI or SPD on their assets?
3. **If yes** → they're an ESP → determine if they're a SPA → if SPA, get their CRM
4. **If no** → it's a tool, not an ESP → document why in your SSP
5. **For each CRM received** → map their responsibilities against your controls → document gaps that are YOUR responsibility

> [!tip] When In Doubt, Document Your Reasoning
> Since there's no published CRM validation method, your best defense is documenting your reasoning for why something is or isn't an ESP, and how you validated the CRM you received.

## Related Articles

- [[When is FedRAMP Required]]
- [[CMMC Assessment Process - What to Expect]]
- [[SPRS and Annual Affirmation Requirements]]
- [[Community Sentiment and Common Frustrations]]
- [[Reassessment and Significant Changes]]
