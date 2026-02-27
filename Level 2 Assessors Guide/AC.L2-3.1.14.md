# AC.L2-3.1.14 – Remote Access Routing

## Security Requirement Route remote access via managed access control points. |

## Assessment Objectives [a] managed access control points are identified and implemented; and  [b] remote access is routed through managed network access control points. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.14 – REMOTE ACCESS ROUTING

### SECURITY REQUIREMENT

Route remote access via managed access control points.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] managed access control points are identified and implemented; and
:   [b] remote access is routed through managed network access control points.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; procedures addressing remote access to the system; system security plan; system design documentation; list of all managed network access control points; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities].

**Test**

[SELECT FROM: Mechanisms routing all remote accesses through managed network access control points].

### DISCUSSION

Routing remote access through managed access control points enhances explicit, organizational control over such connections, reducing the susceptibility to unauthorized access to organizational systems resulting in the unauthorized disclosure of CUI.

### FURTHER DISCUSSION

The contractor can route all remote access through a limited number of remote access control points to reduce the attack surface and simplify network management. This allows for better monitoring and control of the remote connections.

This practice, AC.L2-3.1.14, limits remote access to specific access control points and complements five other practices dealing with remote access (AC.L2-3.1.12, AC.L2-3.1.13, AC.L2-3.1.15, IA.L2-3.5.3, and MA.L2-3.7.5):

* AC.L2-3.1.12 requires the control of remote access sessions.
* AC.L2-3.1.13 requires the use of cryptographic mechanisms when enabling remote sessions.
* AC.L2-3.1.15 requires authorization for privileged commands executed during a remote session.
* IA.L2-3.5.3 requires multifactor authentication for network access to non-privileged accounts.
* Finally, MA.L2-3.7.5 requires the addition of multifactor authentication for remote maintenance sessions.

**Example**

You are a system administrator for a company with many locations, and several employees at different locations need to connect to the organization’s networks while working remotely. Because each company location has a direct connection to headquarters, you decide to route all remote access through the headquarters location [a]. All remote traffic is routed through a single location to simplify monitoring [b].

**Potential Assessment Considerations**

* How many managed access control points are implemented [a]?
* Is all remote access routed through the managed access control points [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.14