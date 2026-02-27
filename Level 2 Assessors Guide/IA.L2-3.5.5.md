# IA.L2-3.5.5 – Identifier Reuse

## Security Requirement Prevent reuse of identifiers for a defined period. |

## Assessment Objectives [a] a period within which identifiers cannot be reused is defined; and  [b] reuse of identifiers is prevented within the defined period. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## IA.L2-3.5.5 – IDENTIFIER REUSE

### SECURITY REQUIREMENT

Prevent reuse of identifiers for a defined period.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] a period within which identifiers cannot be reused is defined; and
:   [b] reuse of identifiers is prevented within the defined period.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Identification and authentication policy; system security plan; procedures addressing authenticator management; procedures addressing user identification and authentication; system design documentation; list of system authenticator types; system configuration settings and associated documentation; change control records associated with managing system authenticators; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with authenticator management responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Mechanisms supporting or implementing authenticator management capability].

### DISCUSSION

Identifiers are provided for users, processes acting on behalf of users, or devices (IA.L1- 3.5.1). Preventing reuse of identifiers implies preventing the assignment of previously used individual, group, role, or device identifiers to different individuals, groups, roles, or devices.

### FURTHER DISCUSSION

Identifiers uniquely associate a user ID to an individual, group, role, or device. Establish guidelines and implement mechanisms to prevent identifiers from being reused for the period of time established in the policy.

**Example**

As a system administrator, you maintain a central directory/domain that holds the accounts for users, computers, and network devices. As part of your job, you issue unique usernames (e.g., riley@acme.com) for the staff to access resources. When you issue staff computers you also rename the computer to reflect to whom it is assigned (e.g., riley-laptop01). Riley has recently left the organization, so you must manage the former staff member’s account. Incidentally, their replacement is also named Riley. In the directory, you do not assign the previous account to the new user, as policy has defined an identifier reuse period of 24 months [a]. In accordance with policy, you create an account called riley02 [b]. This account is assigned the appropriate permissions for the new user. A new laptop is also provided with the identifier of riley02-laptop01.

### Potential Assessment Considerations

* Are accounts uniquely assigned to employees, contractors, and subcontractors [b]?
* Are account identifiers reused [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.5.5