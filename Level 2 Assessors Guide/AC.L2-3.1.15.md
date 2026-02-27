# AC.L2-3.1.15 – Privileged Remote Access

## Security Requirement Authorize remote execution of privileged commands and remote access to security-relevant information. |

## Assessment Objectives [a] privileged commands authorized for remote execution are identified;  [b] security-relevant information authorized to be accessed remotely is identified;  [c] the execution of the identified privileged commands via remote access is authorized; and  [d] access to the identified security-relevant information via remote access is authorized. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.15 – PRIVILEGED REMOTE ACCESS

### SECURITY REQUIREMENT

Authorize remote execution of privileged commands and remote access to security-relevant information.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] privileged commands authorized for remote execution are identified;
:   [b] security-relevant information authorized to be accessed remotely is identified;
:   [c] the execution of the identified privileged commands via remote access is authorized; and
:   [d] access to the identified security-relevant information via remote access is authorized.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; procedures addressing remote access to the system; system configuration settings and associated documentation; system security plan; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities].

**Test**

[SELECT FROM: Mechanisms implementing remote access management].

### DISCUSSION

A privileged command is a human-initiated (interactively or via a process operating on behalf of the human) command executed on a system involving the control, monitoring, or administration of the system including security functions and associated security-relevant information. Security-relevant information is any information within the system that can potentially impact the operation of security functions or the provision of security services in a manner that could result in failure to enforce the system security policy or maintain isolation of code and data. Privileged commands give individuals the ability to execute sensitive, security-critical, or security-relevant system functions. Controlling such access from remote locations helps to ensure that unauthorized individuals are not able to execute such commands freely with the potential to do serious or catastrophic damage to organizational systems. Note that the ability to affect the integrity of the system is considered security-relevant as that could enable the means to by-pass security functions although not directly impacting the function itself.

### FURTHER DISCUSSION

Privileged users are not necessarily allowed to perform their job functions from a remote location. Likewise, not all privileged commands may be executed remotely. Allowing remote execution of privileged commands or remote access to security-relevant information should be avoided if possible. If absolutely necessary, the privileged commands authorized for remote execution should be identified and documented. Document which user roles have permissions to remotely execute privileged commands to make changes and to access security relevant information. Documentation must be used to establish security mechanisms that enforce the policy.

This practice, AC.L2-3.1.15, requires authorization for privileged commands executed during a remote session and complements five other practices dealing with remote access (AC.L2- 3.1.12, AC.L2-3.1.14, AC.L2-3.1.13, IA.L2-3.5.3, and MA.L2-3.7.5):

* AC.L2-3.1.12 requires the control of remote access sessions.
* AC.L2-3.1.14 limits remote access to specific access control points.
* AC.L2-3.1.13 requires the use of cryptographic mechanisms when enabling remote sessions.
* IA.L2-3.5.3 requires multifactor authentication for network access to non-privileged accounts.
* Finally, MA.L2-3.7.5 requires the addition of multifactor authentication for remote maintenance sessions.

This practice, AC.L2-3.1.15, also extends AC.L1-3.1.2, which limits the types of transactions and functions that authorized users are permitted to execute.

**Example**

Your company’s Access Control Policy permits certain work roles to remotely perform a limited set of privileged commands from company-owned computers [a].As a system administrator, you implement controls to enforce who can remotely execute a privileged command, which privileged commands they can execute, and who is allowed access to security relevant information such as audit log configuration settings [a,c,d].

**Potential Assessment Considerations**

* Does system documentation identify system administration or security functions that can be executed remotely [a]?
* Is execution of the identified privileged commands via remote access only authorized for documented operational needs [c]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.15