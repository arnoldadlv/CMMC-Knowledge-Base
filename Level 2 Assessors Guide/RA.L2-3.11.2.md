# RA.L2-3.11.2 – Vulnerability Scan

## Security Requirement Scan for vulnerabilities in organizational systems and applications periodically and when new vulnerabilities affecting those systems and applications are identified. |

## Assessment Objectives [a] the frequency to scan for vulnerabilities in organizational systems and applications is defined;  [b] vulnerability scans are performed on organizational systems with the defined frequency;  [c] vulnerability scans are performed on applications with the defined frequency;  [d] vulnerability scans are performed on organizational systems when new vulnerabilities are identified; and  [e] vulnerability scans are performed on applications when new vulnerabilities are  identified. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## RA.L2-3.11.2 – VULNERABILITY SCAN

### SECURITY REQUIREMENT

Scan for vulnerabilities in organizational systems and applications periodically and when new vulnerabilities affecting those systems and applications are identified.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the frequency to scan for vulnerabilities in organizational systems and applications is defined;
:   [b] vulnerability scans are performed on organizational systems with the defined frequency;
:   [c] vulnerability scans are performed on applications with the defined frequency;
:   [d] vulnerability scans are performed on organizational systems when new vulnerabilities are identified; and
:   [e] vulnerability scans are performed on applications when new vulnerabilities are identified.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Risk assessment policy; procedures addressing vulnerability scanning; risk assessment; system security plan; security assessment report; vulnerability scanning tools and associated configuration documentation; vulnerability scanning results; patch and vulnerability management records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with risk assessment, security assessment and vulnerability scanning responsibilities; personnel with vulnerability scan analysis and remediation responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Organizational processes for vulnerability scanning, analysis, remediation, and information sharing; mechanisms supporting or implementing vulnerability scanning, analysis, remediation, and information sharing].

### DISCUSSION

Organizations determine the required vulnerability scanning for all system components, ensuring that potential sources of vulnerabilities such as networked printers, scanners, and copiers are not overlooked. The vulnerabilities to be scanned are readily updated as new vulnerabilities are discovered, announced, and scanning methods developed. This process ensures that potential vulnerabilities in the system are identified and addressed as quickly as possible. Vulnerability analyses for custom software applications may require additional approaches such as static analysis, dynamic analysis, binary analysis, or a hybrid of the three approaches. Organizations can employ these analysis approaches in source code reviews and in a variety of tools (e.g., static analysis tools, web-based application scanners, binary analyzers). Vulnerability scanning includes: scanning for patch levels; scanning for functions, ports, protocols, and services that should not be accessible to users or devices; and scanning for improperly configured or incorrectly operating information flow control mechanisms.

To facilitate interoperability, organizations consider using products that are Security Content Automated Protocol (SCAP)-validated, scanning tools that express vulnerabilities in the Common Vulnerabilities and Exposures (CVE) naming convention, and that employ the Open Vulnerability Assessment Language (OVAL) to determine the presence of system vulnerabilities. Sources for vulnerability information include the Common Weakness Enumeration (CWE) listing and the National Vulnerability Database (NVD).

Security assessments, such as red team exercises, provide additional sources of potential vulnerabilities for which to scan. Organizations also consider using scanning tools that express vulnerability impact by the Common Vulnerability Scoring System (CVSS). In certain situations, the nature of the vulnerability scanning may be more intrusive or the system component that is the subject of the scanning may contain highly sensitive information. Privileged access authorization to selected system components facilitates thorough vulnerability scanning and protects the sensitive nature of such scanning.

NIST SP 800-40 provides guidance on vulnerability management.

### FURTHER DISCUSSION

A vulnerability scanner is an application that identifies vulnerabilities in organizational assets. Most scanners can create a prioritized list of vulnerabilities ordered by their level of severity. Scan for vulnerabilities on all devices connected to the network including servers, desktops, laptops, virtual machines, containers, firewalls, switches, and printers. All assets that are within the scope of the CMMC assessment must be scanned, including assets such as laptop computers that may not routinely connect to an organization’s network.

Perform reviews of your organization’s custom-developed software. Vulnerability analysis of a custom-made solution may require a penetration tester to properly test and validate findings. Automated vulnerability scanners may not be as thorough when scanning custom developed applications. Source code scanners can help identify weaknesses and vulnerabilities within code prior to compilation and use.

The vulnerability scanning process is a regular activity, not a single occurrence. Organizations put in place a vulnerability scanner that updates its database each time it performs a scan so it can identify the most current known vulnerabilities. Schedule scans with consideration of the potential for impact to normal operations and use caution when scanning critical assets.

This practice, RA.L2-3.11.2, which ensures scanning for vulnerabilities in organizational systems and application, is a baseline Risk Assessment practice. RA.L2-3.11.2 ,contributes to performing risk assessments as described in RA.L2-3.11.1.

**Example**

You are a system administrator. Your organization has assessed its risk and determined that it needs to scan for vulnerabilities in systems and applications once each quarter [a]. You conduct some tests and decide that it is important to be able to schedule scans after standard business hours. You also realize that you have remote workers and that you will need to be sure to scan their remote computers as well [b]. After some final tests, you integrate the scans into normal IT operations, running as scheduled [b,c]. You verify that the scanner application receives the latest updates on vulnerabilities and that those are included in future scans [d,e].

**Potential Assessment Considerations**

* Is the frequency specified for vulnerability scans to be performed in organizational systems and applications (e.g., continuous passive scanning, scheduled active scans) [a]?
* Are vulnerability scans performed on a defined frequency or randomly in accordance with company policy [a,b,c]?
* Are systems periodically scanned for common and new vulnerabilities [d,e]?64
* Is the list of scanned system vulnerabilities updated on a defined frequency or when new vulnerabilities are identified and reported [d,e]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.11.2