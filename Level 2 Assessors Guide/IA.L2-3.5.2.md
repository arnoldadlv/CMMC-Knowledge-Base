# IA.L2-3.5.2 – Authentication [CUI Data]

## Security Requirement Authenticate (or verify) the identities of those users, processes, or devices, as a prerequisite to allowing access to organizational information systems. |

## Assessment Objectives [a] the identity of each user is authenticated or verified as a prerequisite to system access;  [b] the identity of each process acting on behalf of a user is authenticated or verified as a prerequisite to system access; and  [c] the identity of each device accessing or connecting to the system is authenticated or verified as a prerequisite to system access. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## IA.L2-3.5.2 – AUTHENTICATION

Level 1 Reference: IA.L1-b.1.vi

### SECURITY REQUIREMENT

Authenticate (or verify) the identities of those users, processes, or devices, as a prerequisite to allowing access to organizational information systems.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the identity of each user is authenticated or verified as a prerequisite to system access;
:   [b] the identity of each process acting on behalf of a user is authenticated or verified as a prerequisite to system access; and
:   [c] the identity of each device accessing or connecting to the system is authenticated or verified as a prerequisite to system access.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Identification and authentication policy; system security plan; procedures addressing authenticator management; procedures addressing user identification and authentication; system design documentation; list of system authenticator types; system configuration settings and associated documentation; change control records associated with managing system authenticators; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with authenticator management responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Mechanisms supporting or implementing authenticator management capability].

### DISCUSSION

Individual authenticators include the following: passwords, key cards, cryptographic devices, and one-time password devices. Initial authenticator content is the actual content of the authenticator, for example, the initial password. In contrast, the requirements about authenticator content include the minimum password length. Developers ship system components with factory default authentication credentials to allow for initial installation and configuration. Default authentication credentials are often well known, easily discoverable, and present a significant security risk.

Systems support authenticator management by organization-defined settings and restrictions for various authenticator characteristics including minimum password length, validation time window for time synchronous one-time tokens, and number of allowed rejections during the verification stage of biometric authentication. Authenticator management includes issuing and revoking, when no longer needed, authenticators for temporary access such as that required for remote maintenance. Device authenticators include certificates and passwords.

NIST SP 800-63-3 provides guidance on digital identities.

### FURTHER DISCUSSION

Before you let a person or a device have access to your system, verify that the user or device is who or what it claims to be. This verification is called authentication. The most common way to verify identity is using a username and a hard-to-guess password.
Some devices ship with default usernames and passwords. For example, some devices ship so that when you first log on to the device, the username is “admin” and the password is “admin”. When you have devices with this type of default username and password, immediately change the default password to a unique password you create. Default passwords may be well known to the public, easily found in a search, or easy to guess, allowing an unauthorized person to access your system.

**Example 1**

You are in charge of purchasing. You know that some laptops come with a default username and password. You notify IT that all default passwords should be reset prior to laptop use [a]. You ask IT to explain the importance of resetting default passwords and convey how easily they are discovered using internet searches during next week’s cybersecurity awareness training.

**Example 2**

Your company decides to use cloud services for email and other capabilities. Upon reviewing this practice, you realize every user or device that connects to the cloud service must be authenticated. As a result, you work with your cloud service provider to ensure that only properly authenticated users and devices are allowed to connect to the system [a,c].

**Potential Assessment Considerations**

* Are unique authenticators used to verify user identities (e.g., passwords) [a]?
* An example of a process acting on behalf of users could be a script that logs in as a person or service account [b]. Can the contractor show that it maintains a record of all of those service accounts for use when reviewing log data or responding to an incident?
* Are user credentials authenticated in system processes (e.g., credentials binding, certificates, tokens) [b]?
* Are device identifiers used in authentication processes (e.g., MAC address, non-anonymous computer name, certificates) [c]?

### KEY REFERENCES

* FAR Clause 52.204-21 b.1.vi
* NIST SP 800-171 Rev 2 3.5.2