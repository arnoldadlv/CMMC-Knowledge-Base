# AC.L2-3.1.1 – Authorized Access Control [CUI Data]

## Security Requirement Limit information system access to authorized users, processes acting on behalf of authorized users, or devices (including other information systems). |

## Assessment Objectives [a] authorized users are identified;  [b] processes acting on behalf of authorized users are identified;  [c] devices (and other systems) authorized to connect to the system are identified;  [d] system access is limited to authorized users;  [e] system access is limited to processes acting on behalf of authorized users; and  [f] system access is limited to authorized devices (including other systems). |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.1 – AUTHORIZED ACCESS CONTROL

Level 1 Reference: AC.L1-b.1.i

### SECURITY REQUIREMENT

Limit information system access to authorized users, processes acting on behalf of authorized users, or devices (including other information systems).

### ASSESSMENT OBJECTIVES [NIST SP 800-171A]

Determine if:

:   [a] authorized users are identified;
:   [b] processes acting on behalf of authorized users are identified;
:   [c] devices (and other systems) authorized to connect to the system are identified;
:   [d] system access is limited to authorized users;
:   [e] system access is limited to processes acting on behalf of authorized users; and
:   [f] system access is limited to authorized devices (including other systems).

### POTENTIAL ASSESSMENT METHODS AND OBJECTS [NIST SP 800-171A]

**Examine**

[SELECT FROM: Access control policy; procedures addressing account management; system security plan; system design documentation; system configuration settings and associated documentation; list of active system accounts and the name of the individual associated with each account; notifications or records of recently transferred, separated, or terminated employees; list of conditions for group and role membership; list of recently disabled system accounts along with the name of the individual associated with each account; access authorization records; account management compliance reviews; system monitoring records; system audit logs and records; list of devices and systems authorized to connect to organizational systems; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with account management responsibilities; system or network administrators; personnel with information security responsibilities].

**Test**

[SELECT FROM: Organizational processes for managing system accounts; mechanisms for implementing account management].

### DISCUSSION [NIST SP 800-171 R2]

Access control policies (e.g., identity- or role-based policies, control matrices, and cryptography) control access between active entities or subjects (i.e., users or processes acting on behalf of users) and passive entities or objects (e.g., devices, files, records, and domains) in systems. Access enforcement mechanisms can be employed at the application and service level to provide increased information security. Other systems include systems internal and external to the organization. This requirement focuses on account management for systems and applications. The definition of and enforcement of access authorizations, other than those determined by account type (e.g., privileged verses [sic] non-privileged) are addressed in requirement 3.1.2 (AC.L1-3.1.2).

### FURTHER DISCUSSION

Identify users, processes, and devices that are allowed to use company computers and can log on to the company network. Automated updates and other automatic processes should be associated with the user who initiated (authorized) the process. Limit the devices (e.g., printers) that can be accessed by company computers. Set up your system so that only authorized users, processes, and devices can access the company network.

This practice, AC.L1-3.1.1, controls system access based on user, process, or device identity. AC.L1-3.1.1 leverages IA.L1-3.5.1 which provides a vetted and trusted identity for access control.

**Example 1**

Your company maintains a list of all personnel authorized to use company information systems [a]. This list is used to support identification and authentication activities conducted by IT when authorizing access to systems [a,d].

**Example 2**

A coworker wants to buy a new multi-function printer/scanner/fax device and make it available on the company network. You explain that the company controls system and device access to the network and will prevent network access by unauthorized systems and devices [c]. You help the coworker submit a ticket that asks for the printer to be granted access to the network, and appropriate leadership approves the device [f].

**Potential Assessment Considerations**

* Is a list of authorized users maintained that defines their identities and roles [a]?
* Are account requests authorized before system access is granted [d,e,f]?

### KEY REFERENCES

* FAR Clause 52.204-21 b.1.i
* NIST SP 800-171 Rev 2 3.1.1