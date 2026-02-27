# AC.L2-3.1.7 – Privileged Functions

## Security Requirement Prevent non-privileged users from executing privileged functions and capture the execution of such functions in audit logs. |

## Assessment Objectives [a] privileged functions are defined;  [b] non-privileged users are defined;  [c] non-privileged users are prevented from executing privileged functions; and  [d] the execution of privileged functions is captured in audit logs. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.7 – PRIVILEGED FUNCTIONS

### SECURITY REQUIREMENT

Prevent non-privileged users from executing privileged functions and capture the execution of such functions in audit logs.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] privileged functions are defined;
:   [b] non-privileged users are defined;
:   [c] non-privileged users are prevented from executing privileged functions; and
:   [d] the execution of privileged functions is captured in audit logs.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Privacy and security policies, procedures addressing system use notification; documented approval of system use notification messages or banners; system audit logs and records; system design documentation; user acknowledgements of notification message or banner; system security plan; system use notification messages; system configuration settings and associated documentation; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with responsibilities for defining least privileges necessary to accomplish specified tasks; personnel with information security responsibilities; system developers].

**Test**

[SELECT FROM: Mechanisms implementing least privilege functions for non-privileged users; mechanisms auditing the execution of privileged functions].

### DISCUSSION

Privileged functions include establishing system accounts, performing system integrity checks, conducting patching operations, or administering cryptographic key management activities. Non-privileged users are individuals that do not possess appropriate authorizations. Circumventing intrusion detection and prevention mechanisms or malicious code protection mechanisms are examples of privileged functions that require protection from non-privileged users. Note that this requirement represents a condition to be achieved by the definition of authorized privileges in 3.1.2 (AC.L1-3.1.2).

Misuse of privileged functions, either intentionally or unintentionally by authorized users, or by unauthorized external entities that have compromised system accounts, is a serious and ongoing concern and can have significant adverse impacts on organizations. Logging the use of privileged functions is one way to detect such misuse, and in doing so, help mitigate the risk from insider threats and the advanced persistent threat.

### FURTHER DISCUSSION

Non-privileged users should receive only those permissions required to perform their basic job functions. Privileged users are granted additional permissions because their jobs require them. Privileged functions typically involve the control, monitoring, or administration of the system and its security measures. When these special privileged functions are performed, the activity must be captured in an audit log, which can be used to identify abuse. Non- privileged employees must not be granted permission to perform any of the functions of a privileged user.

This practice, AC.L2-3.1.7, manages non-privileged users by logging any attempts to execute privileged functions. AC.L2-3.1.7 leverages AU.L2-3.3.2, which ensures logging and traceability of user actions. AC.L2-3.1.7 also extends AC.L1-3.1.2, which defines a requirement to limit types of transactions and functions to those that authorized users are permitted to execute.

**Example**

As a system administrator for your organization, you have put security controls in place that prevent non-privileged users from performing privileged activities [a,b,c]. However, you accidentally gave a standard user elevated system administrator privileges. The organization has implemented an endpoint detection and response solution that provides visibility into the use of privileged activities. The monitoring system logs a security misconfiguration because the use of administrative privileges was performed by a user who was not known to have that ability. This allows you to correct the error [d].

**Potential Assessment Considerations**

* Is it possible to identify who enabled privileges at any particular time [d]?
* Are the privileged system functions documented (e.g., functions that involve the control, monitoring or administration of the system, including security functions and log management) [a]?
* Do documented procedures describe the configuration of the system to ensure system roles do not grant non-privileged users the ability to execute privileged functions [c]?
* Do procedures describe the configuration of system settings to capture the execution of all privileged functions in audit logs [d]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.7