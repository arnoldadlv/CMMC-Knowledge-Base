---
title: Enclaves and Architecture Strategies
aliases:
  - Enclaves
  - CUI Enclaves
  - Architecture Strategies
  - Enclave Strategy
tags:
  - cmmc
  - enclaves
  - architecture
  - technical
confidence: consensus
last_verified: 2026-02-20
sources:
  - "[[CMMC Enclaves by Industry]]"
---

## Summary

An enclave is a bounded subset of an organization's environment specifically designated for processing, storing, and transmitting CUI. Not all assets across the enterprise need to be in the CMMC assessment scope -- only those people, processes, and technologies that handle CUI. Enclave strategies vary significantly by industry vertical (manufacturing, AEC, regulated research), and the decision to enclave versus go enterprise-wide depends on CUI prevalence, data flow complexity, and the percentage of users who need CUI access.

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

## Key Facts

- **CMMC L2 scoping guidance** establishes that not all assets across an OSC enterprise are automatically part of the assessment scope -- you get to select the people, places, and technologies that process, store, and transmit CUI
- **15% rule**: If more than 15% of users need access to CUI, the overhead of maintaining two separate environments (enclave + corporate) and the risk of CUI spillage increases significantly -- users take the path of least resistance and will bypass enclave controls
- **VDI latency threshold**: Virtual desktop performance degrades badly above **70 milliseconds** of latency -- test the worst-case user location before committing to a VDI-based enclave
- **Print jobs are sent in plain text** by default -- FIPS-enabled printers are very expensive and hard to find; encrypted USB + staging laptop is the common workaround
- **Specialized assets** (CNC machines, test equipment, IoT, OT) can process, store, and transmit CUI but do not need all 110 CMMC controls applied -- a risk-based approach is permitted under the CMMC L2 scoping guidance
- **Four asset types in an enclave**: CUI assets, Security Protection Assets (SPA), Contractor Risk Managed Assets (CRMA), and Specialized Assets
- **CRMAs are described as "a damn dirty trap"** -- assessors can challenge the CRMA classification and require assessment against all 110 controls
- **Hybrid enclave** (cloud + on-prem) brings physical site protection requirements into scope -- the question becomes whether it is a single secure room or an entire facility
- **Hyporei Android app** enables mobile CUI access through an Android instance running Microsoft GovCloud apps, eliminating the need for two physical devices
- **Azure Virtual Desktop with GPUs** (NVIDIA cards) is the standard platform for engineering applications in enclaves; H100 cards are currently available in Azure Gov, H200s forthcoming
- **Printer Logic** provides FIPS 140 encrypted print from enclave to remote printer, end-to-end, with badge/code release at the printer

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

## How It Works

### Data Flow Analysis -- The Critical First Step

Before deciding on an enclave, you must know where all your CUI lives. Daniel Acreage recommends searching your M365 commercial tenant and on-prem file systems for:

- **CUI banner markings**
- **DoD clauses**
- **DoD distribution statements** (Parts B through F)

> [!example] Construction Company Discovery
> A large construction company's CIO planned a 20-person enclave based on gut feeling. After running distribution statement searches, they found **570 files from DoD distribution statements alone** -- and that was only what Microsoft could OCR through PDFs, email, and standard Office attachments. It did not include AutoCAD, SolidWorks, or Revit files. The actual CUI footprint was far larger than 20 people.

This search pays dividends because it prevents the painful "second ask" to executives when you discover six months later that the enclave needs to be much larger than originally planned. Do one big ask with as much data as possible.

> [!warning] IT Cannot Answer These Questions Alone
> CMMC is not solely an IT problem. Data flow analysis requires input from BD, contracts, engineering, and executive leadership. IT supports the infrastructure where CUI may live, but they do not always know whether the data on that infrastructure is CUI.

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

### Manufacturing Enclaves

Manufacturing enclaves present unique challenges around physical equipment and specialized software:

- **Engineering applications**: AutoCAD, SolidWorks, and similar tools require GPU-backed virtual desktops (Azure Virtual Desktop with NVIDIA cards)
- **Print-to-shop-floor workflow**: Manufacturing facilities need to print drawings for assembly -- a harness manufacturer in Huntsville needed 7 computers for CUI work, printing to a shop floor where 50 people assembled harnesses across a dozen desks
- **USB staging laptop approach**: A physical laptop joined to the GovCloud pulls data over TLS, copies to an approved encrypted USB, which is then carried to the shop floor or OT environment -- avoids sending plain-text print jobs across the network
- **Specialized assets**: CNC machines running Windows XP, Windows 2000, or MS-DOS cannot meet all 110 controls but can be classified as specialized assets with a risk-based security approach. One manufacturer has to buy scuzzy drives off eBay with auto-buy alerts just to keep laser cutting systems alive
- **Physical vs. VDI**: Sales and BD teams may work fine on virtual desktops, but manufacturing engineering applications may require physical workstations -- do not assume VDI works for everyone
- **Physical site consolidation**: Large international manufacturers with defense work across 50+ sites worldwide have had to consolidate CUI-processing manufacturing to one or two US-based physical sites -- this can take years
- **Hyporei mobile**: Android app provides mobile CUI access via an Android instance running Microsoft GovCloud apps, eliminating the need for two physical devices for salespeople in the field

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

