# SC.L2-3.13.13 – Mobile Code

## Security Requirement Control and monitor the use of mobile code. |

## Assessment Objectives [a] use of mobile code is controlled; and  [b] use of mobile code is monitored. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SC.L2-3.13.13 – MOBILE CODE

### SECURITY REQUIREMENT

Control and monitor the use of mobile code.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] use of mobile code is controlled; and
:   [b] use of mobile code is monitored.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and communications protection policy; procedures addressing mobile code; mobile code usage restrictions, mobile code implementation policy and procedures; system audit logs and records; system security plan; list of acceptable mobile code and mobile code technologies; list of unacceptable mobile code and mobile technologies; authorization records; system monitoring records; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; personnel with responsibilities for managing mobile code].

**Test**

[SELECT FROM: Organizational process for controlling, authorizing, monitoring, and restricting mobile code; mechanisms supporting or implementing the management of mobile code; mechanisms supporting or implementing the monitoring of mobile code].

### DISCUSSION

Mobile code technologies include Java, JavaScript, ActiveX, Postscript, PDF, Flash animations, and VBScript. Decisions regarding the use of mobile code in organizational systems are based on the potential for the code to cause damage to the systems if used maliciously. Usage restrictions and implementation guidance apply to the selection and use of mobile code installed on servers and mobile code downloaded and executed on individual workstations, notebook computers, and devices (e.g., smart phones). Mobile code policy and procedures address controlling or preventing the development, acquisition, or introduction of unacceptable mobile code in systems, including requiring mobile code to be digitally signed by a trusted source.

### FURTHER DISCUSSION

Ensure mobile code is authorized to execute in company systems only in accordance with policy and technical configuration, and that unauthorized mobile code is not. Monitor the use of mobile code through boundary devices (e.g., firewalls), audit logs, or security utilities (e.g., mobile device management, advanced endpoint protection) and implement remediation activities as needed.

The first intent of this practice is to ensure the limits of mobile code usage and usage restrictions are documented and enforced. This includes documenting all authorizations for the use of mobile code and ensuring it is not used in other ways. Usage restrictions and implementation guidance apply to the selection and use of mobile code installed on servers and mobile code downloaded and executed on individual workstations and devices to include all mobile devices and smart phones.

The second intent is to monitor the use of mobile code and implement remediation steps if its use does not align with policy.

**Example**

Your company has decided to prohibit the use of Flash, ActiveX, and Java plug-ins for web browsers on all of its computers [a]. To enforce this policy you configure the computer baseline configuration to disable and deny the execution of mobile code [a]. You implement an exception process to re-enable mobile code execution only for those users with a legitimate business need [a].

One department complains that a web application they need to perform their job no longer works. You meet with them and verify that the web application uses ActiveX in the browser. You submit a change request with the Change Review Board. Once the change is approved, you reconfigure the department’s computers to allow the running of ActiveX in the browser. You also configure the company firewall to alert you if ActiveX is used by any website but the allowed one [b]. You set a reminder for yourself to check in with the department at the end of the year to verify they still need that web application.

**Potential Assessment Considerations**

* Are there defined limits of mobile code usage and established usage restrictions, which specifically authorize use of mobile code (e.g., Java, JavaScript, ActiveX, PDF, Flash, Shockwave, Postscript, VBScript) within the information system [a]?
* Is the use of mobile code documented, monitored, and managed (e.g., Java, JavaScript, ActiveX, PDF, Flash, Shockwave, Postscript, VBScript) [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.13.13