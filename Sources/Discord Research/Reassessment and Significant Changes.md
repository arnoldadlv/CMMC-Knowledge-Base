---
title: Reassessment and Significant Changes
tags:
  - cmmc
  - reassessment
  - significant-change
  - fedramp
  - discord-research
source: Cooey COE Discord - Reassessment trigger discussions
date: 2026-02-20
---

# Reassessment and Significant Changes

## Key Takeaway

Significant architectural or boundary changes to your assessed environment require a new assessment under 32 CFR 170 — but the enforcement mechanism is weak, the definition of "significant" is borrowed from FedRAMP, and there's a practical paradox when migrating tools.

---

## When Reassessment Is Triggered

Per 32 CFR 170, reassessment is required when there are **significant architectural or boundary changes** to the assessed environment.

### Examples of Triggering Changes

- **Network expansions** — adding new segments, sites, or subnets to the CUI boundary
- **Mergers and acquisitions** — absorbing another company's environment into your assessed scope
- **Major tool swaps** — replacing a core security tool (e.g., swapping ThreatLocker for a different EDR)
- **Cloud migration** — moving from on-prem to cloud, or changing cloud environments
- **Boundary changes** — expanding or contracting what's in scope for CUI

## What Counts as "Significant"?

There's no CMMC-specific definition yet. The community guidance is to **follow FedRAMP's definitions of "major change"**:

> [!tip] Use FedRAMP as Your Guide
> When determining if a change is "significant," FedRAMP's definitions of major change are the best available framework. This includes changes to:
> - Security boundary
> - Authentication mechanisms
> - Encryption methods
> - Core infrastructure components

### The Gray Area — Tool Swaps

Swapping a security tool (e.g., ThreatLocker → another EDR) falls into a gray area:
- Is it a "significant" change if the replacement tool serves the same function?
- What if the new tool is also FedRAMP authorized?
- What if it's NOT FedRAMP authorized?

The safe approach: treat any change to a Security Protection Asset as potentially significant and document your rationale for why reassessment is or isn't needed.

## The Enforcement Problem

> [!warning] Weak Enforcement
> "There is no assessor who is going to refuse to certify you because you didn't undergo reassessment 2 years ago."
> — Cuipacabra, CCP

The practical reality:
- Reassessment for significant changes is expected to be **"infrequent and conducted by DoD"** per the final rule
- There is **no enforcement mechanism** for self-reporting significant changes
- No assessor is checking whether you should have triggered a reassessment between certification cycles

This creates a compliance gray zone where organizations must decide how conservatively to interpret the requirement.

## The Migration Paradox

> [!question] The Paradox
> Migrating tools means you're **temporarily operating outside your assessed scope**. You assessed with Tool A, you're now running Tool B — but you haven't been assessed with Tool B yet.

This is an unavoidable reality of any tool migration:

1. You're assessed with your current environment (Tool A)
2. You decide to migrate to Tool B
3. During migration, you're running Tool B without it having been part of your assessment
4. After migration, your environment no longer matches what was assessed

**Best practice:** Document the change, assess whether it rises to "significant" using FedRAMP definitions, and if it does, plan for reassessment. If it doesn't, document your rationale.

## Practical Guidance

### Changes That Likely Require Reassessment

- Adding a new physical site to your CUI boundary
- Merging with another company and integrating their systems
- Migrating from on-prem to cloud (or vice versa)
- Changing your authentication architecture (e.g., switching identity providers)

### Changes That Likely Don't Require Reassessment

- Patching or updating existing tools (same product, new version)
- Adding users within the existing boundary
- Routine configuration changes that don't affect the boundary
- Replacing a tool with an equivalent that serves the same function (document this)

### When In Doubt

1. Reference FedRAMP's significant change definitions
2. Document your reasoning
3. Consult with your C3PAO (outside of assessment — advisory capacity)
4. Err on the side of transparency in your annual affirmation

## Related Articles

- [[CMMC Assessment Process - What to Expect]]
- [[SPRS and Annual Affirmation Requirements]]
- [[When is FedRAMP Required]]
- [[Scoping ESP and CRM Confusion]]
- [[Community Sentiment and Common Frustrations]]
