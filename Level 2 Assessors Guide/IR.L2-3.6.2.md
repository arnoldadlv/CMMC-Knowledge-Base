# IR.L2-3.6.2 – Incident Reporting

## Security Requirement Track, document, and report incidents to designated officials and/or authorities both internal and external to the organization. |

## Assessment Objectives [a] incidents are tracked;  [b] incidents are documented;  [c] authorities to whom incidents are to be reported are identified;  [d] organizational officials to whom incidents are to be reported are identified;  [e] identified authorities are notified of incidents; and  [f] identified organizational officials are notified of incidents. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## IR.L2-3.6.2 – INCIDENT REPORTING

### SECURITY REQUIREMENT

Track, document, and report incidents to designated officials and/or authorities both internal and external to the organization.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] incidents are tracked;
:   [b] incidents are documented;
:   [c] authorities to whom incidents are to be reported are identified;
:   [d] organizational officials to whom incidents are to be reported are identified;
:   [e] identified authorities are notified of incidents; and
:   [f] identified organizational officials are notified of incidents.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Incident response policy; procedures addressing incident monitoring; incident response records and documentation; procedures addressing incident reporting; incident reporting records and documentation; incident response plan; system security plan; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with incident monitoring responsibilities; personnel with incident reporting responsibilities; personnel who have or should have reported incidents; personnel (authorities) to whom incident information is to be reported; personnel with information security responsibilities].

**Test**

[SELECT FROM: Incident monitoring capability for the organization; mechanisms supporting or implementing tracking and documenting of system security incidents; organizational processes for incident reporting; mechanisms supporting or implementing incident reporting].

### DISCUSSION

Tracking and documenting system security incidents includes maintaining records about each incident, the status of the incident, and other pertinent information necessary for forensics, evaluating incident details, trends, and handling. Incident information can be obtained from a variety of sources including incident reports, incident response teams, audit monitoring, network monitoring, physical access monitoring, and user/administrator reports. Reporting incidents addresses specific incident reporting requirements within an organization and the formal incident reporting requirements for the organization. Suspected security incidents may also be reported and include the receipt of suspicious email communications that can potentially contain malicious code. The types of security incidents reported, the content and timeliness of the reports, and the designated reporting authorities reflect applicable laws, Executive Orders, directives, regulations, and policies.

NIST SP 800-61 provides guidance on incident handling.

### FURTHER DISCUSSION

Incident handling is the actions the organization takes to prevent or contain the impact of an incident to the organization while it is occurring or shortly after it has occurred. The majority of the process consists of incident identification, containment, eradication, and recovery. During this process, it is essential to track the work processes required in order to effectively respond. Designate a central hub to serve as the point to coordinate, communicate, and track activities. The hub should receive and document information from system administrators, incident handlers, and others involved throughout the process. As the incident process moves toward eradication, executives, affected business units, and any required external stakeholders should be kept aware of the incident in order to make decisions affecting the business. Report to designated authorities, taking into account applicable laws, directives, regulations, and other guidance. Specify staff responsible for communicating about the incident to internal and external stakeholders.

**Example**

You notice unusual activity on a server and determine a potential security incident has occurred. You open a tracking ticket with the Security Operations Center (SOC), which assigns an incident handler to work the ticket [a]. The handler investigates and documents initial findings, which lead to a determination that unauthorized access occurred on the server [b].The SOC establishes an incident management team consisting of security, database, network, and system administrators. The team meets daily to update progress and plan courses of action to contain the incident [a]. At the end of the day, the team provides a status report to IT executives [d,f]. Two days later, the team declares the incident contained. The team produces a final report as the database system is rebuilt and placed back into operation.

**Potential Assessment Considerations**

* Is there an incident response policy that directs the establishment of requirements for tracking and reporting of incidents involving CUI to appropriate officials [a,d]?
* Is cybersecurity incident information promptly reported to management [e,f]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.6.2