# SC.L2-3.13.5 – Public-Access System Separation [CUI Data]

## Security Requirement Implement subnetworks for publicly accessible system components that are physically or logically separated from internal networks. |

## Assessment Objectives [a] publicly accessible system components are identified; and  [b] subnetworks for publicly accessible system components are physically or logically separated from internal networks. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SC.L2-3.13.5 – PUBLIC-ACCESS SYSTEM SEPARATION

Level 1 Requirement: SC.L1-b.1.xi

### SECURITY REQUIREMENT

Implement subnetworks for publicly accessible system components that are physically or logically separated from internal networks.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] publicly accessible system components are identified; and
:   [b] subnetworks for publicly accessible system components are physically or logically separated from internal networks.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and communications protection policy; procedures addressing boundary protection; system security plan; list of key internal boundaries of the system; system design documentation; boundary protection hardware and software; system configuration settings and associated documentation; enterprise security architecture documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; system developers; personnel with boundary protection responsibilities].

**Test**

[SELECT FROM: Mechanisms implementing boundary protection capability].

### DISCUSSION

Subnetworks that are physically or logically separated from internal networks are referred to as demilitarized zones (DMZs). DMZs are typically implemented with boundary control devices and techniques that include routers, gateways, firewalls, virtualization, or cloud- based technologies.

NIST SP 800-41 provides guidance on firewalls and firewall policy. SP 800-125B provides guidance on security for virtualization technologies.

### FURTHER DISCUSSION

Separate the publicly accessible systems from the internal systems that need to be protected. Do not place internal systems on the same network as the publicly accessible systems and block access by default from DMZ networks to internal networks.

One method of accomplishing this is to create a DMZ network, which enhances security by providing public access to a specific set of resources while preventing connections from those resources to the rest of the IT environment. Some contractors achieve a similar result through the use of a cloud computing environment that is separated from the rest of the company’s infrastructure.

**Example**

The head of recruiting at your company wants to launch a website to post job openings and allow the public to download an application form [a]. After some discussion, your team realizes it needs to use a firewall to create a perimeter network to do this [b]. You host the server separately from the company’s internal network and make sure the network on which it resides is isolated with the proper firewall rules [b].

**Potential Assessment Considerations**

* Are any system components reachable by the public (e.g., internet-facing web servers, VPN gateways, publicly accessible cloud services) [a]?
* Are publicly accessible system components on physically or logically separated subnetworks (e.g., isolated subnetworks using separate, dedicated VLAN segments such as DMZs) [b]?

### KEY REFERENCES

* FAR Clause 52.204-21 b.1.xi
* NIST SP 800-171 Rev 2 3.13.5