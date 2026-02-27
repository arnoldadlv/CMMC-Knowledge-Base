# AC.L2-3.1.2 – Transaction & Function Control [CUI Data]

## Security Requirement Limit information system access to the types of transactions and functions that authorized users are permitted to execute. |

## Assessment Objectives [a] the types of transactions and functions that authorized users are permitted to execute are defined; and  [b] system access is limited to the defined types of transactions and functions for authorized users. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.2 – TRANSACTION & FUNCTION CONTROL

Level 1 Reference: AC.L1-b.1.ii

### SECURITY REQUIREMENT

Limit information system access to the types of transactions and functions that authorized users are permitted to execute.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the types of transactions and functions that authorized users are permitted to execute are defined; and
:   [b] system access is limited to the defined types of transactions and functions for authorized users.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; procedures addressing access enforcement; system security plan; system design documentation; list of approved authorizations including remote access authorizations; system audit logs and records; system configuration settings and associated documentation; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with access enforcement responsibilities; system or network administrators; personnel with information security responsibilities; system developers].

**Test**

[SELECT FROM: Mechanisms implementing access control policy].

### DISCUSSION

Organizations may choose to define access privileges or other attributes by account, by type of account, or a combination of both. System account types include individual, shared, group, system, anonymous, guest, emergency, developer, manufacturer, vendor, and temporary. Other attributes required for authorizing access include restrictions on time-of-day, day-of- week, and point-of-origin. In defining other account attributes, organizations consider system-related requirements (e.g., system upgrades scheduled maintenance,) and mission or business requirements, (e.g., time zone differences, customer requirements, remote access to support travel requirements).

### FURTHER DISCUSSION

Limit users to only the information systems, roles, or applications they are permitted to use and are needed for their roles and responsibilities. Limit access to applications and data based on the authorized users’ roles and responsibilities. Common types of functions a user can be assigned are create, read, update, and delete.

**Example**

You supervise the team that manages DoD contracts for your company. Members of your team need to access the contract information to perform their work properly. Because some of that data contains FCI, you work with IT to set up your group’s systems so that users can be assigned access based on their specific roles [a]. Each role limits whether an employee has read-access or create/read/delete/update -access [b]. Implementing this access control restricts access to FCI information unless specifically authorized.

**Potential Assessment Considerations**

* Are access control lists used to limit access to applications and data based on role and/or identity [a]?
* Is access for authorized users restricted to those parts of the system they are explicitly permitted to use (e.g., a person who only performs word-processing cannot access developer tools) [b]?

### KEY REFERENCES

* FAR Clause 52.204-21 b.1.ii
* NIST SP 800-171 Rev 2 3.1.2