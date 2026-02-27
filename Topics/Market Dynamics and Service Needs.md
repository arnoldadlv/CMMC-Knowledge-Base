---
title: Market Dynamics and Service Needs
aliases:
  - CMMC Market
  - Service Provider Market
  - MSP Opportunities
tags:
  - cmmc
  - market
  - business
  - service-providers
confidence: consensus
last_verified: 2026-02-20
sources:
  - "[[Community Sentiment and Common Frustrations]]"
  - "[[Getting CMMC Executive Buy-In with Jeff Smedley]]"
  - "[[Where Cybersecurity Meets Legal]]"
---

## Summary
Community frustrations map directly to service opportunities in the CMMC market. DIB readiness is alarmingly low, with approximately 96% of defense industrial base companies not even self-educating on requirements. SMBs face cumulative compliance costs that can easily exceed $100K, and the gap between where companies are and where they need to be creates enormous demand for right-sized compliance services.

## Key Facts
- **The 96% problem**: The most engaged CMMC community (Cooey COE Discord) represents only 2-4% of companies that need Level 2 -- the other 96% are not even self-educating on requirements
- A **30-person machine shop** with a $2M DoD contract faces compliance costs that can easily **exceed $100K**
- **Rule of thumb: $100,000 per 100 employees** for ground-zero implementation (Jeff Smedley's benchmark -- no SSP, no prior compliance work)
- Much of the implementation cost is **one-time** -- CMMC maintenance costs less than the initial buildout; one-time costs can be structured as add-backs that do not affect EBITDA
- Compliance costs are supposed to be rolled into the contractor's bid rate as an **allowable cost** -- the government views this as already paying for it
- **No subsidies, no appropriations, no cost offsets** expected during Phase 1; no NDAA funding for DIB cybersecurity compliance exists
- Companies without CMMC certification trying to sell will "get pennies for the dollar to private equity" -- valuation drops by the minute
- Key SMB cost drivers: PLM system hardening for FIPS, GCC High migration (licensing + implementation), multiple assessments (mock + real), ESP/CRM documentation, ongoing monitoring and annual affirmation, consultant fees for SSP writing and gap analysis
- The CMMC community is **cautiously committed but deeply frustrated** -- they believe in the mission but feel the execution is underspecified, misaligned, and financially punishing
- Companies scoring themselves at "88" for Level 1 using the **wrong framework** represent the massive knowledge gap
- Organizations that think buying GCC High equals compliance are a common failure pattern
- MSPs telling clients they are "covered" without doing real compliance work is widespread

## How It Works

### Community Frustrations Map to Service Opportunities

| Frustration | Service Need |
|---|---|
| Vague guidance | Expert consulting that translates requirements into action |
| ESP scoping chaos | Scoping services with ESP classification and CRM acquisition |
| FIPS breakage | Engineering services for FIPS implementation and testing |
| Low DIB readiness | End-to-end compliance programs for the 96% |
| SMB cost pressure | Right-sized compliance packages, not enterprise overkill |
| Misconceptions | Training and education for both OSCs and assessors |

### Enclave Demand Across Verticals

Enclave demand is growing rapidly across three major industry verticals, each with unique requirements:

- **Manufacturing**: The traditional DoD contractor vertical. Requires GPU-backed VDI for engineering applications, specialized asset handling for OT/CNC equipment, and USB staging workflows for print-to-shop-floor
- **AEC (Architecture, Engineering, Construction)**: A surprising growth area -- five years ago Summit 7 would not have predicted AEC as one of their largest client verticals. Construction companies are building infrastructure at DoD sites (e.g., Guam), dredging at naval ports, and suddenly discovering CUI requirements. One construction company found 570 files from DoD distribution statement searches alone
- **Regulated Research (Universities)**: An emerging and complex market. Research institutions face unique challenges including non-US person segmentation, researcher autonomy (grad students spinning up AWS accounts with Gmail), chargeback per grant/contract, and oversight challenges (top-10 university discovered two unknown HPC environments in a closet). The CIO's office must own the enclave, not individual departments

Each vertical drives demand for enclave architecture services, data flow analysis, GCC High migration, and ongoing managed services.

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

### The DIB Readiness Gap
The gap between where companies ARE and where they need to BE is enormous:
- Companies scoring themselves at "88" for Level 1 using the wrong framework entirely
- Organizations that think buying GCC High = compliance
- MSPs telling clients they are "covered" without doing real compliance work
- The 96% who are not even self-educating on what CMMC requires

### MSP Vetting as Critical Service Need

MSP vetting has emerged as one of the most important -- and most overlooked -- steps in the CMMC journey. The market is full of "**trunk slammers**" -- MSPs padding their portfolios without specializing in regulated defense work:

- **The SRM is non-negotiable**: An MSP without a Shared Responsibility Matrix cannot demonstrate what controls they own during assessment. A Reddit thread exposed an MSP employee who did not know who was responsible for talking to the assessor -- the MSP had no SRM and their only CCP had left.
- **MSPs forcing contract buyouts**: Many MSPs are forcing clients to pay out the remainder of contract terms before switching to a CMMC-capable provider -- if CMMC deliverables are not built into the MSP contract, the client may be trapped.
- **Firing an MSP triggers significant change**: If already certified, switching MSPs likely requires re-certification at $40,000-$70,000. This makes MSP selection a **three-year commitment minimum**.
- **"Less about money, more about time"**: The market shift is accelerating -- conversations are less about price and more about timeline pressure from primes and the government. A higher education research facility told Summit 7: "It is less about money and way more about time because we can't have PIs leaving our university."
- **Every vertical is affected**: Construction, manufacturing, SaaS providers, higher education -- demand is hitting across all industries, not just traditional defense manufacturing.

**GCC High tenant count as a DIB readiness litmus test**: The number of GCC High tenants that exist is a "great litmus test" for how many organizations are actually compliant or pursuing compliance. DoD could ask Microsoft at any time how many regulated tenants exist -- if that number is a tiny fraction of companies with DFARS 7012 obligations, DIB readiness is clearly insufficient.

*(Source: [[The CUI Hotline - Weekly CMMC Q&A Livestream!]], Summit 7, February 2026)*

### MSP Certification Gap -- No Certifying Authority

Mike McGlachlin (cybersecurity attorney, Buchanan Ingersoll & Rooney) identifies a structural gap in the MSP ecosystem: **there is no certifying body for MSPs** in the CMMC space.

- There is no equivalent of Underwriters Laboratory (UL), American Bar Association, or other professional certification that validates MSP quality
- "Billy the IT guy from down the street is just as good as Microsoft in the eyes of any sort of certifying authority because it just doesn't exist"
- Anyone can start an MSP tomorrow and offer CMMC compliance services with no qualification requirements
- This makes MSP vetting a critical but unstructured task for DIB companies
- The bottleneck is not just C3PAO capacity -- **MSP onboarding capacity** is an equally significant bottleneck, with MSPs unable to bring companies to a compliance state fast enough for certification scheduling
- C3PAOs are suspending assessments because companies cannot produce an SSP -- the real bottleneck is happening at the MSP/readiness level before companies ever reach the C3PAO

*(Source: [[Where Cybersecurity Meets Legal]], Summit 7, February 2026)*

### SMB Cost Pressure
The cumulative cost of CMMC compliance crushes small businesses. A typical compliance bill includes:
- PLM system hardening for FIPS
- GCC High migration (licensing + implementation)
- Multiple assessments (mock + real)
- ESP/CRM documentation effort
- Ongoing monitoring and annual affirmation
- Consultant fees for SSP writing and gap analysis

A 30-person machine shop with a $2M DoD contract faces a compliance bill that can easily exceed $100K -- a punishing ratio of compliance cost to contract value.

### Assessment and Implementation Cost Reality

Ryan Bonner (Defcert) provides critical context on the true cost picture that many DIB companies are only now realizing:

- **Assessment cost is the smaller number** -- the much larger cost is implementing NIST 800-171 itself. The FAR CUI rule's cost analysis easily hit $1M+ for implementation (and worse for cloud)
- **DIB IT spend is historically 1% of revenue** -- compared to 7-8% in healthcare, finance, and insurance. Manufacturing and construction are among the lowest IT spenders as a percentage of revenue
- **The DIB is now the most heavily regulated industry on the planet** -- organizations need a strategy to recompose their entire cost structure around these new requirements, not just a strategy to pay for the assessment
- **CMMC raised awareness of a burden that existed since 2017** -- the whiplash comes from getting hit with years of deferred compliance costs all at once in a compressed timeline, plus an expedite fee to jump the queue
- **Projected IT spend increase**: From 1-2% historically to potentially 5-8% of revenue depending on scope
- **No DoD funding exists** -- the proposed $1.5T DoD budget contains zero funding for businesses to achieve CMMC; no tax breaks materialized despite lobbying efforts
- **Set-asides do not trump CMMC** -- hub zones, minority-owned, veteran-owned, disabled-owned businesses are not exempt; CMMC requirements come before set-aside status when vetting contractors
- **"Compliant in 60 days" demand is surging** -- multiple organizations are desperate for immediate compliance because their primes could call any day asking for status; this drives expedite fees and higher costs

*(Source: [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]], Summit 7, January 2026)*

