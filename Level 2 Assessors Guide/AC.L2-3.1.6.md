# AC.L2-3.1.6 – Non-Privileged Account Use

## Security Requirement Use non-privileged accounts or roles when accessing nonsecurity functions. |

## Assessment Objectives [a] nonsecurity functions are identified; and  [b] users are required to use non-privileged accounts or roles when accessing nonsecurity functions. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.6 – NON-PRIVILEGED ACCOUNT USE

### SECURITY REQUIREMENT

Use non-privileged accounts or roles when accessing nonsecurity functions.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] nonsecurity functions are identified; and
:   [b] users are required to use non-privileged accounts or roles when accessing nonsecurity functions.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; procedures addressing least privilege; system security plan; list of system-generated security functions assigned to system accounts or roles; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with responsibilities for defining least privileges necessary to accomplish specified organizational tasks; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Mechanisms implementing least privilege functions].

### DISCUSSION

This requirement limits exposure when operating from within privileged accounts or roles. The inclusion of roles addresses situations where organizations implement access control policies such as role-based access control and where a change of role provides the same degree of assurance in the change of access authorizations for the user and all processes acting on behalf of the user as would be provided by a change between a privileged and non- privileged account.

### FURTHER DISCUSSION

A user with a privileged account can perform more tasks and access more information than a person with a non-privileged account. Tasks (including unauthorized tasks orchestrated by attackers) performed when using the privileged account can have a greater impact on the system. System administrators and users with privileged accounts must be trained not to use their privileged accounts for everyday tasks, such as browsing the internet or connecting unnecessarily to other systems or services.

**Example**

You are a system administrator logged in using your privileged account and you need to look up how to reset a non-functioning application. You should log on to another computer with your non-privileged account before you connect to the web and start searching for the reset information [b]. That way, if your account is compromised during the search, it will be your regular user account rather than an account with elevated privileges.

**Potential Assessment Considerations**

* Are nonsecurity functions and non-privileged roles defined [a,b]?
* Is it required that nonsecurity functions only be accessed with the use of non-privileged accounts? How is this verified [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.6