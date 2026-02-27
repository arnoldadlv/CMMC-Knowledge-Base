# AC.L2-3.1.3 – Control CUI Flow

## Security Requirement Control the flow of CUI in accordance with approved authorizations. |

## Assessment Objectives [a] information flow control policies are defined;  [b] methods and enforcement mechanisms for controlling the flow of CUI are defined;  [c] designated sources and destinations (e.g., networks, individuals, and devices) for CUI within the system and between interconnected systems are identified;  [d] authorizations for controlling the flow of CUI are defined; and  [e] approved authorizations for controlling the flow of CUI are enforced. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.3 – CONTROL CUI FLOW

### SECURITY REQUIREMENT

Control the flow of CUI in accordance with approved authorizations.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] information flow control policies are defined;
:   [b] methods and enforcement mechanisms for controlling the flow of CUI are defined;
:   [c] designated sources and destinations (e.g., networks, individuals, and devices) for CUI within the system and between interconnected systems are identified;
:   [d] authorizations for controlling the flow of CUI are defined; and
:   [e] approved authorizations for controlling the flow of CUI are enforced.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; information flow control policies; procedures addressing information flow enforcement; system security plan; system design documentation; system configuration settings and associated documentation; list of information flow authorizations; system baseline configuration; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; system developers].

**Test**

[SELECT FROM: Mechanisms implementing information flow enforcement policy].

### DISCUSSION

Information flow control regulates where information can travel within a system and between systems (versus who can access the information) and without explicit regard to subsequent accesses to that information. Flow control restrictions include the following: keeping export-controlled information from being transmitted in the clear to the internet; blocking outside traffic that claims to be from within the organization; restricting requests to the internet that are not from the internal web proxy server; and limiting information transfers between organizations based on data structures and content.

Organizations commonly use information flow control policies and enforcement mechanisms to control the flow of information between designated sources and destinations (e.g., networks, individuals, and devices) within systems and between interconnected systems. Flow control is based on characteristics of the information or the information path. Enforcement occurs in boundary protection devices (e.g., gateways, routers, guards, encrypted tunnels, firewalls) that employ rule sets or establish configuration settings that restrict system services, provide a packet-filtering capability based on header information, or message-filtering capability based on message content (e.g., implementing key word searches or using document characteristics). Organizations also consider the trustworthiness of filtering and inspection mechanisms (i.e., hardware, firmware, and software components) that are critical to information flow enforcement.

Transferring information between systems representing different security domains with different security policies introduces risk that such transfers violate one or more domain security policies.

Organizations consider the shared nature of commercial telecommunications services in the implementation of security requirements associated with the use of such services. Commercial telecommunications services are commonly based on network components and consolidated management systems shared by all attached commercial customers and may also include third party-provided access lines and other service elements. Such transmission services may represent sources of increased risk despite contract security provisions. NIST SP 800-41 provides guidance on firewalls and firewall policy. SP 800-125B provides guidance on security for virtualization technologies.

In such situations, information owners or stewards provide guidance at designated policy enforcement points between interconnected systems. Organizations consider mandating specific architectural solutions when required to enforce specific security policies. Enforcement includes: prohibiting information transfers between interconnected systems (i.e., allowing access only); employing hardware mechanisms to enforce one-way information flows; and implementing trustworthy regrading mechanisms to reassign security attributes and security labels.

### FURTHER DISCUSSION

Typically, companies will have a firewall between the internal network and the internet. Often multiple firewalls or routing switches are used inside a network to create zones to separate sensitive data, business units, or user groups. Proxy servers can be used to break the connection between multiple networks. All traffic entering or leaving a network is intercepted by the proxy, preventing direct access between networks. Companies should also ensure by policy and enforcement mechanisms that all CUI allowed to flow across the internet is encrypted.

**Example 1**

As a system administrator, you configure a proxy device on your company’s network. Your goal is to better mask and protect the devices inside the network while enforcing information flow policies. After the device is configured, information does not flow directly from the internal network to the internet. The proxy device intercepts the traffic and analyzes it to determine if the traffic conforms to organization information flow control policies. If it does, the device allows the information to pass to its destination [b]. The proxy blocks traffic that does not meet policy requirements [e].

**Example 2**

As a subcontractor on a DoD contract, your organization sometimes needs to transmit CUI to the prime contractor. You create a policy document that specifies who is allowed to transmit CUI and that such transmission requires manager approval [a,c,d]. The policy instructs users to encrypt any CUI transmitted via email or to use a designated secure file sharing utility [b,d]. The policy states that users who do not follow appropriate procedures may be subject to disciplinary action [e].

**Potential Assessment Considerations**

* Are designated sources of regulated data identified within the system (e.g., internal network and IP address) and between interconnected systems (e.g., external networks, IP addresses, ports, and protocols) [c]?
* Are designated destinations of regulated data identified within the system (e.g., internal network and IP address) and between interconnected systems (external networks and IP addresses) [c]?
* Are authorizations defined for each source and destination within the system and between interconnected systems (e.g., allow or deny rules for each combination of source and destination) [d]?
* Are approved authorizations for controlling the flow of regulated data enforced within the system and between interconnected systems (e.g., traffic between authorized sources and destinations is allowed and traffic between unauthorized sources and destinations is denied) [e]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.3