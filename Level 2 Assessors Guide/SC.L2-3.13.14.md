# SC.L2-3.13.14 – Voice over Internet Protocol

## Security Requirement Control and monitor the use of Voice over Internet Protocol (VoIP) technologies. |

## Assessment Objectives [a] use of Voice over Internet Protocol (VoIP) technologies is controlled; and  [b] use of Voice over Internet Protocol (VoIP) technologies is monitored. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SC.L2-3.13.14 – VOICE OVER INTERNET PROTOCOL

### SECURITY REQUIREMENT

Control and monitor the use of Voice over Internet Protocol (VoIP) technologies.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] use of Voice over Internet Protocol (VoIP) technologies is controlled; and
:   [b] use of Voice over Internet Protocol (VoIP) technologies is monitored.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and communications protection policy; procedures addressing VoIP; VoIP usage restrictions; VoIP implementation guidance; system security plan; system design documentation; system audit logs and records; system configuration settings and associated documentation; system monitoring records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; personnel with responsibilities for managing VoIP].

**Test**

[SELECT FROM: Organizational process for authorizing, monitoring, and controlling VoIP; mechanisms supporting or implementing authorizing, monitoring, and controlling VoIP].

### DISCUSSION

VoIP has different requirements, features, functionality, availability, and service limitations when compared with the Plain Old Telephone Service (POTS) (i.e., the standard telephone service). In contrast, other telephone services are based on high-speed, digital communications lines, such as Integrated Services Digital Network (ISDN) and Fiber Distributed Data Interface (FDDI).The main distinctions between POTS and non-POTS services are speed and bandwidth. To address the threats associated with VoIP, usage restrictions and implementation guidelines are based on the potential for the VoIP technology to cause damage to the system if it is used maliciously. Threats to VoIP are similar to those inherent with any Internet-based application.

### FURTHER DISCUSSION

Controlling VoIP technologies starts with establishing guidelines and enforcing the appropriate usage that is described in organizational policies. Monitoring should include the users’ activity for anything other than what is permitted and authorized and detection of insecure or unauthorized use of the VoIP technology. Security concerns for VoIP include eavesdropping on calls and using ID spoofing to impersonate trusted individuals.

Selecting a solution that can encrypt VoIP traffic is helpful in maintaining the confidentiality and integrity of the voice data.

**Example**

You are a system administrator responsible for the VoIP system. You configure VoIP for new users after being notified that they have signed the Acceptable Use Policy for VoIP technology [a]. You verify that the VoIP solution is configured to use encryption and have enabled requirements for passwords on voice mailboxes and on phone extension management. You require phone system administrators to log in using multifactor authentication when managing the system [a]. You add the VoIP software to the list of applications that are patched monthly as needed [a,b]. Finally, you configure the VoIP system to send logs to your log aggregator so that they can be correlated with those from other systems and examined for signs of suspicious activity [b].

**Potential Assessment Considerations**

* Are VoIP technologies (e.g., approved and managed products or solutions) that may or may not be used in the system defined [a]?
* Is monitoring for unapproved VoIP technologies or unapproved use of the allowed VoIP solutions employed [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.13.14