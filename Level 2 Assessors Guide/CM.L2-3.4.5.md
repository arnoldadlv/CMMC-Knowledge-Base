# CM.L2-3.4.5 – Access Restrictions for Change

## Security Requirement Define, document, approve, and enforce physical and logical access restrictions associated with changes to organizational systems. |

## Assessment Objectives [a] physical access restrictions associated with changes to the system are defined;  [b] physical access restrictions associated with changes to the system are documented;  [c] physical access restrictions associated with changes to the system are approved;  [d] physical access restrictions associated with changes to the system are enforced;  [e] logical access restrictions associated with changes to the system are defined;  [f] logical access restrictions associated with changes to the system are documented;  [g] logical access restrictions associated with changes to the system are approved; and  [h] logical access restrictions associated with changes to the system are enforced. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## CM.L2-3.4.5 – ACCESS RESTRICTIONS FOR CHANGE

### SECURITY REQUIREMENT

Define, document, approve, and enforce physical and logical access restrictions associated with changes to organizational systems.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] physical access restrictions associated with changes to the system are defined;
:   [b] physical access restrictions associated with changes to the system are documented;
:   [c] physical access restrictions associated with changes to the system are approved;
:   [d] physical access restrictions associated with changes to the system are enforced;
:   [e] logical access restrictions associated with changes to the system are defined;
:   [f] logical access restrictions associated with changes to the system are documented;
:   [g] logical access restrictions associated with changes to the system are approved; and
:   [h] logical access restrictions associated with changes to the system are enforced.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Configuration management policy; procedures addressing access restrictions for changes to the system; system security plan; configuration management plan; system design documentation; system architecture and configuration documentation; system configuration settings and associated documentation; logical access approvals; physical access approvals; access credentials; change control records; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with logical access control responsibilities; personnel with physical access control responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Organizational processes for managing access restrictions associated with changes to the system; mechanisms supporting, implementing, and enforcing access restrictions associated with changes to the system].

### DISCUSSION

Any changes to the hardware, software, or firmware components of systems can potentially have significant effects on the overall security of the systems. Therefore, organizations permit only qualified and authorized individuals to access systems for purposes of initiating changes, including upgrades and modifications. Access restrictions for change also include software libraries. Access restrictions include physical and logical access control requirements, workflow automation, media libraries, abstract layers (e.g., changes implemented into external interfaces rather than directly into systems), and change windows (e.g., changes occur only during certain specified times). In addition to security concerns, commonly-accepted due diligence for configuration management includes access restrictions as an essential part in ensuring the ability to effectively manage the configuration.

NIST SP 800-128 provides guidance on configuration change control.

### FURTHER DISCUSSION

Define, identify, and document qualified individuals authorized to make physical and logical changes to the organization’s hardware, software, software libraries, or firmware components. Control of configuration management activities may involve:

* physical access control that prohibits unauthorized users from gaining physical access to an asset (e.g., requiring a special key card to enter a server room);
* logical access control that prevents unauthorized users from logging onto a system to make configuration changes (e.g., requiring specific credentials for modifying configuration settings, patching software, or updating software libraries);
* workflow automation in which configuration management workflow rules define human tasks and data or files are routed between people authorized to do configuration management based on pre-defined business rules (e.g., passing an electronic form to a manager requesting approval of configuration change made by an authorized employee);
* an abstraction layer for configuration management that requires changes be made from an external system through constrained interface (e.g., software updates can only be made from a patch management system with a specific IP address); and
* utilization of a configuration management change window (e.g., software updates are only allowed between 8:00 AM and 10:00 AM or between 6:00 PM and 8:00 PM).

**Example**

Your datacenter requires expanded storage capacity in a server. The change has been approved, and security is planning to allow an external technician to access the building at a specific date and time under the supervision of a manager [a,b,c,d]. A system administrator creates a temporary privileged account that can be used to log into the server’s operating system and update storage settings [e,f,g]. On the appointed day, the technician is escorted into the datacenter, upgrades the hardware, expands the storage in the operating system (OS), and departs. The manager verifies the upgrade and disables the privileged account [h].

**Potential Assessment Considerations**

* Are only employees who are approved to make physical or logical changes on systems allowed to do so [a,d,e,h]?
* Are authorized personnel approved and documented by the service owner and IT security [a,e]?
* Does all change documentation include the name of the authorized employee making the change [b,d,f,h]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.4.5