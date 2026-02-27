# SI.L2-3.14.1 – Flaw Remediation [CUI Data]

## Security Requirement Identify, report, and correct information and information system flaws in a timely manner. |

## Assessment Objectives [a] the time within which to identify system flaws is specified;  [b] system flaws are identified within the specified time frame;  [c] the time within which to report system flaws is specified;  [d] system flaws are reported within the specified time frame;  [e] the time within which to correct system flaws is specified; and  [f] system flaws are corrected within the specified time frame. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SI.L2-3.14.1 – FLAW REMEDIATION

Level 1 Requirement: SI.L1-b.1.xii

### SECURITY REQUIREMENT

Identify, report, and correct information and information system flaws in a timely manner.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the time within which to identify system flaws is specified;
:   [b] system flaws are identified within the specified time frame;
:   [c] the time within which to report system flaws is specified;
:   [d] system flaws are reported within the specified time frame;
:   [e] the time within which to correct system flaws is specified; and
:   [f] system flaws are corrected within the specified time frame.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and information integrity policy; procedures addressing flaw remediation; procedures addressing configuration management; system security plan; list of flaws and vulnerabilities potentially affecting the system; list of recent security flaw remediation actions performed on the system (e.g., list of installed patches, service packs, hot fixes, and other software updates to correct system flaws);test results from the installation of software and firmware updates to correct system flaws; installation/change control records for security-relevant software and firmware updates; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; personnel installing, configuring, and maintaining the system; personnel with responsibility for flaw remediation; personnel with configuration management responsibility].

**Test**

[SELECT FROM: Organizational processes for identifying, reporting, and correcting system flaws; organizational process for installing software and firmware updates; mechanisms supporting or implementing reporting, and correcting system flaws; mechanisms supporting or implementing testing software and firmware updates].

### DISCUSSION

Organizations identify systems that are affected by announced software and firmware flaws including potential vulnerabilities resulting from those flaws and report this information to designated personnel with information security responsibilities. Security-relevant updates include patches, service packs, hot fixes, and anti-virus signatures. Organizations address flaws discovered during security assessments, continuous monitoring, incident response activities, and system error handling.Organizations can take advantage of available resources such as the Common Weakness Enumeration (CWE) database or Common Vulnerabilities and Exposures (CVE) database in remediating flaws discovered in organizational systems.

Organization-defined time periods for updating security-relevant software and firmware may vary based on a variety of factors including the criticality of the update (i.e., severity of the vulnerability related to the discovered flaw). Some types of flaw remediation may require more testing than other types of remediation. NIST SP 800-40 provides guidance on patch management technologies.

### FURTHER DISCUSSION

All software and firmware have potential flaws. Many vendors work to remedy those flaws by releasing vulnerability information and updates to their software and firmware. Contractors must have a process to review relevant vendor notifications and updates about problems or weaknesses. After reviewing the information, the contractor must implement a patch management process that allows for software and firmware flaws to be fixed without adversely affecting the system functionality. Contractors must define the time frames within which flaws are identified, reported, and corrected for all systems. Contractors should consider purchasing support from their vendors to ensure timely access to updates.

**Example**

You know that software vendors typically release patches, service packs, hot fixes, etc. and want to make sure your software is up to date. You develop a policy that requires checking vendor websites for flaw notifications every week [a]. The policy further requires that those flaws be assessed for severity and patched on end-user computers once each week and servers once each month [c,e]. Consistent with that policy, you configure the system to check for updates weekly or daily depending on the criticality of the software [b,e]. Your team reviews available updates and implements the applicable ones according to the defined schedule [f].

**Potential Assessment Considerations**

* Is the time frame (e.g., a set number of days) within which system flaw identification activities (e.g., vulnerability scans, configuration scans, manual review) must be performed defined and documented [a]?
* Are system flaws (e.g., vulnerabilities, misconfigurations) identified in accordance with the specified time frame [b]?
* Is the time frame (e.g., a set number of days dependent on the assessed severity of a flaw) within which system flaws must be corrected defined and documented [e]?
* Are system flaws (e.g., applied security patches, made configuration changes, or implemented workarounds or mitigations) corrected in accordance with the specified time frame [f]?

### KEY REFERENCES

* FAR Clause 52.204-21 b.1.xii
* NIST SP 800-171 Rev 2 3.14.1