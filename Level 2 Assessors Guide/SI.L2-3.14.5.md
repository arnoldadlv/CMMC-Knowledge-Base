# SI.L2-3.14.5 – System & File Scanning [CUI Data]

## Security Requirement Perform periodic scans of the information system and real-time scans of files from external sources as files are downloaded, opened, or executed. |

## Assessment Objectives [a] the frequency for malicious code scans is defined;  [b] malicious code scans are performed with the defined frequency; and  [c] real-time malicious code scans of files from external sources as files are downloaded, opened, or executed are performed. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SI.L2-3.14.5 – SYSTEM & FILE SCANNING

Level 1 Requirement: SI.L1-b.1.xv

### SECURITY REQUIREMENT

Perform periodic scans of the information system and real-time scans of files from external sources as files are downloaded, opened, or executed.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the frequency for malicious code scans is defined;
:   [b] malicious code scans are performed with the defined frequency; and
:   [c] real-time malicious code scans of files from external sources as files are downloaded, opened, or executed are performed.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and information integrity policy; configuration management policy and procedures; procedures addressing malicious code protection; malicious code protection mechanisms; records of malicious code protection updates; system security plan; system design documentation; system configuration settings and associated documentation; scan results from malicious code protection mechanisms; record of actions initiated by malicious code protection mechanisms in response to malicious code detection; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; personnel installing, configuring, and maintaining the system; personnel with responsibility for malicious code protection; personnel with configuration management responsibility].

**Test**
[SELECT FROM: Organizational processes for employing, updating, and configuring malicious code protection mechanisms; organizational process for addressing false positives and resulting potential impact; mechanisms supporting or implementing malicious code protection mechanisms (including updates and configurations); mechanisms supporting or implementing malicious code scanning and subsequent actions].

### DISCUSSION

Periodic scans of organizational systems and real-time scans of files from external sources can detect malicious code. Malicious code can be encoded in various formats (e.g., UUENCODE, Unicode), contained within compressed or hidden files, or hidden in files using techniques such as steganography. Malicious code can be inserted into systems in a variety of ways including web accesses, electronic mail, electronic mail attachments, and portable storage devices. Malicious code insertions occur through the exploitation of system vulnerabilities.

### FURTHER DISCUSSION

Use anti-malware software to scan for and identify viruses in your computer systems and determine how often scans are conducted. Real-time scans look at the system whenever new files are downloaded, opened, and saved. Periodic scans check previously saved files against updated malware information.

**Example**

You work with your company’s email provider to enable enhanced protections that will scan all attachments to identify and quarantine those that may be harmful prior to a user opening them [c].In addition, you configure antivirus software on each computer to scan for malicious code every day [a,b]. The software also scans files that are downloaded or copied from removable media such as USB drives. It quarantines any suspicious files and notifies the security team [c].

**Potential Assessment Considerations**

* Are files from media (e.g., USB drives, CD-ROM) included in the definition of external sources and are they being scanned [c]?

### KEY REFERENCES

* FAR Clause 52.204-21 b.1.xv
* NIST SP 800-171 Rev 2 3.14.5