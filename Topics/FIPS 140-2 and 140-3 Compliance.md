---
title: FIPS 140-2 and 140-3 Compliance
aliases:
  - FIPS
  - FIPS 140-2
  - FIPS 140-3
  - FIPS Validated Cryptography
tags:
  - cmmc
  - fips
  - cryptography
  - technical
confidence: confirmed
last_verified: 2026-02-20
sources:
  - "[[Community Sentiment and Common Frustrations]]"
  - "[[The CUI Hotline - Weekly CMMC Q&A Livestream!]]"
---

## Summary
FIPS mode is a hard requirement for CUI protection, but enabling it causes real-world breakage across common enterprise tools including PLM systems, VMware Horizon, Intune MDM, and legacy applications. This is not a documentation problem but a genuine engineering challenge that requires testing and remediation before assessment.

## Key Facts
- FIPS mode is a **hard requirement** for CUI protection under CMMC Level 2
- Enabling FIPS mode causes real-world breakage across common enterprise tools -- this is not a documentation problem but a genuine engineering challenge
- **PLM systems** (Product Lifecycle Management) often break under FIPS enforcement
- **VMware Horizon** VDI environments experience compatibility issues with FIPS
- **Intune MDM** has registry key confusion -- FIPS enforcement through MDM policies is not straightforward
- **Legacy applications** that use non-FIPS cryptographic libraries break silently when FIPS mode is enabled
- FIPS breakage is one of the top pain points in the CMMC practitioner community and represents a real engineering services opportunity
- The cost of PLM system hardening for FIPS is a significant contributor to overall SMB compliance costs

## How It Works

### FIPS Mode Breakage -- Known Problem Systems

| System | FIPS Issue |
|---|---|
| **PLM systems** | Product Lifecycle Management tools often break under FIPS enforcement |
| **VMware Horizon** | VDI environments experience compatibility issues |
| **Intune MDM** | Registry key confusion -- FIPS enforcement through MDM policies is not straightforward |
| **Legacy applications** | Many older apps use non-FIPS cryptographic libraries and break silently |
| **AutoCAD** | Enabling FIPS on physical devices breaks AutoCAD -- a critical tool for manufacturing and AEC enclaves |
| **QuickBooks** | Enabling FIPS on QuickBooks on-prem causes it to stop working entirely |
| **Revit** | Subject to the same FIPS breakage as AutoCAD; compounded by EOL version retention requirements |

