# SI.L2-3.14.7 – Identify Unauthorized Use

## Security Requirement Identify unauthorized use of organizational systems. |

## Assessment Objectives [a] authorized use of the system is defined; and  [b] unauthorized use of the system is identified. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SI.L2-3.14.7 – IDENTIFY UNAUTHORIZED USE

### SECURITY REQUIREMENT

Identify unauthorized use of organizational systems.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] authorized use of the system is defined; and
:   [b] unauthorized use of the system is identified.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Continuous monitoring strategy; system and information integrity policy; procedures addressing system monitoring tools and techniques; facility diagram/layout; system security plan; system design documentation; system monitoring tools and techniques documentation; locations within system where monitoring devices are deployed; system configuration settings and associated documentation; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; personnel installing, configuring, and maintaining the system; personnel with responsibility for monitoring the system].

**Test**

[SELECT FROM: Organizational processes for system monitoring; mechanisms supporting or implementing system monitoring capability].

### DISCUSSION

System monitoring includes external and internal monitoring. System monitoring can detect unauthorized use of organizational systems. System monitoring is an integral part of continuous monitoring and incident response programs. Monitoring is achieved through a variety of tools and techniques (e.g., intrusion detection systems, intrusion prevention systems, malicious code protection software, scanning tools, audit record monitoring software, network monitoring software). Output from system monitoring serves as input to continuous monitoring and incident response programs.

Unusual/unauthorized activities or conditions related to inbound and outbound communications traffic include internal traffic that indicates the presence of malicious code in systems or propagating among system components, the unauthorized exporting of information, or signaling to external systems. Evidence of malicious code is used to identify potentially compromised systems or system components. System monitoring requirements, including the need for specific types of system monitoring, may be referenced in other requirements.

NIST SP 800-94 provides guidance on intrusion detection and prevention systems.

### FURTHER DISCUSSION

Define authorized use of your systems. Create an acceptable use policy to establish the baseline for how users access devices, internal network services, and the internet. Define authorized use by specific roles such as: user, administrator, and technician. After authorized use is defined, identify unauthorized use of systems.

Monitor systems by observing audit activities from the system logs. This can be accomplished in real time using automated solutions or by manual means. To identify unauthorized use, leverage existing tools and techniques, such as:

* intrusion detection systems;
* intrusion prevention systems;
* malicious code protection software;
* scanning tools;
* audit record monitoring software; and
* network monitoring software.

This practice, SI.L2-3.14.7, which deals with identifying unauthorized use of organizational systems, is related to practices: AC.L1-3.1.1, AU.L2-3.3.1, IA.L1-3.5.1, and IA.L1-3.5.2. All of these practices help create the building blocks that support SI.L2-3.14.7.

**Example 1**

You are in charge of IT operations. You need to ensure that everyone using an organizational system is authorized to do so and conforms to the written authorized use policy. To do this, you deploy an application that monitors user activity and records the information for later analysis. You review the data from this application for signs of activity that does not conform to the acceptable use policy [a,b].

**Example 2**

You are alerted through your Intrusion Detection System (IDS) that one of your users is connecting to a server that is from a high-risk domain (based on your commercial domain reputation service). You investigate and determine that it’s not the user, but instead an unauthorized connection attempt [b]. You add the domain to your list of blocked domains to prevent connections in the future.

**Potential Assessment Considerations**

* Is authorized use of systems defined (e.g., data types permitted for storage or processing, personnel authorized to access, times or days of permitted use, permitted software) [a]?
* Is unauthorized use of systems defined (e.g., not authorized to use systems for bitcoin mining, not authorized for pornographic content, not authorized to access gambling games/content) [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.14.7