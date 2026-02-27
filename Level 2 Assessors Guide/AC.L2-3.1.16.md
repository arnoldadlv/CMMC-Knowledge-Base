# AC.L2-3.1.16 – Wireless Access Authorization

## Security Requirement Authorize wireless access prior to allowing such connections. |

## Assessment Objectives [a] wireless access points are identified; and  [b] wireless access is authorized prior to allowing such connections. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.16 – WIRELESS ACCESS AUTHORIZATION

### SECURITY REQUIREMENT

Authorize wireless access prior to allowing such connections.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] wireless access points are identified; and
:   [b] wireless access is authorized prior to allowing such connections.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; configuration management plan; procedures addressing wireless access implementation and usage (including restrictions);system security plan; system design documentation; system configuration settings and associated documentation; wireless access authorizations; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with responsibilities for managing wireless access connections; personnel with information security responsibilities].

**Test**

[SELECT FROM: Wireless access management capability for the system].

### DISCUSSION

Establishing usage restrictions and configuration/connection requirements for wireless access to the system provides criteria for organizations to support wireless access authorization decisions. Such restrictions and requirements reduce the susceptibility to unauthorized access to the system through wireless technologies. Wireless networks use authentication protocols that provide credential protection and mutual authentication.

### FURTHER DISCUSSION

Guidelines from management form the basis for the requirements that must be met prior to authorizing a wireless connection. These guidelines may include the following:

* types of devices, such as corporate or privately owned equipment;
* configuration requirements of the devices; and
* authorization requirements before granting such connections.

AC.L2-3.1.16, AC.L2-3.1.17, and AC.L2-3.1.18 are complementary practices in that they all establish requirements to control the connection of mobile devices and wireless devices through the use of authentication, authorization, and encryption mechanisms.

**Example**

Your company is implementing a wireless network at its headquarters. You work with management to draft a policy about the use of the wireless network. The policy states that only company-approved devices that contain verified security configuration settings are allowed to connect. The policy also includes usage restrictions that must be followed for anyone who wants to use the wireless network. Authorization is required before devices are allowed to connect to the wireless network [b].

**Potential Assessment Considerations**

* Is an updated list of approved network devices providing wireless access to the system maintained [a]?
* Are network devices providing wireless access configured to require users or devices be authorized prior to permitting a wireless connection [b]?
* Is wireless access to the system authorized and managed [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.16