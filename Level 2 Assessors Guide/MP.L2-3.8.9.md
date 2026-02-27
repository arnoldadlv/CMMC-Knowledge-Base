# MP.L2-3.8.9 – Protect Backups

## Security Requirement Protect the confidentiality of backup CUI at storage locations. |

## Assessment Objectives [a] the confidentiality of backup CUI is protected at storage locations. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## MP.L2-3.8.9 – PROTECT BACKUPS

### SECURITY REQUIREMENT

Protect the confidentiality of backup CUI at storage locations.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the confidentiality of backup CUI is protected at storage locations.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Procedures addressing system backup; system configuration settings and associated documentation; security plan; backup storage locations; system backup logs or records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with system backup responsibilities; personnel with information security responsibilities].

**Test**

[SELECT FROM: Organizational processes for conducting system backups; mechanisms supporting or implementing system backups].

### DISCUSSION

Organizations can employ cryptographic mechanisms or alternative physical controls to protect the confidentiality of backup information at designated storage locations. Backed-up information containing CUI may include system-level information and user-level information. System-level information includes system-state information, operating system software, application software, and licenses. User-level information includes information other than system-level information.

### FURTHER DISCUSSION

You protect CUI to ensure that it remains private (confidentiality) and unchanged (integrity).Methods to ensure confidentiality may include:

* encrypting files or media;
* managing who has access to the information; and
* physically securing devices and media that contain CUI.

Storage locations for information are varied, and may include:

* external hard drives;
* USB drives;
* magnetic media (tape cartridge);
* optical disk (CD, DVD);
* Networked Attached Storage (NAS);
* servers; and
* cloud backup.

This practice, MP.L2-3.8.9, requires the confidentiality of backup information at storage locations.

**Example**

You are in charge of protecting CUI for your company. Because the company’s backups contain CUI, you work with IT to protect the confidentiality of backup data. You agree to encrypt all CUI data as it is saved to an external hard drive [a].

**Potential Assessment Considerations**

* Are data backups encrypted on media before removal from a secured facility [a]?
* Are cryptographic mechanisms FIPS validated [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.8.9