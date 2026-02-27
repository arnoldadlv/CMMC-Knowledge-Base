# SI.L2-3.14.2 – Malicious Code Protection [CUI Data]

## Security Requirement Provide protection from malicious code at appropriate locations within organizational information systems. |

## Assessment Objectives [a] designated locations for malicious code protection are identified; and  [b] protection from malicious code at designated locations is provided. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SI.L2-3.14.2 – MALICIOUS CODE PROTECTION

Level 1 Requirement: SI.L1-b.1.xiii

### SECURITY REQUIREMENT

Provide protection from malicious code at appropriate locations within organizational information systems.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] designated locations for malicious code protection are identified; and
:   [b] protection from malicious code at designated locations is provided.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS [NIST SP 800-171A]

**Examine**

[SELECT FROM: System and information integrity policy; configuration management policy and procedures; procedures addressing malicious code protection; records of malicious code protection updates; malicious code protection mechanisms; system security plan; system configuration settings and associated documentation; record of actions initiated by malicious code protection mechanisms in response to malicious code detection; scan results from malicious code protection mechanisms; system design documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; personnel installing, configuring, and maintaining the system; personnel with responsibility for malicious code protection; personnel with configuration management responsibility].

**Test**

[SELECT FROM: Organizational processes for employing, updating, and configuring malicious code protection mechanisms; organizational process for addressing false positives and resulting potential impact; mechanisms supporting or implementing employing, updating, and configuring malicious code protection mechanisms; mechanisms supporting or implementing malicious code scanning and subsequent actions].

### DISCUSSION

Designated locations include system entry and exit points which may include firewalls, remote access servers, workstations, electronic mail servers, web servers, proxy servers, notebook computers, and mobile devices. Malicious code includes viruses, worms, Trojan horses, and spyware. Malicious code can be encoded in various formats (e.g., UUENCODE, Unicode), contained within compressed or hidden files, or hidden in files using techniques such as steganography. Malicious code can be inserted into systems in a variety of ways including web accesses, electronic mail, electronic mail attachments, and portable storage devices. Malicious code insertions occur through the exploitation of system vulnerabilities. Malicious code protection mechanisms include anti-virus signature definitions and reputation-based technologies. A variety of technologies and methods exist to limit or eliminate the effects of malicious code. Pervasive configuration management and comprehensive software integrity controls may be effective in preventing execution of unauthorized code. In addition to commercial off-the-shelf software, malicious code may also be present in custom-built software. This could include logic bombs, back doors, and other types of cyber-attacks that could affect organizational missions/business functions. Traditional malicious code protection mechanisms cannot always detect such code. In these situations, organizations rely instead on other safeguards including secure coding practices, configuration management and control, trusted procurement processes, and monitoring practices to help ensure that software does not perform functions other than the functions intended. NIST SP 800-83 provides guidance on malware incident prevention.

### FURTHER DISCUSSION

A designated location may be a network device such as a firewall or an end user’s computer. Malicious code, which can be delivered by a range of means (e.g., email, removable media, or websites), includes the following:

* virus – program designed to damage, steal information, change data, send email, show messages, or any combination of these things;
* spyware – program designed to gather information about a person’s activity in secret when they click on a link, usually installed without the person knowing;
* trojan horse – type of malware made to look like legitimate software and used by cyber criminals to get access to a company’s systems; and
* ransomware – type of malware that threatens to publish the contractor’s data or perpetually block access to it unless a ransom is paid.

Use anti-malware tools to stop or lessen the impact of malicious code.

**Example**

You are buying a new computer and want to protect your company’s information from viruses, spyware, etc. You buy and install anti-malware software [a,b].

**Potential Assessment Considerations**

* Are system components (e.g., workstations, servers, email gateways, mobile devices) for which malicious code protection must be provided identified and documented [a]?

### KEY REFERENCES

* FAR Clause 52.204-21 b.1.xiii
* NIST SP 800-171 Rev 2 3.14.2