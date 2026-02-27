# SI.L2-3.14.6 – Monitor Communications for Attacks

## Security Requirement Monitor organizational systems, including inbound and outbound communications traffic, to detect attacks and indicators of potential attacks. |

## Assessment Objectives [a] the system is monitored to detect attacks and indicators of potential attacks;  [b] inbound communications traffic is monitored to detect attacks and indicators of potential attacks; and  [c] outbound communications traffic is monitored to detect attacks and indicators of potential attacks. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SI.L2-3.14.6 – MONITOR COMMUNICATIONS FOR ATTACKS

### SECURITY REQUIREMENT

Monitor organizational systems, including inbound and outbound communications traffic, to detect attacks and indicators of potential attacks.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the system is monitored to detect attacks and indicators of potential attacks;
:   [b] inbound communications traffic is monitored to detect attacks and indicators of potential attacks; and
:   [c] outbound communications traffic is monitored to detect attacks and indicators of potential attacks.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and information integrity policy; procedures addressing system monitoring tools and techniques; continuous monitoring strategy; system and information integrity policy; procedures addressing system monitoring tools and techniques; facility diagram or layout; system security plan; system monitoring tools and techniques documentation; system design documentation; locations within system where monitoring devices are deployed; system protocols; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; personnel installing, configuring, and maintaining the system; personnel with responsibility monitoring the system; personnel with responsibility for the intrusion detection system].

**Test**

[SELECT FROM: Organizational processes for system monitoring; mechanisms supporting or implementing intrusion detection capability and system monitoring; mechanisms supporting or implementing system monitoring capability; organizational processes for intrusion detection and system monitoring; mechanisms supporting or implementing the monitoring of inbound and outbound communications traffic].

### DISCUSSION

System monitoring includes external and internal monitoring. External monitoring includes the observation of events occurring at the system boundary (i.e., part of perimeter defense and boundary protection). Internal monitoring includes the observation of events occurring within the system. Organizations can monitor systems, for example, by observing audit record activities in real time or by observing other system aspects such as access patterns, characteristics of access, and other actions. The monitoring objectives may guide determination of the events. System monitoring capability is achieved through a variety of tools and techniques (e.g., intrusion detection systems, intrusion prevention systems, malicious code protection software, scanning tools, audit record monitoring software, network monitoring software). Strategic locations for monitoring devices include selected perimeter locations and near server farms supporting critical applications, with such devices being employed at managed system interfaces. The granularity of monitoring information collected is based on organizational monitoring objectives and the capability of systems to support such objectives.

System monitoring is an integral part of continuous monitoring and incident response programs. Output from system monitoring serves as input to continuous monitoring and incident response programs. A network connection is any connection with a device that communicates through a network (e.g., local area network, Internet). A remote connection is any connection with a device communicating through an external network (e.g., the Internet). Local, network, and remote connections can be either wired or wireless.

Unusual or unauthorized activities or conditions related to inbound/outbound communications traffic include internal traffic that indicates the presence of malicious code in systems or propagating among system components, the unauthorized exporting of information, or signaling to external systems. Evidence of malicious code is used to identify potentially compromised systems or system components. System monitoring requirements, including the need for specific types of system monitoring, may be referenced in other requirements.

NIST SP 800-94 provides guidance on intrusion detection and prevention systems.

### FURTHER DISCUSSION

Think of indicators of attack as a set of footprints an adversary leaves during an attack. Indicators of attack provide information on the steps the adversary followed and its intent. Indicators of attacks on organizational systems may include:

* internal traffic that indicates the presence of malicious code;
* anomalous activity detected during non-business hours;
* unauthorized data leaving the organization; and
* communicating to external information systems.

To detect attacks and indicators of attacks, deploy monitoring devices or agents. Place these sensors at strategic points within the systems and networks to collect essential information. Strategic points include internal and external system boundaries. Monitor both inbound traffic and outbound traffic as well as actions on hosts.

This practice, SI.L2-3.14.6, provides details for the communications of organizational systems. SI.L2-3.14.6 supports the practice AU.L2-3.3.1, which involves creating and retaining records for monitoring, analysis, and investigations.

**Example**

It is your job to look for known indicators of attack or anomalous activity within your systems and communications traffic [a,b,c]. Because these indicators can show up in a variety of places on your network, you have created a checklist of places to check each week. These include the office firewall logs, the audit logs of the file server where CUI is stored, and the connection log for your VPN gateway [b].

You conduct additional reviews when you find an indicator, or something that does not perform as it should [a].

**Potential Assessment Considerations**

* Are details provided for the methodology of determining attacks and indicators of attack [a]?
* Are monitoring devices deployed within the information system to collect information that may indicate an attack [a]?
* Are communications traffic flows understood and is there a deployed capability to review that traffic [b,c]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.14.6