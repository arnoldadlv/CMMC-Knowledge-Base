# SC.L2-3.13.9 – Connections Termination

## Security Requirement Terminate network connections associated with communications sessions at the end of the sessions or after a defined period of inactivity. |

## Assessment Objectives [a] a period of inactivity to terminate network connections associated with communications sessions is defined;  [b] network connections associated with communications sessions are terminated at the end of the sessions; and  [c] network connections associated with communications sessions are terminated after the defined period of inactivity. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SC.L2-3.13.9 – CONNECTIONS TERMINATION

### SECURITY REQUIREMENT

Terminate network connections associated with communications sessions at the end of the sessions or after a defined period of inactivity.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] a period of inactivity to terminate network connections associated with communications sessions is defined;
:   [b] network connections associated with communications sessions are terminated at the end of the sessions; and
:   [c] network connections associated with communications sessions are terminated after the defined period of inactivity.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and communications protection policy; procedures addressing network disconnect; system design documentation; system security plan; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; system developer].

**Test**

[SELECT FROM: Mechanisms supporting or implementing network disconnect capability].

### DISCUSSION

This requirement applies to internal and external networks. Terminating network connections associated with communications sessions include de-allocating associated TCP/IP address or port pairs at the operating system level, or de-allocating networking assignments at the application level if multiple application sessions are using a single, operating system-level network connection. Time periods of user inactivity may be established by organizations and include time periods by type of network access or for specific network accesses.

### FURTHER DISCUSSION

Prevent malicious actors from taking advantage of an open network session or an unattended computer at the end of the connection. Balance user work patterns and needs against security to determine the length of inactivity that will force a termination.

This practice, SC.L2-3.13.9, requires network connections be terminated under certain conditions, which complements AC.L2-3.1.18 that requires control of mobile device connections.

**Example**

You are an administrator of a server that provides remote access. Your company’s policies state that network connections must be terminated after being idle for 60 minutes [a]. You edit the server configuration file and set the timeout to 60 minutes and restart the remote access software [c]. You test the software and verify that the connection is terminated appropriately.

**Potential Assessment Considerations**

* Are the network connections requiring management and time-out for inactivity documented [a]?
* Are the network connections requiring management and time-out for inactivity configured and implemented [c]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.13.9