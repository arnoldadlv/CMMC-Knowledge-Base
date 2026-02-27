# IA.L2-3.5.1 – Identification [CUI Data]

## Security Requirement Identify information system users, processes acting on behalf of users, or devices. |

## Assessment Objectives [a] system users are identified;  [b] processes acting on behalf of users are identified; and  [c] devices accessing the system are identified. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## IA.L2-3.5.1 – IDENTIFICATION

Level 1 Reference: IA.L1-b.1.v

### SECURITY REQUIREMENT

Identify information system users, processes acting on behalf of users, or devices.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] system users are identified;
:   [b] processes acting on behalf of users are identified; and
:   [c] devices accessing the system are identified.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Identification and authentication policy; procedures addressing user identification and authentication; system security plan, system design documentation; system configuration settings and associated documentation; system audit logs and records; list of system accounts; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with system operations responsibilities; personnel with information security responsibilities; system or network administrators; personnel with account management responsibilities; system developers].

**Test**

[SELECT FROM: Organizational processes for uniquely identifying and authenticating users; mechanisms supporting or implementing identification and authentication capability].

### DISCUSSION

Common device identifiers include media access control (MAC), Internet Protocol (IP) addresses, or device-unique token identifiers. Management of individual identifiers is not applicable to shared system accounts. Typically, individual identifiers are the user names associated with the system accounts assigned to those individuals. Organizations may require unique identification of individuals in group accounts or for detailed accountability of individual activity. In addition, this requirement addresses individual identifiers that are not necessarily associated with system accounts. Organizational devices requiring identification may be defined by type, by device, or by a combination of type/device. NIST SP 800-63-3 provides guidance on digital identities.

### FURTHER DISCUSSION

Make sure to assign individual, unique identifiers (e.g., user names) to all users and processes that access company systems. Authorized devices also should have unique identifiers. Unique identifiers can be as simple as a short set of alphanumeric characters (e.g., SW001 could refer to a network switch, SW002 could refer to a different network switch).

This practice, IA.L1-3.5.1, provides a vetted and trusted identity that supports the access control mechanism required by AC.L1-3.1.1.

**Example**

You want to make sure that all employees working on a project can access important information about it. Because this is work for the DoD and may contain FCI, you also need to prevent employees who are not working on that project from being able to access the information. You assign each employee is assigned a unique user ID, which they use to log into the system [a].

**Potential Assessment Considerations**

* Are unique identifiers issued to individual users (e.g., usernames) [a]?
* Are the processes and service accounts that an authorized user initiates identified (e.g., scripts, automatic updates, configuration updates, vulnerability scans) [b]?
* Are unique device identifiers used for devices that access the system identified [c]?

### KEY REFERENCES

* FAR Clause 52.204-21 b.1.v
* NIST SP 800-171 Rev 2 3.5.1