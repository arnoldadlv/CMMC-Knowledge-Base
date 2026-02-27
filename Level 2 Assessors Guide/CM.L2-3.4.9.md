# CM.L2-3.4.9 – User-Installed Software

## Security Requirement Control and monitor user-installed software. |

## Assessment Objectives [a] a policy for controlling the installation of software by users is established;  [b] installation of software by users is controlled based on the established policy; and  [c] installation of software by users is monitored. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## CM.L2-3.4.9 – USER-INSTALLED SOFTWARE

### SECURITY REQUIREMENT

Control and monitor user-installed software.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] a policy for controlling the installation of software by users is established;
:   [b] installation of software by users is controlled based on the established policy; and
:   [c] installation of software by users is monitored.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Configuration management policy; procedures addressing user installed software; configuration management plan; system security plan; system design documentation; system configuration settings and associated documentation; list of rules governing user-installed software; system monitoring records; system audit logs and records; continuous monitoring strategy; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with responsibilities for governing user-installed software; personnel operating, using, or maintaining the system; personnel monitoring compliance with user-installed software policy; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Organizational processes governing user-installed software on the system; mechanisms enforcing rules or methods for governing the installation of software by users; mechanisms monitoring policy compliance].

### DISCUSSION

Users can install software in organizational systems if provided the necessary privileges. To maintain control over the software installed, organizations identify permitted and prohibited actions regarding software installation through policies. Permitted software installations include updates and security patches to existing software and applications from organization-approved “app stores.” Prohibited software installations may include software with unknown or suspect pedigrees or software that organizations consider potentially malicious. The policies organizations select governing user-installed software may be organization-developed or provided by some external entity. Policy enforcement methods include procedural methods, automated methods, or both.

### FURTHER DISCUSSION

Software that users have the ability to install is limited to items that the organization approves. When not controlled, users could install software that can create unnecessary risk. This risk applies both to the individual machine and to the larger operating environment. Policies and technical controls reduce risk to the organization by preventing users from installing unauthorized software.

**Example**

You are a system administrator. A user calls you for help installing a software package. They are receiving a message asking for a password because they do not have permission to install the software. You explain that the policy prohibits users from installing software without approval [a]. When you set up workstations for users, you do not provide administrative privileges. After the call, you redistribute the policy to all users ensuring everyone in the company is aware of the restrictions.

**Potential Assessment Considerations**

* Are user controls in place to prohibit the installation of unauthorized software [a]?
* Is all software in use on the information systems approved [b]?
* Is there a mechanism in place to monitor the types of software a user is permitted to download (e.g., is there a white list of approved software) [c]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.4.9