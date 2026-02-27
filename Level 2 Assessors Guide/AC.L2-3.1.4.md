# AC.L2-3.1.4 – Separation of Duties

## Security Requirement Separate the duties of individuals to reduce the risk of malevolent activity without collusion. |

## Assessment Objectives [a] the duties of individuals requiring separation are defined;  [b] responsibilities for duties that require separation are assigned to separate individuals; and  [c] access privileges that enable individuals to exercise the duties that require separation are granted to separate individuals. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.4 – SEPARATION OF DUTIES

### SECURITY REQUIREMENT

Separate the duties of individuals to reduce the risk of malevolent activity without collusion.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the duties of individuals requiring separation are defined;
:   [b] responsibilities for duties that require separation are assigned to separate individuals; and
:   [c] access privileges that enable individuals to exercise the duties that require separation are granted to separate individuals.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; procedures addressing divisions of responsibility and separation of duties; system security plan; system configuration settings and associated documentation; list of divisions of responsibility and separation of duties; system access authorizations; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with responsibilities for defining divisions of responsibility and separation of duties; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Mechanisms implementing separation of duties policy].

### DISCUSSION

Separation of duties addresses the potential for abuse of authorized privileges and helps to reduce the risk of malevolent activity without collusion. Separation of duties includes dividing mission functions and system support functions among different individuals or roles; conducting system support functions with different individuals (e.g., configuration management, quality assurance and testing, system management, programming, and network security);and ensuring that security personnel administering access control functions do not also administer audit functions. Because separation of duty violations can span systems and application domains, organizations consider the entirety of organizational systems and system components when developing policy on separation of duties.

### FURTHER DISCUSSION

No one person should be in charge of an entire critical task from beginning to end. Documenting and dividing elements of important duties and tasks between employees reduces intentional or unintentional execution of malicious activities.

**Example 1**

You are responsible for the management of several key systems within your organization. You assign the task of reviewing the system logs to two different people. This way, no one person is solely responsible for the execution of this critical security function [c].

**Example 2**

You are a system administrator. Human Resources notifies you of a new hire, and you create an account with general privileges, but you are not allowed to grant access to systems that contain CUI [a,b]. The program manager contacts the team in your organization that has system administration authority over the CUI systems and informs them which CUI the new hire will need to access. Subsequently, a second system administrator grants access privileges to the new hire [c].

**Potential Assessment Considerations**

* Does system documentation identify the system functions or processes that require separation of duties (e.g., function combinations that represent a conflict of interest or an over-allocation of security privilege for one individual) [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.4