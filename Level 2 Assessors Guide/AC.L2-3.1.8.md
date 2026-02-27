# AC.L2-3.1.8 – Unsuccessful Logon Attempts

## Security Requirement Limit unsuccessful logon attempts. |

## Assessment Objectives [a] the means of limiting unsuccessful logon attempts is defined; and  [b] the defined means of limiting unsuccessful logon attempts is implemented. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.8 – UNSUCCESSFUL LOGON ATTEMPTS

### SECURITY REQUIREMENT

Limit unsuccessful logon attempts.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the means of limiting unsuccessful logon attempts is defined; and
:   [b] the defined means of limiting unsuccessful logon attempts is implemented.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; procedures addressing unsuccessful logon attempts; system security plan; system design documentation; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with information security responsibilities; system developers; system or network administrators].

**Test**

[SELECT FROM: Mechanisms implementing access control policy for unsuccessful logon attempts].

### DISCUSSION

This requirement applies regardless of whether the logon occurs via a local or network connection. Due to the potential for denial of service, automatic lockouts initiated by systems are, in most cases, temporary and automatically release after a predetermined period established by the organization (i.e., a delay algorithm). If a delay algorithm is selected, organizations may employ different algorithms for different system components based on the capabilities of the respective components. Responses to unsuccessful logon attempts may be implemented at the operating system and application levels.

### FURTHER DISCUSSION

Consecutive unsuccessful logon attempts may indicate malicious activity. Contractors can mitigate these attacks by limiting the number of unsuccessful logon attempts, typically by locking the account. A defined number of consecutive unsuccessful logon attempts is a common configuration setting. Contractors are expected to set this number at a level that fits their risk profile with the knowledge that fewer unsuccessful attempts provide higher security.

After an unsuccessful login attempt threshold is exceeded and the system locks an account, the account may either remain locked until an administrator takes action to unlock it, or it may be locked for a predefined time after which it unlocks automatically.

**Example**

You attempt to log on to your work computer. You mistype your password three times in a row, and an error message is generated telling you the account is locked [b]. You call your IT help desk or system administrator to request assistance. The system administrator explains that the account is locked as a result of three unsuccessful logon attempts [a].The administrator offers to unlock the account and notes that you can wait 30 minutes for the account to unlock automatically.

**Potential Assessment Considerations**

* Is there a defined threshold for the number of unsuccessful logon attempts for which the system takes action to prevent additional attempts [a]?
* Is a mechanism for limiting the number of unsuccessful logon attempts implemented and does it use the defined threshold [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.8