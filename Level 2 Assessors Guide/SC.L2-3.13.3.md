# SC.L2-3.13.3 – Role Separation

## Security Requirement Separate user functionality from system management functionality. |

## Assessment Objectives [a] user functionality is identified;  [b] system management functionality is identified; and  [c] user functionality is separated from system management functionality. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SC.L2-3.13.3 – ROLE SEPARATION

### SECURITY REQUIREMENT

Separate user functionality from system management functionality.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] user functionality is identified;
:   [b] system management functionality is identified; and
:   [c] user functionality is separated from system management functionality.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and communications protection policy;procedures addressing application partitioning; system design documentation; system configuration settings and associated documentation;system security plan;system audit logs and records;other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; system developer].

**Test**

[SELECT FROM: Separation of user functionality from system management functionality].

### DISCUSSION

System management functionality includes functions necessary to administer databases, network components, workstations, or servers, and typically requires privileged user access.The separation of user functionality from system management functionality is physical or logical. Organizations can implement separation of system management functionality from user functionality by using different computers, different central processing units, different instances of operating systems, or different network addresses; virtualization techniques; or combinations of these or other methods, as appropriate. This type of separation includes web administrative interfaces that use separate authentication methods for users of any other system resources. Separation of system and user functionality may include isolating administrative interfaces on different domains and with additional access controls.

### FURTHER DISCUSSION

Prevent users and user services from accessing system management functionality on IT components (e.g., databases, network components, workstations, servers). This reduces the attack surface to those critical interfaces by limiting who can access and how they can be accessed. By separating the user functionality from system management functionality, the administrator or privileged functions are not available to the general user.

The intent of this practice is to ensure:

* general users are not permitted to perform system administration functions; and
* system administrators only perform system administration functions from their privileged account.

This can be accomplished using separation like VLANs or logical separation using strong access control methods.

**Example**

As a system administrator, you are responsible for managing a number of core systems.Policy prevents you from conducting any administration from the computer or system account you use for day-to-day work [a,b]. The servers you manage also are isolated from the main corporate network. To work with them you use a special unique account to connect to a “jump” server that has access to the systems you routinely administer.

**Potential Assessment Considerations**

* Are physical or logical controls used to separate user functionality from system management-related functionality (e.g., to ensure that administration (e.g., privilege) options are not available to general users) [c]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.13.3