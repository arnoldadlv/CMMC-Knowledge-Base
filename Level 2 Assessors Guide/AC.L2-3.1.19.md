# AC.L2-3.1.19 – Encrypt CUI on Mobile

## Security Requirement Encrypt CUI on mobile devices and mobile computing platforms. |

## Assessment Objectives [a] mobile devices and mobile computing platforms that process, store, or transmit CUI are identified; and  [b] encryption is employed to protect CUI on identified mobile devices and mobile computing platforms. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.19 – ENCRYPT CUI ON MOBILE

### SECURITY REQUIREMENT

Encrypt CUI on mobile devices and mobile computing platforms.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] mobile devices and mobile computing platforms that process, store, or transmit CUI are identified; and
:   [b] encryption is employed to protect CUI on identified mobile devices and mobile computing platforms.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; procedures addressing access control for mobile devices; system design documentation; system configuration settings and associated documentation; encryption mechanisms and associated configuration documentation; system security plan; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with access control responsibilities for mobile devices; system or network administrators; personnel with information security responsibilities].

**Test**

[SELECT FROM: Encryption mechanisms protecting confidentiality of information on mobile devices].

### DISCUSSION

Organizations can employ full-device encryption or container-based encryption to protect the confidentiality of CUI on mobile devices and computing platforms. Container-based encryption provides a more fine-grained approach to the encryption of data and information including encrypting selected data structures such as files, records, or fields.

### FURTHER DISCUSSION

Ensure CUI is encrypted on all mobile devices and mobile computing platforms that process, store, or transmit CUI including smartphones, tablets, and e-readers.

When CMMC requires cryptography, it is to protect the confidentiality of CUI. FIPS-validated cryptography means the cryptographic module has to have been tested and validated to meet FIPS 140-1 or-2 requirements. Simply using an approved algorithm is not sufficient – the module (software and/or hardware) used to implement the algorithm must be separately validated under FIPS 140. Accordingly, FIPS-validated cryptography is required to meet CMMC practices that protect CUI when transmitted or stored outside the protected environment of the covered contractor information system (including wireless/remote access). Encryption used for other purposes, such as within applications or devices within the protected environment of the covered contractor information system, would not need to be FIPS-validated.

This practice, AC.L2-3.1.19, requires that CUI be encrypted on mobile devices and extends three other CUI protection practices (MP.L2-3.8.1, MP.L2-3.8.2, and SC.L2-3.13.16):

* MP.L2-3.8.1 requires that media containing CUI be protected.
* MP.L2-3.8.2 limits access to CUI to authorized users.
* Finally, SC.L2-3.13.16 requires confidentiality of CUI at rest.

This practice, AC.L2-3.1.19, also leverages SC.L2-3.13.11, which specifies that the algorithms used must be FIPS-validated, and SC.L2-3.13.10, which specifies that any cryptographic keys in use must be protected.

**Example**

You are in charge of mobile device security. You configure all laptops to use the full-disk encryption technology built into the operating system. This approach is FIPS-validated and encrypts all files, folders, and volumes.

Phones and tablets pose a greater technical challenge with their wide range of manufacturers and operating systems. You select a proprietary mobile device management (MDM) solution to enforce FIPS-validated encryption on those devices [a,b].

**Potential Assessment Considerations**

* Is a list maintained of mobile devices and mobile computing platforms that are permitted to process, store, or transmit CUI [a]?
* Is CUI encrypted on mobile devices using FIPS-validated algorithms [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.19