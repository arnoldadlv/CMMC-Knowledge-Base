# AC.L2-3.1.17 – Wireless Access Protection

## Security Requirement Protect wireless access using authentication and encryption. |

## Assessment Objectives [a] wireless access to the system is protected using authentication; and  [b] wireless access to the system is protected using encryption. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.17 – WIRELESS ACCESS PROTECTION

### SECURITY REQUIREMENT

Protect wireless access using authentication and encryption.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] wireless access to the system is protected using authentication; and
:   [b] wireless access to the system is protected using encryption.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; system design documentation; procedures addressing wireless implementation and usage (including restrictions); system security plan; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; system developers].

**Test**

[SELECT FROM: Mechanisms implementing wireless access protections to the system].

### DISCUSSION

Organizations authenticate individuals and devices to help protect wireless access to the system. Special attention is given to the wide variety of devices that are part of the Internet of Things with potential wireless access to organizational systems.

### FURTHER DISCUSSION

Use a combination of authentication and encryption methods to protect the access to wireless networks. Authenticating users to a wireless access point can be achieved in multiple ways. The most common authentication and encryption methods used include:

* WPA2-PSK (WiFi Protected Access-Pre-shared Key) – This method uses a password or passphrase known by the wireless access point and the client (user device). It is common in small companies that have little turnover because the key must be changed each time an employee leaves in order to prevent the terminated employee from connecting to the network without authorization. WPA2 is typically configured to use Advanced Encryption Standard (AES) encryption.
* WPA2 Enterprise – This method may be better for larger companies and enterprise networks because authentication is based on the identity of the individual user or device rather than a shared password or passphrase. It typically requires a Remote Authentication Dial-in User Service (RADIUS) server for authentication and can provide higher security than WPA2-PSK.

Open authentication must not be used because it authenticates any user and lacks security capabilities.

When CMMC requires cryptography, it is to protect the confidentiality of CUI. Federal Information Processing Standard (FIPS)-validated cryptography means the cryptographic module has to have been tested and validated to meet FIPS 140-1 or-2 requirements. Simply using an approved algorithm is not sufficient – the module (software and/or hardware) used to implement the algorithm must be separately validated under FIPS 140. Accordingly, FIPS- validated cryptography is required to meet CMMC practices that protect CUI when transmitted or stored outside the protected environment of the covered contractor information system (including wireless/remote access). Encryption used for other purposes, such as within applications or devices within the protected environment of the covered contractor information system, would not need to be FIPS-validated.

AC.L2-3.1.16, AC.L2-3.1.17, and AC.L2-3.1.18 are complementary practices in that they all establish requirements to control the connection of mobile devices and wireless devices through the use of authentication, authorization, and encryption mechanisms.

**Example 1**

You manage the wireless network at a small company and are installing a new wireless solution. You start by selecting a product that employs encryption validated against the FIPS 140 standard. You configure the wireless solution to use WPA2, requiring users to enter a pre-shared key to connect to the wireless network [a,b].

**Example 2**

You manage the wireless network at a large company and are installing a new wireless solution. You start by selecting a product that employs encryption that is validated against the FIPS 140 standard. Because of the size of your workforce, you configure the wireless system to authenticate users with a RADIUS server. Users must provide the wireless system with their domain usernames and passwords to be able to connect, and the RADIUS server verifies those credentials. Users unable to authenticate are denied access [a,b].

**Potential Assessment Considerations**

* Is wireless access limited only to authenticated and authorized users (e.g., required to supply a username and password) [a]?
* If the organization is securing its wireless network with a pre-shared key, is access to that key restricted to only authorized users [a]?
* Is wireless access encrypted using FIPS-validated cryptography? Note that simply using an approved algorithm is not sufficient; the module (software and/or hardware) used to implement the algorithm must be separately validated under FIPS 140 [b].

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.17