### AEC (Architecture, Engineering, Construction) Enclaves

AEC enclaves share many manufacturing challenges plus additional complexities around field work and plotting:

- **Same engineering applications**: AutoCAD, Revit, SolidWorks, Blue Beam
- **Blueprint plotting**: Companies need to plot blueprints and schematics for job sites, but plotting sends data in plain text across the network
- **Tablets for job sites**: Instead of printing, digitize where possible -- use CUI-compliant iPads joined to the GovCloud for reviewing drawings and taking pictures on job sites, with uploads going directly to OneDrive/SharePoint/Teams
- **Blue Beam workaround**: Blue Beam is not FedRAMP authorized as a cloud service, but has a local install option that can be self-hosted inside an enclave -- "you have to go through three back doors and knock twice" to get it, but it exists
- **[[FIPS 140-2 and 140-3 Compliance|FIPS]] breaks engineering software**: Enabling FIPS on physical devices breaks AutoCAD and similar tools; see the [[FIPS 140-2 and 140-3 Compliance]] page for details
- **Secure print room**: If printing is unavoidable, designate a specific room as the physical CUI print room to avoid bringing the entire facility into scope
- **Pooled licensing via site-to-site VPN**: Connect back to on-prem license servers through a site-to-site VPN to avoid buying duplicate license pools for the GovCloud enclave -- the license server itself is not a CUI asset
- **Enclave trailer concept**: Ryan Bonner and Daniel Acreage have discussed the idea of a mobile enclave trailer that gets driven to job sites with physical protections, drawings, and iPads for checkout
- **Alternate work site policy**: Remote workers connecting from home to GCC High over TLS are covered by the alternate work site policy -- their home network is not in scope because the connection is FIPS-validated encrypted end-to-end
- **Printer Logic for encrypted print**: FIPS 140 encryption from enclave through to the remote printer, with badge/code release at the device, over a site-to-site VPN -- this approach has been accepted by assessors as keeping the intermediary network out of scope

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

### Regulated Research Enclaves

Universities and research institutions face a unique set of enclave challenges driven by researcher autonomy, export control, and cost allocation:

- **Applications**: MatLab, Python, and domain-specific research tools
- **Non-US person segmentation**: Must segment non-US persons away from export control data while potentially allowing them access to non-export-controlled CUI. Implementation approach:
  - Use **Purview site containers** and **custom attributes** for US/non-US person identification in the tenant
  - Feed citizenship/personship data from HR systems (Workday, etc.) into Active Directory and Entra ID provisioning
  - Use **dynamic groups** to auto-assign permissions based on custom attributes
  - Apply site container permissions per export control classification
  - Naval nuclear propulsion information requires US **citizens** (not just US persons -- green cards do not suffice)
- **Chargeback per grant/contract/subscription**: The CIO's office does not want to foot the entire bill. Azure subscription provisioning allows unique chargebacks per research grant, contract, or subscription -- build this architecture on the front end because doing it retroactively is much harder
- **Centralized oversight is critical**: Do NOT let individual departments spin up their own enclaves -- it must sit under the CIO's office

> [!warning] Top 10 University Horror Story
> A top-10 US university called Summit 7 after discovering **two high-performance compute on-prem environments** doing highly regulated research that the CIO's office did not know existed. A researcher or grad student had set them up in a closet with power supplies -- zero NIST 800-171 controls applied.

- **Researcher AWS problem**: Research contracts are often awarded directly to the researcher, who then signs up for AWS commercial with a Gmail account and starts processing CUI with zero oversight or controls
- **Tension between research dollars and compliance**: Universities are reluctant to confront researchers because they bring research grant money -- finding the balance between enabling research and enforcing compliance is "a lot easier said than done"
- **200+ labs**: One large research institute has approximately 200 labs, none managed exactly the same way -- the strategy is to roll as much compliance as possible into the cloud and limit physical protection requirements on-prem
- **Site-to-site VPN to labs**: Connect physical research labs back to the GovCloud enclave environment

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

### CDO (Customer Documents Only) Enclaves -- Minimum Viable Enclave

