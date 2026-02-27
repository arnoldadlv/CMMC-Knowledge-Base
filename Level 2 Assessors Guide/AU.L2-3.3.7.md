# AU.L2-3.3.7 – Authoritative Time Source

## Security Requirement Provide a system capability that compares and synchronizes internal system clocks with an authoritative source to generate time stamps for audit records. |

## Assessment Objectives [a] internal system clocks are used to generate time stamps for audit records;  [b] an authoritative source with which to compare and synchronize internal system clocks is specified; and  [c] internal system clocks used to generate time stamps for audit records are compared to and synchronized with the specified authoritative time source. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AU.L2-3.3.7 – AUTHORITATIVE TIME SOURCE

### SECURITY REQUIREMENT

Provide a system capability that compares and synchronizes internal system clocks with an authoritative source to generate time stamps for audit records.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] internal system clocks are used to generate time stamps for audit records;
:   [b] an authoritative source with which to compare and synchronize internal system clocks is specified; and
:   [c] internal system clocks used to generate time stamps for audit records are compared to and synchronized with the specified authoritative time source.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Audit and accountability policy; procedures addressing time stamp generation; system design documentation; system security plan; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with information security responsibilities; system or network administrators; system developers].

**Test**

[SELECT FROM: Mechanisms implementing time stamp generation; mechanisms implementing internal information system clock synchronization].

### DISCUSSION

Internal system clocks are used to generate time stamps, which include date and time. Time is expressed in Coordinated Universal Time (UTC), a modern continuation of Greenwich Mean Time (GMT), or local time with an offset from UTC. The granularity of time measurements refers to the degree of synchronization between system clocks and reference clocks, for example, clocks synchronizing within hundreds of milliseconds or within tens of milliseconds. Organizations may define different time granularities for different system components. Time service can also be critical to other security capabilities such as access control and identification and authentication, depending on the nature of the mechanisms used to support those capabilities. This requirement provides uniformity of time stamps for systems with multiple system clocks and systems connected over a network.

### FURTHER DISCUSSION

Each system must synchronize its time with a central time server to ensure that all systems are recording audit logs using the same time source. Reviewing audit logs from multiple systems can be a difficult task if time is not synchronized. Systems can be synchronized to a network device or directory service or configured manually.

**Example**

You are setting up several new computers on your company’s network. You update the time settings on each machine to use the same authoritative time server on the internet [b,c].When you review audit logs, all your machines will have synchronized time, which aids in any potential security investigations.

**Potential Assessment Considerations**

* Can the records’ time stamps map to Coordinated Universal Time (UTC), compare system clocks with authoritative Network Time Protocol (NTP) servers, and synchronize system clocks when the time difference is greater than 1 second [c]?
* Does the system synchronize internal system clocks on a defined frequency [c]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.3.7