### The Sentiment Summary
The CMMC community is cautiously committed but deeply frustrated. They believe in the mission (protecting CUI) but feel the execution is:
- **Underspecified** in critical areas (ESP scoping, CRM validation)
- **Over-specified** in areas that do not matter as much
- **Misaligned** between what assessors expect and what the rule actually requires
- **Financially punishing** for the small businesses that make up most of the DIB

The companies that survive this transition will be the ones who start early, get expert help, and do not try to shortcut the process.

### Early Adopter Behavior and MSP Role (Fernando Machado, C3PAO Perspective)

Fernando Machado's assessment backlog and industry observations confirm several market dynamics:

**Early Adopters -- Public Skepticism, Private Urgency:**
- At conferences and events, companies would publicly cast doubt on CMMC: "We don't think it's going to happen, we don't think it's real"
- Those same companies would privately approach afterward asking: "When can we get in line?"
- **"In public they were casting doubt, in private being like we want to be first out of the gate"** -- the certification race was happening behind closed doors while public sentiment remained skeptical

**MSP Role as Force Multiplier:**
- MSPs are described as "force multipliers" for assessments -- a well-prepared MSP with a clear [[CRM (Customer Responsibility Matrix)|CRM]] dramatically streamlines the assessment process
- A certified MSP does not need to present staff at the assessment table, reducing both time and cost for the contractor
- However, MSPs claiming to "handle everything" without clear shared responsibility documentation remain a persistent failure pattern

