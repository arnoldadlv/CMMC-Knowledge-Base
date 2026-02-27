# AC.L2-3.1.5 – Least Privilege

## Security Requirement Employ the principle of least privilege, including for specific security functions and privileged accounts. |

## Assessment Objectives [a] privileged accounts are identified;  [b] access to privileged accounts is authorized in accordance with the principle of least privilege;  [c] security functions are identified; and  [d] access to security functions is authorized in accordance with the principle of least privilege. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.5 – LEAST PRIVILEGE

### SECURITY REQUIREMENT

Employ the principle of least privilege, including for specific security functions and privileged accounts.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] privileged accounts are identified;
:   [b] access to privileged accounts is authorized in accordance with the principle of least privilege;
:   [c] security functions are identified; and
:   [d] access to security functions is authorized in accordance with the principle of least privilege.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; procedures addressing account management; system security plan; system design documentation; system configuration settings and associated documentation; list of active system accounts and the name of the individual associated with each account; list of conditions for group and role membership; notifications or records of recently transferred, separated, or terminated employees; list of recently disabled system accounts along with the name of the individual associated with each account ;access authorization records; account management compliance reviews; system monitoring/audit records; procedures addressing least privilege; list of security functions (deployed in hardware, software, and firmware) and security-relevant information for which access is to be explicitly authorized; list of system-generated privileged accounts; list of system administration personnel; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with account management responsibilities; system or network administrators; personnel with information security responsibilities; personnel with responsibilities for defining least privileges necessary to accomplish specified tasks].

**Test**

[SELECT FROM: Organizational processes for managing system accounts; mechanisms for implementing account management; mechanisms implementing least privilege functions; mechanisms prohibiting privileged access to the system].

### DISCUSSION

Organizations employ the principle of least privilege for specific duties and authorized accesses for users and processes. The principle of least privilege is applied with the goal of authorized privileges no higher than necessary to accomplish required organizational missions or business functions. Organizations consider the creation of additional processes, roles, and system accounts as necessary, to achieve least privilege. Organizations also apply least privilege to the development, implementation, and operation of organizational systems. Security functions include establishing system accounts, setting events to be logged, setting intrusion detection parameters, and configuring access authorizations (i.e., permissions, privileges).

Privileged accounts, including super user accounts, are typically described as system administrator for various types of commercial off-the-shelf operating systems. Restricting privileged accounts to specific personnel or roles prevents day-to-day users from having access to privileged information or functions. Organizations may differentiate in the application of this requirement between allowed privileges for local accounts and for domain accounts provided organizations retain the ability to control system configurations for key security parameters and as otherwise necessary to sufficiently mitigate risk.

### FURTHER DISCUSSION

The principle of least privilege applies to all users and processes on all systems, but it is critical to systems containing or accessing CUI. Least privilege:

* restricts user access to only the machines and information needed to fulfill job responsibilities; and
* limits what system configuration settings users can change, only allowing individuals with a business need to change them.

**Example**

As a system administrator, you create accounts. By default, everyone is assigned a basic user role, which prevents a user from modifying system configurations. Privileged access is only assigned to users and processes that require it to carry out job functions, such as IT staff, and is very selectively granted [b,d].

**Potential Assessment Considerations**

* Are privileged accounts documented and is when they may be used defined [a]?
* Are users assigned privileged accounts to perform their job functions only when it is necessary [b]?
* Are necessary security functions identified (e.g., access control configuration, system configuration settings, or privileged account lists) that must be managed through the use of privileged accounts [c]?
* Is access to privileged functions and security information restricted to authorized employees [d]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.5