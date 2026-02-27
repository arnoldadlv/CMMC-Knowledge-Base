# MA.L2-3.7.5 – Nonlocal Maintenance

## Security Requirement Require multifactor authentication to establish nonlocal maintenance sessions via external network connections and terminate such connections when nonlocal maintenance is complete. |

## Assessment Objectives [a] multifactor authentication is used to establish nonlocal maintenance sessions via external network connections; and  [b] nonlocal maintenance sessions established via external network connections are terminated when nonlocal maintenance is complete. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## MA.L2-3.7.5 – NONLOCAL MAINTENANCE

### SECURITY REQUIREMENT

Require multifactor authentication to establish nonlocal maintenance sessions via external network connections and terminate such connections when nonlocal maintenance is complete.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] multifactor authentication is used to establish nonlocal maintenance sessions via external network connections; and
:   [b] nonlocal maintenance sessions established via external network connections are terminated when nonlocal maintenance is complete.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System maintenance policy; procedures addressing nonlocal system maintenance; system security plan; system design documentation; system configuration settings and associated documentation; maintenance records; diagnostic records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with system maintenance responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Organizational processes for managing nonlocal maintenance; mechanisms implementing, supporting, and managing nonlocal maintenance; mechanisms for strong authentication of nonlocal maintenance diagnostic sessions; mechanisms for terminating nonlocal maintenance sessions and network connections].

### DISCUSSION

Nonlocal maintenance and diagnostic activities are those activities conducted by individuals communicating through an external network. The authentication techniques employed in the establishment of these nonlocal maintenance and diagnostic sessions reflect the network access requirements in IA.L2-3.5.3.

### FURTHER DISCUSSION

Nonlocal maintenance activities must use multifactor authentication. Multifactor authentication requires at least two factors, such as:

* something you know (e.g., password, personal identification number [PIN]);
* something you have (e.g., cryptographic identification device, token); or
* something you are (e.g., biometric fingerprint or facial scan).

Requiring two or more factors to prove your identity increases the security of the connection. Nonlocal maintenance activities are activities conducted from external network connections such as over the internet. After nonlocal maintenance activities are complete, shut down the external network connection.

This practice, MA.L2-3.7.5 requires the addition of multifactor authentication for remote maintenance sessions and complements five other practices dealing with remote access (AC.L2-3.1.12, AC.L2-3.1.14, AC.L2-3.1.13, AC.L2-3.1.15, and IA.L2-3.5.3):

* AC.L2-3.1.12 requires the control of remote access sessions.
* AC.L2-3.1.14 limits remote access to specific access control points.
* AC.L2-3.1.13 requires the use of cryptographic mechanisms when enabling remote sessions.
* AC.L2-3.1.15 requires authorization for privileged commands executed during a remote session.
* Finally, IA.L2-3.5.3 requires multifactor authentication for network access to non-privileged accounts.

**Example**

You are responsible for maintaining your company’s firewall. In order to conduct maintenance while working remotely, you connect to the firewall’s management interface and log in using administrator credentials. The firewall then sends a verification request to the multifactor authentication app on your smartphone [a]. You need both of these things to prove your identity [a]. After you respond to the multifactor challenge, you have access to the maintenance interface. When you finish your activities, you shut down the remote connection by logging out and quitting your web browser [b].

**Potential Assessment Considerations**

* Is multifactor authentication required prior to maintenance of a system when connecting remotely from outside the system boundary [a]?
* Are personnel required to manually terminate remote maintenance sessions established via external network connections when maintenance is complete, or are connections terminated automatically through system session management mechanisms [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.7.5