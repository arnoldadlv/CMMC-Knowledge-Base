# AU.L2-3.3.9 – Audit Management

## Security Requirement Limit management of audit logging functionality to a subset of privileged users. |

## Assessment Objectives [a] a subset of privileged users granted access to manage audit logging functionality is defined; and  [b] management of audit logging functionality is limited to the defined subset of privileged users. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AU.L2-3.3.9 – AUDIT MANAGEMENT

### SECURITY REQUIREMENT

Limit management of audit logging functionality to a subset of privileged users.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] a subset of privileged users granted access to manage audit logging functionality is defined; and
:   [b] management of audit logging functionality is limited to the defined subset of privileged users.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Audit and accountability policy; access control policy and procedures; procedures addressing protection of audit information; system security plan; system design documentation; system configuration settings and associated documentation; access authorizations; system-generated list of privileged users with access to management of audit logging functionality; access control list; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with audit and accountability responsibilities; personnel with information security responsibilities; system or network administrators; system developers].

**Test**

[SELECT FROM: Mechanisms managing access to audit logging functionality].

### DISCUSSION

Individuals with privileged access to a system and who are also the subject of an audit by that system, may affect the reliability of audit information by inhibiting audit logging activities or modifying audit records. This requirement specifies that privileged access be further defined between audit-related privileges and other privileges, thus limiting the users with audit-related privileges.

### FURTHER DISCUSSION

Companies should restrict access to audit logging functions to a limited number of privileged users who can modify audit logs and audit settings. General users should not be granted permissions to perform audit management. All audit managers should be privileged users, but only a small subset of privileged users will be given audit management responsibilities.

Functions performed by privileged users must be distinctly separate from the functions performed by users who have audit-related responsibilities to reduce the potential of fraudulent activities by privileged users not being detected or reported. When possible, individuals who manage audit logs should not have access to other privileged functions.

**Example**

You are a junior system administrator responsible for the administration of select company infrastructure, but you are not responsible for managing audit information. You are not permitted to review audit logs, delete audit logs, or modify audit log settings [b]. Full control of audit logging functions has been given to senior system administrators [a,b].This separation of system administration duties from audit logging management is necessary to prevent possible log file tampering.

**Potential Assessment Considerations**

* Are audit records of nonlocal accesses to privileged accounts and the execution of privileged functions protected [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.3.9