# CM.L2-3.4.7 – Nonessential Functionality

## Security Requirement Restrict, disable, or prevent the use of nonessential programs, functions, ports, protocols, and services. |

## Assessment Objectives [a] essential programs are defined;  [b] the use of nonessential programs is defined;  [c] the use of nonessential programs is restricted, disabled, or prevented as defined;  [d] essential functions are defined;  [e] the use of nonessential functions is defined;  [f] the use of nonessential functions is restricted, disabled, or prevented as defined;  [g] essential ports are defined;  [h] the use of nonessential ports is defined;  [i] the use of nonessential ports is restricted, disabled, or prevented as defined;  [j] essential protocols are defined;  [k] the use of nonessential protocols is defined;  [l] the use of nonessential protocols is restricted, disabled, or prevented as defined;  [m] essential services are defined;  [n] the use of nonessential services is defined; and  [o] the use of nonessential services is restricted, disabled, or prevented as defined. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## CM.L2-3.4.7 – NONESSENTIAL FUNCTIONALITY

### SECURITY REQUIREMENT

Restrict, disable, or prevent the use of nonessential programs, functions, ports, protocols, and services.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] essential programs are defined;
:   [b] the use of nonessential programs is defined;
:   [c] the use of nonessential programs is restricted, disabled, or prevented as defined;
:   [d] essential functions are defined;
:   [e] the use of nonessential functions is defined;
:   [f] the use of nonessential functions is restricted, disabled, or prevented as defined;
:   [g] essential ports are defined;
:   [h] the use of nonessential ports is defined;
:   [i] the use of nonessential ports is restricted, disabled, or prevented as defined;
:   [j] essential protocols are defined;
:   [k] the use of nonessential protocols is defined;
:   [l] the use of nonessential protocols is restricted, disabled, or prevented as defined;
:   [m] essential services are defined;
:   [n] the use of nonessential services is defined; and
:   [o] the use of nonessential services is restricted, disabled, or prevented as defined.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Configuration management policy; procedures addressing least functionality in the system; configuration management plan; system security plan; system design documentation; security configuration checklists; system configuration settings and associated documentation; specifications for preventing software program execution; documented reviews of programs, functions, ports, protocols, and/or services; change control records; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with responsibilities for reviewing programs, functions, ports, protocols, and services on the system; personnel with information security responsibilities; system or network administrators; system developers].

**Test**

[SELECT FROM: Organizational processes for reviewing and disabling nonessential programs, functions, ports, protocols, or services; mechanisms implementing review and handling of nonessential programs, functions, ports, protocols, or services; organizational processes preventing program execution on the system; organizational processes for software program usage and restrictions; mechanisms supporting or implementing software program usage and restrictions; mechanisms preventing program execution on the system].

### DISCUSSION

Restricting the use of nonessential software (programs) includes restricting the roles allowed to approve program execution; prohibiting auto-execute; program blacklisting and whitelisting; or restricting the number of program instances executed at the same time. The organization makes a security-based determination which functions, ports, protocols, and/or services are restricted. Bluetooth, File Transfer Protocol (FTP), and peer-to-peer networking are examples of protocols organizations consider preventing the use of, restricting, or disabling.

### FURTHER DISCUSSION

Organizations should only use the minimum set of programs, services, ports, and protocols required for to accomplish the organization’s mission. This has several implications:

* All unnecessary programs and accounts are removed from all endpoints and servers.
* The organization makes a policy decision to control the execution of programs through either whitelisting or blacklisting. Whitelisting means a program can only run if the software has been vetted in some way, and the executable name has been entered onto a list of allowed software. Blacklisting means any software can execute as long it is not on a list of known malicious software. Whitelisting provides far more security than blacklisting, but the organization’s policy can direct the implementation of either approach. Control of execution applies to both servers and endpoints.
* The organization restricts the use of all unnecessary ports, protocols, and system services in order to limit entry points that attackers can use. For example, the use of the FTP service is eliminated from all computers, and the associated ports are blocked unless a required service utilizes those ports. The elimination of nonessential functionality on the network and systems provides a smaller attack surface for an attacker to gain access and take control of your network or systems.

This practice, CM.L2-3.4.7, which requires limiting functionality to essential programs, ports, protocols, and services, extends CM.L2-3.4.6, which requires adherence to the principle of least functionality but does not specifically address which elements of a system should be limited.

**Example**

You are responsible for purchasing new endpoint hardware, installing organizationally required software to the hardware, and configuring the endpoint in accordance with the organization’s policy. The organization has a system imaging capability that loads all necessary software, but it does not remove unnecessary services, eliminate the use of certain protocols, or close unused ports. After imaging the systems, you close all ports and block the use of all protocols except the following:

* TCP for SSH on port 22;
* SMTP on port 25;
* TCP and UDP on port 53; and
* HTTP and HTTPS on port 443.

The use of any other ports or protocols are allowed by exception only [i,l,o].

**Potential Assessment Considerations**

* Are only applications and services that are needed for the function of the system configured and enabled [a,b,c,d,e,f]?
* Are only those ports and protocols necessary to provide the service of the information system configured for that system [g,h,i,j,k,l]?
* Are systems services reviewed to determine what is essential for the function of that system [m]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.4.7