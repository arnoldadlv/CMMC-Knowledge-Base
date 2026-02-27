# CM.L2-3.4.6 – Least Functionality

## Security Requirement Employ the principle of least functionality by configuring organizational systems to provide only essential capabilities. |

## Assessment Objectives [a] essential system capabilities are defined based on the principle of least functionality; and  [b] the system is configured to provide only the defined essential capabilities. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## CM.L2-3.4.6 – LEAST FUNCTIONALITY

### SECURITY REQUIREMENT

Employ the principle of least functionality by configuring organizational systems to provide only essential capabilities.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] essential system capabilities are defined based on the principle of least functionality; and
:   [b] the system is configured to provide only the defined essential capabilities.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Configuration management policy; configuration management plan; procedures addressing least functionality in the system; system security plan; system design documentation; system configuration settings and associated documentation; security configuration checklists; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with security configuration management responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Organizational processes prohibiting or restricting functions, ports, protocols, or services; mechanisms implementing restrictions or prohibition of functions, ports, protocols, or services].

### DISCUSSION

Systems can provide a wide variety of functions and services. Some of the functions and services routinely provided by default, may not be necessary to support essential organizational missions, functions, or operations. It is sometimes convenient to provide multiple services from single system components. However, doing so increases risk over limiting the services provided by any one component. Where feasible, organizations limit component functionality to a single function per component.

Organizations review functions and services provided by systems or components of systems, to determine which functions and services are candidates for elimination. Organizations disable unused or unnecessary physical and logical ports and protocols to prevent unauthorized connection of devices, transfer of information, and tunneling. Organizations can utilize network scanning tools, intrusion detection and prevention systems, and end-point protections such as firewalls and host-based intrusion detection systems to identify and prevent the use of prohibited functions, ports, protocols, and services.

### FURTHER DISCUSSION

You should customize organizational systems to remove non-essential applications and disable unnecessary services. Systems come with many unnecessary applications and settings enabled by default including unused ports and protocols. Leave only the fewest capabilities necessary for the systems to operate effectively.

**Example**

You have ordered a new server, which has arrived with a number of free utilities installed in addition to the operating system. Before you deploy the server, you research the utilities to determine which ones can be eliminated without impacting functionality. You remove the unneeded software, then move on to disable unused ports and services. The server that enters production therefore has only the essential capabilities enabled for the system to function in its role [a,b].

**Potential Assessment Considerations**

* Are the roles and functions for each system identified along with the software and services required to perform those functions [a]?
* Are the software and services required for those defined functions identified [a]?
* Is the information system configured to exclude any function not needed in the operational environment [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.4.6