The smallest enclave type is the **CDO enclave** -- a "look but don't touch" environment for receiving customer documents:

- Documents are piped in from DoD Safe, portals, or shared mailboxes into a contained environment
- **Read-only access** -- documents cannot leave the enclave to prevent scope expansion
- Requires **rearchitecting business processes** -- customers must be trained to communicate through new channels (e.g., dedicated shared mailbox instead of emailing individual engineers)
- **Conway's Law applies**: communication flows must inform the system design, otherwise you end up with a system no one uses
- CDO enclaves are **minimum viable product** -- they buy time but rarely match how the business actually operates
- Most organizations will immediately need to expand beyond CDO because "that doesn't match the way we do business"

**Key evaluation criteria for CMMC-as-a-Service per-seat enclaves:**
- How many "knobs and levers" can you adjust? (install software, expand user count, add workloads, add applications)
- If you cannot install software or visit more than five websites, understand those limitations upfront
- A per-seat enclave likely **only buys time** -- plan for migration to something more capable or determine it is not for you

*(Source: [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]], Summit 7, January 2026)*

### Hosted vs. Managed Enclaves

There are two fundamental enclave delivery models:

**Hosted Enclave** -- You buy a per-seat subscription to someone else's environment:
- The provider owns the hardware and infrastructure
- Typically does not scale well
- **Hard to get your data out** if you need to change providers -- one organization took three months to migrate out
- **Difficult to extend on-prem** for hybrid use cases (manufacturing shop floors, research labs)
- Requires the hosted provider to be **FedRAMP Moderate** (or equivalent) since they are acting as a CSP
- You still cannot avoid the customer responsibility matrix

**Managed Enclave** -- You own the Microsoft GovCloud subscriptions and a partner manages them:
- You own the Microsoft GCC High tenant and Azure Gov subscriptions
- You **inherit Microsoft's SSP** for physical controls and platform security
- You inherit the managed service provider's customer responsibility matrix (e.g., Summit 7's CRM)
- **Data portability**: If you part ways with the managed provider, the environment keeps running -- your data stays in your tenant
- Can extend on-prem through hybrid configurations
- Most organizations prefer this model for control and portability

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

### Asset Types Within an Enclave

| Asset Type | Description | Controls Required | Notes |
|---|---|---|---|
| **CUI Asset** | Systems that process, store, or transmit CUI | All 110 CMMC L2 controls | Always in scope |
| **Security Protection Asset (SPA)** | Assets providing security functions for CUI but not processing CUI directly | Relevant security controls | Firewalls, SIEM, identity systems |
| **Contractor Risk Managed Asset (CRMA)** | Assets on the same network as CUI assets but not supposed to process CUI | Policies and procedures | "A damn dirty trap" -- assessor can upgrade to full 110 control assessment |
| **Specialized Asset** | OT, IoT, test equipment, government property, restricted info systems | Risk-based approach | Does NOT require all 110 controls; critical for manufacturing and research |

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

## Decision Criteria

### When to Enclave vs. Enterprise-Wide

- **Less than 15% of users need CUI access?** --> Enclave is a strong candidate; reduces scope and cost
- **More than 15% of users need CUI access?** --> Enclave overhead and spillage risk increase significantly; consider enterprise-wide compliance
- **Not sure how many users need CUI access?** --> Run the data flow search first (CUI banners, DoD distribution statements, DoD clauses) before deciding

### Hosted vs. Managed Enclave

- **Need on-prem integration** (shop floors, labs, OT)?  --> Managed enclave is strongly preferred; hosted enclaves are difficult to extend on-prem
- **Concerned about vendor lock-in?** --> Managed enclave; you own the tenant and the data
- **Small team, want simplest possible setup?** --> Hosted enclave may work but understand the FedRAMP requirement and data portability limitations
- **Need to scale over time?** --> Managed enclave scales better because you control the subscriptions

### Physical Workstations vs. VDI

- **User latency above 70ms?** --> VDI will perform poorly; consider physical workstations
- **Engineering applications (AutoCAD, SolidWorks, Revit)?** --> Test VDI performance carefully; physical workstations may be necessary depending on GPU requirements and latency
- **Sales/BD users?** --> VDI is typically sufficient
- **Mobile workers in the field?** --> Hyporei Android app or CUI-compliant tablets (iPads)

### Printing CUI

- **Can you avoid printing?** --> Use tablets and digital workflows instead
- **Must print?** --> Use encrypted USB + staging laptop + approved USB printer (not traversing the network), OR use Printer Logic for FIPS 140 encrypted print end-to-end
- **Do NOT send plain-text print jobs across a network** that is supposedly out of scope -- it brings the network into scope

