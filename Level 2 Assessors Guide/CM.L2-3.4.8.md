# CM.L2-3.4.8 – Application Execution Policy

## Security Requirement Apply deny-by-exception (blacklisting) policy to prevent the use of unauthorized software or deny-all, permit-by-exception (whitelisting) policy to allow the execution of authorized software. |

## Assessment Objectives [a] a policy specifying whether whitelisting or blacklisting is to be implemented is specified;  [b] the software allowed to execute under whitelisting or denied use under blacklisting is specified; and  [c] whitelisting to allow the execution of authorized software or blacklisting to prevent the use of unauthorized software is implemented as specified. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## CM.L2-3.4.8 – APPLICATION EXECUTION POLICY

### SECURITY REQUIREMENT

Apply deny-by-exception (blacklisting) policy to prevent the use of unauthorized software or deny-all, permit-by-exception (whitelisting) policy to allow the execution of authorized software.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] a policy specifying whether whitelisting or blacklisting is to be implemented is specified;
:   [b] the software allowed to execute under whitelisting or denied use under blacklisting is specified; and
:   [c] whitelisting to allow the execution of authorized software or blacklisting to prevent the use of unauthorized software is implemented as specified.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Configuration management policy; procedures addressing least functionality in the system; system security plan; configuration management plan; system design documentation; system configuration settings and associated documentation; list of software programs not authorized to execute on the system; list of software programs authorized to execute on the system; security configuration checklists; review and update records associated with list of authorized or unauthorized software programs; change control records; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with responsibilities for identifying software authorized or not authorized to execute on the system; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Organizational process for identifying, reviewing, and updating programs authorized or not authorized to execute on the system; process for implementing blacklisting or whitelisting; mechanisms supporting or implementing blacklisting or whitelisting].

### DISCUSSION

The process used to identify software programs that are not authorized to execute on systems is commonly referred to as blacklisting. The process used to identify software programs that are authorized to execute on systems is commonly referred to as whitelisting. Whitelisting is the stronger of the two policies for restricting software program execution.

In addition to whitelisting, organizations consider verifying the integrity of whitelisted software programs using, for example, cryptographic checksums, digital signatures, or hash functions. Verification of whitelisted software can occur either prior to execution or at system startup.

NIST SP 800-167 provides guidance on application whitelisting.

### FURTHER DISCUSSION

Organizations should determine their blacklisting or whitelisting policy and configure the system to manage software that is allowed to run. Blacklisting or deny-by-exception allows all software to run except if on an unauthorized software list such as what is maintained in antivirus solutions. Whitelisting or permit-by-exception does not allow any software to run except if on an authorized software list. The stronger policy of the two is whitelisting.

This practice, CM.L2-3.4.8, requires the implementation of allow-lists and deny-lists for application software. It leverages CM.L2-3.4.1, which requires the organization to establish and maintain software inventories.

This practice, CM.L2-3.4.8, also extends CM.L2-3.4.9, which only requires control and monitoring of any user installed software.

**Example**

To improve your company’s protection from malware, you have decided to allow only designated programs to run. With additional research you identify a capability within the latest operating system that can control executables, scripts, libraries, or application installers run in your environment [c]. To ensure success you begin by authorizing digitally signed executables. Once they are deployed, you then plan to evaluate and deploy whitelisting for software libraries and scripts [c].

**Potential Assessment Considerations**

* Is the information system configured to only allow authorized software to run [a,b,c]?
* Is the system configured to disallow running unauthorized software [a,b,c]?
* Is there a defined list of software programs authorized to execute on the system [b]?
* Is the authorization policy a deny-all, permit by exception for software allowed to execute on the system [a,b,c]?
* Are automated mechanisms used to prevent program execution in accordance with defined lists (e.g., white listing) [a,b,c]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.4.8