# CM.L2-3.4.3 – System Change Management

## Security Requirement Track, review, approve or disapprove, and log changes to organizational systems. |

## Assessment Objectives [a] changes to the system are tracked;  [b] changes to the system are reviewed;  [c] changes to the system are approved or disapproved; and  [d] changes to the system are logged. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## CM.L2-3.4.3 – SYSTEM CHANGE MANAGEMENT

### SECURITY REQUIREMENT

Track, review, approve or disapprove, and log changes to organizational systems.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] changes to the system are tracked;
:   [b] changes to the system are reviewed;
:   [c] changes to the system are approved or disapproved; and
:   [d] changes to the system are logged.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Configuration management policy; procedures addressing system configuration change control; configuration management plan; system architecture and configuration documentation; system security plan; change control records; system audit logs and records; change control audit and review reports; agenda/minutes from configuration change control oversight meetings; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with configuration change control responsibilities; personnel with information security responsibilities; system or network administrators; members of change control board or similar].

**Test**

[SELECT FROM: Organizational processes for configuration change control; mechanisms that implement configuration change control].

### DISCUSSION

Tracking, reviewing, approving/disapproving, and logging changes is called configuration change control. Configuration change control for organizational systems involves the systematic proposal, justification, implementation, testing, review, and disposition of changes to the systems, including system upgrades and modifications. Configuration change control includes changes to baseline configurations for components and configuration items of systems, changes to configuration settings for information technology products (e.g., operating systems, applications, firewalls, routers, and mobile devices), unscheduled and unauthorized changes, and changes to remediate vulnerabilities.

Processes for managing configuration changes to systems include Configuration Control Boards or Change Advisory Boards that review and approve proposed changes to systems.

For new development systems or systems undergoing major upgrades, organizations consider including representatives from development organizations on the Configuration Control Boards or Change Advisory Boards. Audit logs of changes include activities before and after changes are made to organizational systems and the activities required to implement such changes.

NIST SP 800-128 provides guidance on configuration change control.

### FURTHER DISCUSSION

You must track, review, and approve configuration changes before committing to production. Changes to computing environments can create unintended and unforeseen issues that can affect the security and availability of the systems. Relevant experts and stakeholders must review and approve proposed changes. They should discuss potential impacts before the organization puts the changes in place. Relevant items include changes to the physical environment and to the systems hosted within it.

**Example**

Once a month, the management and technical team leads join a change control board meeting. During this meeting, everyone reviews all proposed changes to the environment [b,c]. This includes changes to the physical and computing environments. The meeting ensures that relevant subject-matter experts review changes and propose alternatives where needed.

**Potential Assessment Considerations**

* Are changes to the system authorized by company management and documented : [a,b,c,d]?
* Are changes documented and tracked (e.g., manually written down or included in a tracking service such as a ticketing system) [d]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.4.3