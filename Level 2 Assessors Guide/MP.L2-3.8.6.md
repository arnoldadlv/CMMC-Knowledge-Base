# MP.L2-3.8.6 – Portable Storage Encryption

## Security Requirement Implement cryptographic mechanisms to protect the confidentiality of CUI stored on digital media during transport unless otherwise protected by alternative physical safeguards. |

## Assessment Objectives [a] the confidentiality of CUI stored on digital media is protected during transport using cryptographic mechanisms or alternative physical safeguards. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## MP.L2-3.8.6 – PORTABLE STORAGE ENCRYPTION

### SECURITY REQUIREMENT

Implement cryptographic mechanisms to protect the confidentiality of CUI stored on digital media during transport unless otherwise protected by alternative physical safeguards.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the confidentiality of CUI stored on digital media is protected during transport using cryptographic mechanisms or alternative physical safeguards.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System media protection policy; procedures addressing media transport; system design documentation; system security plan; system configuration settings and associated documentation; system media transport records; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with system media transport responsibilities; personnel with information security responsibilities].

**Test**

[SELECT FROM: Cryptographic mechanisms protecting information on digital media during transportation outside controlled areas].

### DISCUSSION

This requirement applies to portable storage devices (e.g., USB memory sticks, digital video disks, compact disks, external or removable hard disk drives).

NIST SP 800-111 provides guidance on storage encryption technologies for end user devices.

### FURTHER DISCUSSION

CUI can be stored and transported on a variety of portable media, which increases the chance that the CUI can be lost. When identifying the paths CUI flows through your company, identify devices to include in this practice.

To mitigate the risk of losing or exposing CUI, implement an encryption scheme to protect the data. Even if the media are lost, proper encryption renders the data inaccessible. When encryption is not an option, apply alternative physical safeguards during transport.

This practice, MP.L2-3.8.6, provides additional protections to those provided by MP.L2-3.8.5.This practice is intended to protect against situations where control of media access fails, such as through the loss of the media.

**Example**

You manage the backups for file servers in your datacenter. You know that in addition to the company’s sensitive information, CUI is stored on the file servers. As part of a broader plan to protect data, you send the backup tapes off site to a vendor. You are aware that your backup software provides the option to encrypt data onto tape. You develop a plan to test and enable backup encryption for the data sent off site. This encryption provides additional protections for the data on the backup tapes during transport and offsite storage [a].

**Potential Assessment Considerations**

* Are all CUI data on media encrypted or physically protected prior to transport outside of controlled areas [a]?
* Are cryptographic mechanisms used to protect digital media during transport outside of controlled areas [a]?
* Do cryptographic mechanisms comply with FIPS 140-2 [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.8.6