**Consultant and ESP Quality Directly Correlates to Scores:**
- Companies that achieve perfect 110 scores consistently work with **good consultants and ESPs** -- this is the "biggest interconnecting tissue" Fernando has observed
- The most successful consultants/ESPs have **DIBCAC experience** from having gone through DIBCAC High assessments
- This aligns with the broader pattern: companies that invest in experienced partners outperform those that try to go it alone or use inexperienced providers

*(Source: [[What to Know From a C3PAO]], Summit 7, December 2024)*

### NAVAIR Opportunity Analysis -- Market Size and Timeline Pressure

Analysis of NAVAIR's December 2025 Long Range Acquisition Forecast (LRAF) reveals the scale and urgency of the CMMC market for naval aviation programs. The LRAF listed **1,676 contract opportunities** ranging from $700K to multi-billion dollars, covering everything from missile systems to drone sustainment.

**Market scale indicators:**
- **1,070 opportunities** with calculable timelines (both solicitation and award dates listed)
- **550 unclassified opportunities** alone, averaging only 9 months from solicitation to award
- **294 opportunities under $2M** -- the bread-and-butter contract size for small businesses -- with an average of only **8 months** from solicitation to award
- Contract types span: repairs, redesigns, prototypes, full life cycle support, C-130s to drones

