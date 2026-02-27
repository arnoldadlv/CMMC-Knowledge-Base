# AU.L2-3.3.3 – Event Review

## Security Requirement Review and update logged events. |

## Assessment Objectives [a] a process for determining when to review logged events is defined;  [b] event types being logged are reviewed in accordance with the defined review process; and  [c] event types being logged are updated based on the review. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AU.L2-3.3.3 – EVENT REVIEW

### SECURITY REQUIREMENT

Review and update logged events.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] a process for determining when to review logged events is defined;
:   [b] event types being logged are reviewed in accordance with the defined review process; and
:   [c] event types being logged are updated based on the review.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Audit and accountability policy; procedures addressing audit records and event types; system security plan; list of organization-defined event types to be logged; reviewed and updated records of logged event types; system audit logs and records; system incident reports; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with audit and accountability responsibilities; personnel with information security responsibilities].

**Test**

[SELECT FROM: Mechanisms supporting review and update of logged event types].

### DISCUSSION

The intent of this requirement is to periodically re-evaluate which logged events will continue to be included in the list of events to be logged. The event types that are logged by organizations may change over time. Reviewing and updating the set of logged event types periodically is necessary to ensure that the current set remains necessary and sufficient.

### FURTHER DISCUSSION

This practice is focused on the configuration of the auditing system, not the review of the audit records produced by the selected events. The review of the audit logs is covered under AU.L2-3.3.5 and AU.L2-3.3.6.

**Example**

You are in charge of IT operations for your company and are responsible for identifying and documenting which events are relevant to the security of your company’s systems. Your company has decided that this list of events should be updated annually or when new security threats or events have been identified, which may require additional events to be logged and reviewed [a]. The list of events you are capturing in your logs started as the list of recommended events given by the manufacturers of your operating systems and devices, but it has grown from experience.

Your company experiences a security incident, and a forensics review shows the logs appear to have been deleted by a remote user. You notice that remote sessions are not currently being logged [b]. You update the list of events to include logging all VPN sessions [c].

**Potential Assessment Considerations**

* Do documented processes include methods for determining when to review logged event types (i.e., regular frequency, after incidents, after major system changes) [a]?
* Do documented processes include methods for reviewing event types being logged (i.e., based on specific threat, use case, retention capacity, current utilization, and/or newly added system component or functionality) [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.3.3