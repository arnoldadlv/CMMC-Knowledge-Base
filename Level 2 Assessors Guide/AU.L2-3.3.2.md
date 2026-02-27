# AU.L2-3.3.2 – User Accountability

## Security Requirement Ensure that the actions of individual system users can be uniquely traced to those users so they can be held accountable for their actions. |

## Assessment Objectives [a] the content of the audit records needed to support the ability to uniquely trace users to their actions is defined; and  [b] audit records, once created, contain the defined content. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AU.L2-3.3.2 – USER ACCOUNTABILITY

### SECURITY REQUIREMENT

Ensure that the actions of individual system users can be uniquely traced to those users so they can be held accountable for their actions.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the content of the audit records needed to support the ability to uniquely trace users to their actions is defined; and
:   [b] audit records, once created, contain the defined content.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Audit and accountability policy; procedures addressing audit records and event types; system security plan; system design documentation; system configuration settings and associated documentation; procedures addressing audit record generation; procedures addressing audit review, analysis, and reporting; reports of audit findings; system audit logs and records; system events; system incident reports; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with audit and accountability responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Mechanisms implementing system audit logging].

### DISCUSSION

This requirement ensures that the contents of the audit record include the information needed to link the audit event to the actions of an individual to the extent feasible. Organizations consider logging for traceability including results from monitoring of account usage, remote access, wireless connectivity, mobile device connection, communications at system boundaries, configuration settings, physical access, nonlocal maintenance, use of maintenance tools, temperature and humidity, equipment delivery and removal, system component inventory, use of mobile code, and use of VoIP.

### FURTHER DISCUSSION

Capturing the necessary information in audit logs ensures that you can trace actions to a specific user. This may include capturing user IDs, source and destination addresses, and time stamps. Logging from networks, servers, clients, and applications should be considered in ensuring accountability.

This practice, AU.L2-3.3.2, which ensures logging and traceability of user actions, supports the control of non-privileged users required by AC.L2-3.1.7 as well as many other auditing, configuration management, incident response, and situation awareness practices.

**Example**

You are a system administrator. You want to ensure that you can trace all remote access sessions to a specific user. You configure the VPN device to capture the following information for all remote access connections: source and destination IP address, user ID, machine name, time stamp, and user actions during the remote session [b].

**Potential Assessment Considerations**

* Are users uniquely traced and held responsible for unauthorized actions [a]?
* Does the system protect against an individual denying having performed an action (non-repudiation) [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.3.2