*(AutoCAD/QuickBooks/Revit source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

### The Engineering Challenge
Enabling FIPS is not a checkbox exercise. Each of these breakages requires dedicated testing and remediation:
- PLM systems may need vendor patches, configuration changes, or architecture redesign
- VMware Horizon environments need specific FIPS-compatible configurations
- Intune MDM FIPS enforcement requires careful registry key management that differs from standard MDM policy deployment
- Legacy applications may require replacement, wrapping, or isolation if they cannot be made FIPS-compliant
- **AutoCAD, Revit, and QuickBooks** break when OS-level FIPS is enabled on physical devices -- most application vendors "hadn't realized what FIPS was" until CMMC drove a wave of demand. For these applications, the workaround is to run them in Azure Virtual Desktop where **Azure hardware is FIPS validated and encrypted at the drive level**, satisfying the FIPS requirement without enabling the OS-level FIPS flag that breaks the application. *(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

### Azure Hardware-Level FIPS

Azure Gov infrastructure provides FIPS validation at the hardware/drive level:
- All data processed on Azure VMs inherits FIPS-validated encryption at the drive level
- This allows organizations to run FIPS-incompatible applications (AutoCAD, QuickBooks, Revit) in Azure Virtual Desktop without enabling the OS-level FIPS flag
- **Physical devices** do not get this benefit -- FIPS must be enabled at both the hardware and software level, which is where application breakage occurs
- This distinction is critical for [[Enclaves and Architecture Strategies|enclave]] design: applications that break under FIPS should be run in Azure VDI rather than on physical workstations where possible

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

### Encrypted Print Workaround (Printer Logic)

Print jobs are sent in plain text by default, which brings the traversed network into scope. Solutions:
- **Printer Logic** provides FIPS 140 encrypted print from the enclave through to the remote printer, with badge/code release at the device
- Combined with a site-to-site VPN (TLS 1.2), this keeps the intermediary network out of scope
- Summit 7's own CMMC-certified environment uses an analogous approach: remote workers connect to GCC High over TLS from home laptops, with the alternate work site policy keeping the home network out of scope
- **NIST position**: If data is encrypted to FIPS standards, it is not considered plain text -- if it is not encrypted to FIPS, it IS considered plain text regardless of other encryption present

*(Source: [[CMMC Enclaves by Industry]], Summit 7, June 2025)*

### When FIPS Is (and Is Not) Required

FIPS validation is required **only when encryption is the method used to protect CUI**. Organizations have a choice between encryption and physical protection:

- **When encryption is the mechanism you rely on** for the protection of CUI, that encryption **must be FIPS validated**
- **Physical compensating controls can substitute** for encryption in certain scenarios -- locks on doors, secured areas, and physical access controls can protect CUI without requiring FIPS encryption on those systems
- This is not an either/or at the environment level -- different parts of the environment can use different protection methods

**Internal vs. External Network Distinction:**

| Location | Typical Approach |
|---|---|
| **Externally facing** (firewalls, internet-facing appliances) | FIPS validated encryption required |
| **Internal traffic** (systems within a secured physical boundary) | Physical compensating controls may suffice -- FIPS not required if physical protection is adequate |

Network appliances can be scoped with FIPS enabled or disabled depending on where they are located and how CUI is protected at that point. A common pattern is FIPS-validated firewalls externally with non-FIPS internal traffic protected by physical controls.

*(Source: [[The CUI Hotline - Weekly CMMC Q&A Livestream!]], Summit 7, February 2026)*

### Wireless and FIPS Interaction
If all CUI traffic over wireless is FIPS-encrypted through a VPN, certain wireless-specific controls can legitimately be marked as Not Applicable. The encryption satisfies the protection requirement regardless of the transport medium.

## Decision Criteria
- **Handling CUI?** --> FIPS-validated cryptography is required for data at rest and in transit
- **Using PLM, VMware Horizon, or Intune?** --> Plan for FIPS breakage testing and remediation before assessment
- **Running legacy applications?** --> Test each one under FIPS mode; many use non-FIPS crypto libraries that break silently
- **CUI over wireless via FIPS-encrypted VPN?** --> Wireless-specific controls can potentially be marked N/A

## Common Misconceptions
| Misconception | Reality | Source |
|---|---|---|
| Enabling FIPS mode is a simple checkbox | FIPS mode causes real-world breakage across PLM, VMware Horizon, Intune MDM, and legacy applications -- it requires testing and engineering remediation | [[Community Sentiment and Common Frustrations]] |
| Wireless controls always apply | If all CUI traffic over wireless is FIPS-encrypted through a VPN, certain wireless-specific controls can be marked N/A | [[Community Sentiment and Common Frustrations]] |
| Legacy apps will keep working under FIPS | Many older applications use non-FIPS cryptographic libraries and break silently when FIPS mode is enabled | [[Community Sentiment and Common Frustrations]] |
| AutoCAD/Revit/QuickBooks work fine with FIPS enabled | These applications break when OS-level FIPS is enabled on physical devices -- the workaround is Azure VDI where FIPS is handled at the hardware/drive level | [[CMMC Enclaves by Industry]] |
| You must enable OS-level FIPS on every CUI asset | Azure VMs inherit FIPS-validated encryption at the drive level, satisfying the requirement without the OS-level FIPS flag that breaks applications | [[CMMC Enclaves by Industry]] |
| Print jobs are encrypted by default | Print jobs are sent in plain text -- use Printer Logic (FIPS 140 end-to-end) or encrypted USB + staging laptop to avoid bringing the network into scope | [[CMMC Enclaves by Industry]] |
| FIPS is required for all encryption in the CUI environment | FIPS is required only when encryption is the method used to protect CUI -- physical compensating controls (locks, secured areas) can substitute for internal traffic | [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] |
| Internal network traffic must be FIPS encrypted | Internal traffic can be protected by physical controls instead of encryption -- only externally facing systems must use FIPS-validated encryption | [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] |

### Top Failed Control -- C3PAO Assessment Data (Fernando Machado)

Fernando Machado (provisional assessor #8, 29th authorized C3PAO) identifies FIPS validated cryptography as one of the **top 2 most-failed controls** he has observed across assessments (alongside MFA):

- The primary failure pattern: contractors implement firewalls with the **latest and greatest firmware** but **forget to put the firewall into FIPS mode** with the correct firmware version
- This is not just about enabling FIPS -- the firmware version matters because FIPS-validated firmware may differ from the latest available firmware
- FIPS failure is a consistent observation across both JSVA and CMMC assessments, aligning with DIBCAC's published findings from Nick Del Rosso's reports

*(Source: [[What to Know From a C3PAO]], Summit 7, December 2024)*

## Open Questions / Debates
- The extent to which FIPS-broken legacy applications can be isolated or wrapped versus replaced is an ongoing engineering debate
- Whether Intune MDM registry key enforcement qualifies as proper FIPS enforcement is contested -- the MDM policy approach does not map cleanly to FIPS requirements

## Related Topics
- [[Scoping and Assessment Boundaries]] -- FIPS requirements apply to systems within the CUI boundary
- [[Market Dynamics and Service Needs]] -- FIPS breakage remediation is a key service opportunity
- [[CMMC Levels and Framework Structure]] -- FIPS is required at Level 2 for CUI protection
- [[Enclaves and Architecture Strategies]] -- Azure VDI as FIPS workaround for incompatible applications, encrypted print solutions, physical vs virtual tradeoffs
- [[GCC High vs Commercial M365]] -- Azure Gov hardware FIPS validation at drive level

## Sources
- [[Community Sentiment and Common Frustrations]] -- FIPS breakage across PLM, VMware Horizon, Intune MDM, and legacy apps; wireless N/A when FIPS-encrypted VPN is used
- [[What to Know From a C3PAO]] -- FIPS as #1 failed control (alongside MFA), firewall FIPS mode firmware mismatch pattern
- [[CMMC Enclaves by Industry]] -- AutoCAD/QuickBooks/Revit FIPS breakage, Azure hardware-level FIPS as workaround, Printer Logic FIPS 140 encrypted print, NIST plain text definition, alternate work site policy for encrypted connections
- [[The CUI Hotline - Weekly CMMC Q&A Livestream!]] -- FIPS only when encryption is the protection method, physical compensating controls as alternative, internal vs. external network distinction, firewall externally = FIPS validated / internal = physical protection acceptable