## Common Misconceptions

| Misconception | Reality | Source |
|---|---|---|
| "20 users = our CUI footprint" | Without data flow analysis, gut estimates of CUI scope are almost always wrong. One construction company thought 20 people; a search returned 570 files from DoD distribution statements alone | [[CMMC Enclaves by Industry]] |
| "I can build an enclave for all my suppliers" | Suppliers using your enclave for their CMMC certification boundary cannot do competitive work for other primes in your environment -- the certification boundary becomes very complex | [[CMMC Enclaves by Industry]] |
| "CRMA is a good way to avoid controls" | CRMAs are "a damn dirty trap" -- an assessor can challenge the classification and require assessment against all 110 controls on that asset, creating a nasty surprise if you were not prepared | [[CMMC Enclaves by Industry]] |
| "VDI works for everyone" | Engineering applications may require physical workstations; latency above 70ms makes VDI unusable; manufacturing OT environments often cannot run virtually | [[CMMC Enclaves by Industry]] |
| "We just need to enable FIPS on everything" | Enabling FIPS breaks AutoCAD, QuickBooks, and other common applications -- Azure handles FIPS at the hardware/drive level, but physical devices require careful testing | [[CMMC Enclaves by Industry]] |
| "An enclave is our forever solution" | An enclave may be a stop-gap while you figure out how much larger your CUI scope actually is -- it is often the beginning, not the end | [[CMMC Enclaves by Industry]] |
| "IT can handle enclave scoping alone" | Data flow analysis requires BD, contracts, engineering, and executive input -- IT manages the infrastructure but does not know which data is CUI | [[CMMC Enclaves by Industry]] |

## Open Questions / Debates

- **Supplier enclave certification boundary**: If you build an enclave and allow suppliers to use it for their CMMC scope, how do you handle the certification boundary when those suppliers do competitive work with other primes? No clean answer exists yet. *(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*
- **Rev 3 impact on specialized assets**: Rev 2 allows a risk-based approach for specialized assets (OT, CNC machines, test equipment). Rev 3 may be "a little bit more heavy-hitting" on those requirements. Proactively seek DoD CIO exemptions for EOL systems now. *(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*
- **EOL software and records retention**: Revit releases yearly versions with only 3 years of support, but DoD requires records retention of data created in older versions. The recommended approach: seek DoD CIO exemptions proactively and have them on file for your assessor. *(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*
- **Encrypted print job scoping**: Whether a FIPS 140 encrypted print path (e.g., Printer Logic) keeps the intermediary network out of scope is still debated by assessors -- Summit 7 argues it should be treated the same as TLS to GCC High, and this has held up in their own CMMC certification. *(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*
- **Rev 2 to Rev 3 transition**: GSA is already using Rev 3 while CMMC remains pinned to Rev 2. Application allow-listing is only in Rev 3. Split tunneling requirements differ between revisions. Organizations should adopt ODPs (Organization-Defined Parameters) now to ease transition. *(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

## Related Topics

- [[Scoping and Assessment Boundaries]] -- asset classifications (CUI, SPA, CRMA, Specialized) and assessment boundary decisions
- [[FIPS 140-2 and 140-3 Compliance]] -- FIPS application breakage, Azure hardware FIPS, encrypted print
- [[GCC High vs Commercial M365]] -- GCC High as the cloud foundation for enclaves, Business Premium licensing
- [[Market Dynamics and Service Needs]] -- enclave demand across verticals, emerging markets
- [[ESP (External Service Provider) Classification]] -- hosted enclave providers as ESPs requiring FedRAMP
- [[CRM (Customer Responsibility Matrix)]] -- managed enclave CRM inheritance from Microsoft SSP and service providers
- [[SSP Development]] -- documenting the enclave boundary and asset classifications
- [[Assessment Process and Timeline]] -- how enclave boundaries affect what gets assessed

## Sources

- [[CMMC Enclaves by Industry]] -- Daniel Acreage (Summit 7), June 2025. Primary source for enclave definition, 15% rule, data flow analysis, manufacturing/AEC/regulated research enclave considerations, hosted vs managed models, asset types, CRMA trap, supplier enclave gotcha, specialized assets, VDI latency threshold, printing challenges, Blue Beam workaround, Printer Logic encrypted print, Hyporei mobile, chargeback model, non-US person segmentation, EOL software challenge, Rev 2 to Rev 3 transition
- [[CUI Hotline - Weekly Q&A with Ryan Bonner (Jan 24 2026)]] -- CDO (Customer Documents Only) enclave type, CMMC-as-a-service per-seat evaluation criteria, Conway's Law and business process rearchitecting, CDO as minimum viable product that buys time