**Timeline pressure on the market:**
- **35% of all opportunities** have a 6-month or shorter award window -- far too short for most companies to achieve certification from a standing start
- **30% of solicitations** and **32% of contract awards** are concentrated in Q2 2026, creating a near-term surge of CMMC-gated opportunities
- The smaller the contract, the less preparation time -- this systematically disadvantages the small businesses that make up most of the DIB
- Internal procurement cycles (budget approvals, vendor selection, project kickoffs) consume approximately one quarter of the available window before implementation work even begins

**Service demand implications:**
- Companies pursuing sub-$2M contracts need accelerated implementation programs that can deliver results in well under 8 months
- The Q2 2026 concentration creates a near-term capacity crunch for consultants, MSPs, and C3PAOs
- Subcontractors face compounded pressure: primes are requiring certification evidence to view classified solicitations, and subcontractors often have no visibility into the PALT window
- PALT analysis services and strategic planning offerings are themselves a market opportunity -- contractors need help calculating their specific risk exposure

*(Source: [[No CMMC, No Contract - Why You're Already Too Late for NAVAIR]], Summit 7, February 2026)*

## Decision Criteria
- **Are you a service provider targeting the DIB?** --> The 96% who are not self-educating represent the largest untapped market
- **Serving SMBs?** --> Right-sized compliance packages beat enterprise-scale solutions; cost sensitivity is extreme
- **Offering technical services?** --> FIPS breakage remediation and ESP scoping are the highest-demand engineering challenges
- **Offering consulting?** --> Translating vague guidance into actionable steps is the core value proposition
- **Offering training?** --> Both OSCs and assessors need education; misconceptions persist even among credentialed practitioners

## Common Misconceptions
| Misconception | Reality | Source |
|---|---|---|
| Buying GCC High = compliance | GCC High is a prerequisite for CUI handling, not a compliance solution by itself -- you still need controls, documentation, and assessment | [[Community Sentiment and Common Frustrations]] |
| CMMC is just a cost center | CMMC is a revenue enabler and competitive differentiator; a company sold for $1B with CMMC readiness cited as a valuation factor | [[Getting CMMC Executive Buy-In with Jeff Smedley]] |
| The government will eventually subsidize compliance costs | No appropriations exist and no appetite in Congress; compliance costs are considered already paid for through contract rates | [[CMMC Phase 1 - What Comes Next]] |
| We can delay until costs come down or subsidies arrive | Every month of delay erodes competitive position and company valuation; this is an "astronomically unlikely scenario" | [[CMMC Phase 1 - What Comes Next]] |
| CMMC is an IT problem that IT can just fix | Cultural adoption is the long pole; requires board-level ownership, CFO partnership, and BD team alignment | [[Getting CMMC Executive Buy-In with Jeff Smedley]] |
| "My MSP says we're covered" | Many MSPs claim compliance without doing real compliance work; this is widespread in the 96% who are not self-educating | [[Community Sentiment and Common Frustrations]] |
| The CMMC market is fake because only a few hundred certs exist | Certifications are a fraction of the market -- thousands of companies are pursuing compliance; the services and assessment ecosystems are two different parts of the CMMC world | [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] |
| MSPs are certified or regulated | There is no certifying body for MSPs -- no UL, no ABA, no professional certification. Anyone can hang out a shingle and offer CMMC compliance services | [[Where Cybersecurity Meets Legal]] |
| 802.1x is required for control 3.1.1 | 802.1x network access control is NOT a requirement for satisfying 3.1.1 -- there are multiple valid approaches | [[Community Sentiment and Common Frustrations]] |
| Windows Hello PIN is not MFA | Windows Hello for Business with PIN qualifies as MFA: something you have (TPM-bound device) + something you know (PIN) | [[Community Sentiment and Common Frustrations]] |
| RMF expectations apply to CMMC | Some assessors from RMF backgrounds apply DoD RMF expectations that are overkill or misapplied in a CMMC Level 2 context | [[Community Sentiment and Common Frustrations]] |

## Open Questions / Debates
- **How long does implementation actually take?** Jeff Smedley suggests starting from ground zero with a 100-person company, 12-18 months is realistic. Technical buildout is only part of the challenge -- organizational and cultural adoption is the "long pull in the tent." *(Source: [[Getting CMMC Executive Buy-In with Jeff Smedley]], July 2025)*
- **Will small businesses survive?** Companies that cannot afford compliance face three options: comply, diversify out of defense, or sell before CMMC is required. Those who sell without CMMC readiness "get pennies for the dollar." *(Source: [[Getting CMMC Executive Buy-In with Jeff Smedley]], July 2025)*
- **Will the 96% ever get compliant?** The vast majority of DIB companies needing Level 2 are not even aware of the requirements. Whether market forces, contract loss, or government enforcement will drive adoption is an open question.
- **RMF vs. CMMC assessor expectations**: Some assessors bring RMF-level expectations to CMMC assessments. Per community: "Can we please explain to assessors that everything you may have seen working for the DoD or with RMF is NOT expected in CMMC?" This mismatch creates inconsistent assessment outcomes.
- **Control 3.13.13 (mobile code)**: Described as "one of the hardest requirements to explain as a consultant and one of the hardest to evaluate as an assessor" -- this generates more confusion per word than almost any other NIST 800-171 requirement.

## Related Topics
- [[Enclaves and Architecture Strategies]] -- enclave demand across manufacturing, AEC, and regulated research verticals
- [[FIPS 140-2 and 140-3 Compliance]] -- FIPS breakage is a key engineering service opportunity
- [[Scoping and Assessment Boundaries]] -- ESP scoping services as key market opportunity
- [[GCC High vs Commercial M365]] -- GCC High migration as a major cost driver and service opportunity
- [[SPRS and Annual Affirmation]] -- Annual affirmation adds to the ongoing compliance burden for SMBs
- [[CMMC Levels and Framework Structure]] -- Understanding what 96% of companies are missing
- [[Assessment Process and Timeline]] -- Mock + real assessment costs are a major SMB expense
- [[False Claims Act and DOJ Enforcement]] -- FCA enforcement risk driving urgency for compliance services
- [[Phase Rollout and Contract Language]] -- timeline pressure driving market demand for compliance services

## Sources
- [[Community Sentiment and Common Frustrations]] -- Frustration-to-service-opportunity mapping, the 96% problem, SMB cost pressure ($100K+ for 30-person shop), DIB readiness gap, common misconceptions (802.1x, Windows Hello, RMF mismatch), mobile code confusion, community sentiment summary
- [[CMMC Phase 1 - What Comes Next]] -- Early adopters winning work, no subsidies/appropriations, compliance as allowable cost, delay strategy risks
- [[Getting CMMC Executive Buy-In with Jeff Smedley]] -- Cost estimates ($100K/100 employees), CMMC as revenue enabler, $1B acquisition case study, executive buy-in framework, CFO partnership strategy
- [[What to Know From a C3PAO]] -- Early adopter public vs. private behavior, MSP force multiplier role, consultant/ESP quality correlation to scores, DIBCAC experience as differentiator
- [[No CMMC, No Contract - Why You're Already Too Late for NAVAIR]] -- NAVAIR LRAF analysis (1,676 opportunities), PALT timeline pressure by contract value, small business disadvantage, Q2 2026 surge, subcontractor visibility gap
- [[CMMC Enclaves by Industry]] -- Enclave demand across manufacturing, AEC, and regulated research verticals; construction as surprising growth area; universities as emerging complex market; managed vs hosted enclave service models
- [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] -- MSP vetting (trunk slammers, SRM requirement, Reddit horror story, contract buyout traps, firing MSP = significant change at $40-70K), "less about money more about time" market shift, every vertical affected (construction, manufacturing, SaaS, higher ed), GCC High tenant count as DIB readiness litmus test, CMMC market not fake
- [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]] -- Assessment cost vs implementation cost ($1M+ for 800-171), DIB IT spend 1% vs 7-8% in regulated industries, DIB as most heavily regulated industry, no DoD funding, set-asides don't trump CMMC, "compliant in 60 days" surge demand, expedite fees, 5-8% projected IT spend increase
- [[Where Cybersecurity Meets Legal]] -- MSP certification gap (no certifying authority), MSP onboarding bottleneck, C3PAO assessment suspensions due to SSP readiness, attorney perspective on market dynamics (Mike McGlachlin)
