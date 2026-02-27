# MP.L2-3.8.3 – Media Disposal [CUI Data]

## Security Requirement Sanitize or destroy information system media containing Federal Contract Information before disposal or release for reuse. |

## Assessment Objectives [a] system media containing CUI is sanitized or destroyed before disposal; and  [b] system media containing CUI is sanitized before it is released for reuse. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## MP.L2-3.8.3 – MEDIA DISPOSAL

Level 1 Reference: MP.L1-b.1.vii

### SECURITY REQUIREMENT

Sanitize or destroy information system media containing Federal Contract Information before disposal or release for reuse.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] system media containing FCI is sanitized or destroyed before disposal; and
:   [b] system media containing FCI is sanitized before it is released for reuse.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System media protection policy; procedures addressing media sanitization and disposal; applicable standards and policies addressing media sanitization; system security plan; media sanitization records; system audit logs and records; system design documentation; system configuration settings and associated documentation; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with media sanitization responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Organizational processes for media sanitization; mechanisms supporting or implementing media sanitization].

### DISCUSSION

This requirement applies to all system media, digital and non-digital, subject to disposal or reuse. Examples include: digital media found in workstations, network components, scanners, copiers, printers, notebook computers, and mobile devices; and non-digital media such as paper and microfilm. The sanitization process removes information from the media such that the information cannot be retrieved or reconstructed. Sanitization techniques, including clearing, purging, cryptographic erase, and destruction, prevent the disclosure of information to unauthorized individuals when such media is released for reuse or disposal.

Organizations determine the appropriate sanitization methods, recognizing that destruction may be necessary when other methods cannot be applied to the media requiring sanitization. Organizations use discretion on the employment of sanitization techniques and procedures for media containing information that is in the public domain or publicly releasable or deemed to have no adverse impact on organizations or individuals if released for reuse or disposal. Sanitization of non-digital media includes destruction, removing FCI from documents, or redacting selected sections or words from a document by obscuring the redacted sections or words in a manner equivalent in effectiveness to removing the words or sections from the document. NARA policy and guidance control sanitization processes for federal contract information. NIST SP 800-88 provides guidance on media sanitization.

### FURTHER DISCUSSION

“Media” refers to a broad range of items that store information, including paper documents, disks, tapes, digital photography, USB drives, CDs, DVDs, and mobile phones. It is important to know what information is on media so that you can handle it properly. If there is FCI, you or someone in your company should either:

* shred or destroy the device before disposal so it cannot be read; or
* clean or purge the information, if you want to reuse the device.

See NIST Special Publication 800-88, Revision 1, Guidelines for Media Sanitization, for more information.

**Example**

As you pack for an office move, you find some old CDs in a file cabinet. You determine that one has information about an old project your company did for the DoD. You shred the CD rather than simply throwing it in the trash [a].

**Potential Assessment Considerations**

* Is all managed data storage erased, encrypted, or destroyed using mechanisms to ensure that no usable data is retrievable [a,b]?

### KEY REFERENCES

* FAR Clause 52.204-21 b.1.vii
* NIST SP 800-171 Rev 2 3.8.3