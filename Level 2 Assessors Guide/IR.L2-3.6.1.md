# IR.L2-3.6.1 – Incident Handling

## Security Requirement Establish an operational incident-handling capability for organizational systems that includes preparation, detection, analysis, containment, recovery, and user response activities. |

## Assessment Objectives [a] an operational incident-handling capability is established;  [b] the operational incident-handling capability includes preparation;  [c] the operational incident-handling capability includes detection;  [d] the operational incident-handling capability includes analysis;  [e] the operational incident-handling capability includes containment;  [f] the operational incident-handling capability includes recovery; and  [g] the operational incident-handling capability includes user response |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## IR.L2-3.6.1 – INCIDENT HANDLING

### SECURITY REQUIREMENT

Establish an operational incident-handling capability for organizational systems that includes preparation, detection, analysis, containment, recovery, and user response activities.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] an operational incident-handling capability is established;
:   [b] the operational incident-handling capability includes preparation;
:   [c] the operational incident-handling capability includes detection;
:   [d] the operational incident-handling capability includes analysis;
:   [e] the operational incident-handling capability includes containment;
:   [f] the operational incident-handling capability includes recovery; and
:   [g] the operational incident-handling capability includes user response activities.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Incident response policy; contingency planning policy; procedures addressing incident handling; procedures addressing incident response assistance; incident response plan; contingency plan; system security plan; procedures addressing incident response training; incident response training curriculum; incident response training materials; incident response training records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with incident handling responsibilities; personnel with contingency planning responsibilities; personnel with incident response training and operational responsibilities; personnel with incident response assistance and support responsibilities; personnel with access to incident response support and assistance capability; personnel with information security responsibilities].

**Test**

[SELECT FROM: Incident-handling capability for the organization; organizational processes for incident response assistance; mechanisms supporting or implementing incident response assistance].

### DISCUSSION

Organizations recognize that incident handling capability is dependent on the capabilities of organizational systems and the mission/business processes being supported by those systems. Organizations consider incident handling as part of the definition, design, and development of mission/business processes and systems. Incident-related information can be obtained from a variety of sources including audit monitoring, network monitoring, physical access monitoring, user and administrator reports, and reported supply chain events. Effective incident handling capability includes coordination among many organizational entities including mission/business owners, system owners, authorizing officials, human resources offices, physical and personnel security offices, legal departments, operations personnel, procurement offices, and the risk executive.

As part of user response activities, incident response training is provided by organizations and is linked directly to the assigned roles and responsibilities of organizational personnel to ensure that the appropriate content and level of detail is included in such training. For example, regular users may only need to know who to call or how to recognize an incident on the system; system administrators may require additional training on how to handle or remediate incidents;and incident responders may receive more specific training on forensics, reporting, system recovery, and restoration. Incident response training includes user training in the identification/reporting of suspicious activities from external and internal sources. User response activities also includes incident response assistance which may consist of help desk support, assistance groups, and access to forensics services or consumer redress services, when required.

NIST SP 800-61 provides guidance on incident handling. SP 800-86 and SP 800-101 provide guidance on integrating forensic techniques into incident response. SP 800-161 provides guidance on supply chain risk management.

### FURTHER DISCUSSION

Incident handling capabilities prepare your organization to respond to incidents and may:

* identify people inside and outside your organization you may need to contact during an incident;
* establish a way to report incidents, such as an email address or a phone number;
* establish a system for tracking incidents; and
* determine a place and a way to store evidence of an incident.

Software and hardware may be required to analyze incidents when they occur. Incident prevention activities are also part of an incident-handling capability. The incident-handling team provides input for such things as risk assessments and training.

Contractors detect incidents using different indicators. Indicators may include:

* alerts from sensors or antivirus software;
* a filename that looks unusual; and
* log entries that raise concern.

After detecting an incident, an incident response team performs analysis. This requires some knowledge of normal network operations. The incident should be documented including all the log entries associated with the incident.

Containment of the incident is a critical step to stop the damage the incident is causing to your network. Containment activities should be based on previously defined organizational priorities and assessment of risk.

Recovery activities restore systems to pre-incident functionality and address its underlying causes. Organizations should use recovery activities as a means of improving their overall resilience to future attacks.

**Example**

Your manager asks you to set up your company’s incident-response capability [a]. First, you create an email address to collect information on possible incidents. Next, you draft a contact list of all the people who need to know when an incident occurs. You document a procedure for how to submit incidents that includes roles and responsibilities when a potential incident is detected or reported. The procedure also explains how to track incidents, from initial creation to closure [b].

**Potential Assessment Considerations**

* Is there an incident response policy which specifically outlines requirements for handling of incidents involving CUI [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.6.1