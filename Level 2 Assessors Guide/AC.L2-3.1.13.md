# AC.L2-3.1.13 – Remote Access Confidentiality

## Security Requirement Employ cryptographic mechanisms to protect the confidentiality of remote access sessions. |

## Assessment Objectives [a] cryptographic mechanisms to protect the confidentiality of remote access sessions are identified; and  [b] cryptographic mechanisms to protect the confidentiality of remote access sessions are implemented. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.13 – REMOTE ACCESS CONFIDENTIALITY

### SECURITY REQUIREMENT

Employ cryptographic mechanisms to protect the confidentiality of remote access sessions.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] cryptographic mechanisms to protect the confidentiality of remote access sessions are identified; and
:   [b] cryptographic mechanisms to protect the confidentiality of remote access sessions are implemented.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; procedures addressing remote access to the system; system security plan; system design documentation; system configuration settings and associated documentation; cryptographic mechanisms and associated configuration documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; system developers].

**Test**

[SELECT FROM: Cryptographic mechanisms protecting remote access sessions].

### DISCUSSION

Cryptographic standards include FIPS-validated cryptography and NSA-approved cryptography.

### FURTHER DISCUSSION

A remote access session involves logging into the organization’s systems such as its internal network or a cloud service provider from a remote location such as home or an alternate work site. This remote access session must be secured using FIPS-validated cryptography to provide confidentiality and prevent anyone from deciphering session information exchanges.

When CMMC requires cryptography, it is to protect the confidentiality of CUI. FIPS-validated cryptography means the cryptographic module has to have been tested and validated to meet FIPS 140-1 or -2 requirements. Simply using an approved algorithm is not sufficient – the module (software and/or hardware) used to implement the algorithm must be separately validated under FIPS 140. Accordingly, FIPS-validated cryptography is required to meet CMMC practices that protect CUI when transmitted or stored outside the protected environment of the covered contractor information system (including wireless/remote access). Encryption used for other purposes, such as within applications or devices within the protected environment of the covered contractor information system, would not need to be FIPS-validated. This practice, AC.L2-3.1.13, requires the use of cryptographic mechanisms when enabling remote sessions and complements five other practices dealing with remote access (AC.L2-3.1.12, AC.L2-3.1.14, AC.L2-3.1.15, IA.L2-3.5.3, and MA.L2-3.7.5):

* AC.L2-3.1.12 requires the control of remote access sessions.
* AC.L2-3.1.14 limits remote access to specific access control points.
* AC.L2-3.1.15 requires authorization for privileged commands executed during a remote session.
* IA.L2-3.5.3 requires multifactor authentication for network access to non-privileged accounts.
* Finally, MA.L2-3.7.5 requires the addition of multifactor authentication for remote maintenance sessions.

**Example**

As a system administrator you are responsible for implementing a remote network access capability for users who work offsite. In order to provide session confidentiality, you decide to implement a VPN mechanism and select a product that has completed FIPS 140 validation [a,b].

**Potential Assessment Considerations**

* Are cryptographic mechanisms used for remote access sessions (e.g., Transport Layer Security (TLS) and Internet Protocol Security (IPSec) using FIPS-validated encryption algorithms) defined and implemented [a,b]? Note that simply using an approved algorithm is not sufficient – the module (software and/or hardware) used to implement the algorithm must be separately validated under FIPS 140.

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.13