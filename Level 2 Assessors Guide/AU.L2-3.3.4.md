# AU.L2-3.3.4 – Audit Failure Alerting

## Security Requirement Alert in the event of an audit logging process failure. |

## Assessment Objectives [a] personnel or roles to be alerted in the event of an audit logging process failure are identified;  [b] types of audit logging process failures for which alert will be generated are defined; and  [c] identified personnel or roles are alerted in the event of an audit logging process failure. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AU.L2-3.3.4 – AUDIT FAILURE ALERTING

### SECURITY REQUIREMENT

Alert in the event of an audit logging process failure.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] personnel or roles to be alerted in the event of an audit logging process failure are identified;
:   [b] types of audit logging process failures for which alert will be generated are defined; and
:   [c] identified personnel or roles are alerted in the event of an audit logging process failure.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Audit and accountability policy; procedures addressing response to audit logging processing failures; system design documentation; system security plan; system configuration settings and associated documentation; list of personnel to be notified in case of an audit logging processing failure; system incident reports; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with audit and accountability responsibilities; personnel with information security responsibilities; system or network administrators; system developers].

**Test**

[SELECT FROM: Mechanisms implementing system response to audit logging process failures].

### DISCUSSION

Audit logging process failures include software and hardware errors, failures in the audit record capturing mechanisms, and audit record storage capacity being reached or exceeded. This requirement applies to each audit record data storage repository (i.e., distinct system component where audit records are stored), the total audit record storage capacity of organizations (i.e., all audit record data storage repositories combined), or both.

### FURTHER DISCUSSION

Audit logging keeps track of activities occurring on the network, servers, user workstations, and other components of the overall system. These logs must always be available and functional. The company’s designated security personnel (e.g., system administrator and security officer) need to be aware when the audit log process fails or becomes unavailable [a]. Notifications (e.g., email, Short Message Service (SMS)) should to be sent to the company’s designated security personnel to immediately take appropriate action. If security personnel are unaware of the audit logging process failure, then they will be unaware of any suspicious activity occurring at that time. Response to an audit logging process failure should account for the extent of the failure (e.g., a single component’s audit logging versus failure of the centralized logging solution), the risks involved in this loss of audit logging, and other factors (e.g., the possibility that an adversary could have caused the audit logging process failure).

**Example**

You are in charge of IT operations for your company, and your responsibilities include managing the audit logging process. You configure your systems to send you an email in the event of an audit log failure. One day, you receive one of these alerts. You connect to the system, restart logging, and determine why the logging stopped [a,b,c].

**Potential Assessment Considerations**

* Will the system alert personnel with security responsibilities in the event of an audit processing failure?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.3.4