# AU.L2-3.3.8 – Audit Protection

## Security Requirement Protect audit information and audit logging tools from unauthorized access, modification, and deletion. |

## Assessment Objectives [a] audit information is protected from unauthorized access;  [b] audit information is protected from unauthorized modification;  [c] audit information is protected from unauthorized deletion;  [d] audit logging tools are protected from unauthorized access;  [e] audit logging tools are protected from unauthorized modification; and  [f] audit logging tools are protected from unauthorized deletion. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AU.L2-3.3.8 – AUDIT PROTECTION

### SECURITY REQUIREMENT

Protect audit information and audit logging tools from unauthorized access, modification, and deletion.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] audit information is protected from unauthorized access;
:   [b] audit information is protected from unauthorized modification;
:   [c] audit information is protected from unauthorized deletion;
:   [d] audit logging tools are protected from unauthorized access;
:   [e] audit logging tools are protected from unauthorized modification; and
:   [f] audit logging tools are protected from unauthorized deletion.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Audit and accountability policy; access control policy and procedures; procedures addressing protection of audit information; system security plan; system design documentation; system configuration settings and associated documentation, system audit logs and records; audit logging tools; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with audit and accountability responsibilities; personnel with information security responsibilities; system or network administrators; system developers].

**Test**

[SELECT FROM: Mechanisms implementing audit information protection].

### DISCUSSION

Audit information includes all information (e.g., audit records, audit log settings, and audit reports) needed to successfully audit system activity. Audit logging tools are those programs and devices used to conduct audit and logging activities. This requirement focuses on the technical protection of audit information and limits the ability to access and execute audit logging tools to authorized individuals. Physical protection of audit information is addressed by media protection and physical and environmental protection requirements.

### FURTHER DISCUSSION

Audit information is a critical record of what events occurred, the source of the events, and the outcomes of the events; this information needs to be protected. The logs must be properly secured so that the information may not be modified or deleted, either intentionally or unintentionally. Only those with a legitimate need-to-know should have access to audit information, whether that information is being accessed directly from logs or from audit tools.

**Example**

You are in charge of IT operations in your company. Your responsibilities include protecting audit information and audit logging tools. You protect the information from modification or deletion by having audit log events forwarded to a central server and by restricting the local audit logs to only be viewable by the system administrators [a,b,c]. Only a small group of security professionals can view the data on the central audit server [b,c,d]. For an additional layer of protection, you back up the server daily and encrypt the backups before sending them to a cloud data repository [a,b,c].

**Potential Assessment Considerations**

* Is there a list of authorized users for audit systems and tools [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.3.8