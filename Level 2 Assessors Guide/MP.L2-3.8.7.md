# MP.L2-3.8.7 – Removable Media

## Security Requirement Control the use of removable media on system components. |

## Assessment Objectives [a] the use of removable media on system components is controlled. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## MP.L2-3.8.7 – REMOVEABLE MEDIA

### SECURITY REQUIREMENT

Control the use of removable media on system components.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the use of removable media on system components is controlled.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System media protection policy; system use policy; procedures addressing media usage restrictions; system security plan; rules of behavior; system design documentation; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with system media use responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Organizational processes for media use; mechanisms restricting or prohibiting use of system media on systems or system components].

### DISCUSSION

In contrast to requirement MP.L2-3.8.1, which restricts user access to media, this requirement restricts the use of certain types of media on systems, for example, restricting or prohibiting the use of flash drives or external hard disk drives. Organizations can employ technical and nontechnical controls (e.g., policies, procedures, and rules of behavior) to control the use of system media. Organizations may control the use of portable storage devices, for example, by using physical cages on workstations to prohibit access to certain external ports, or disabling or removing the ability to insert, read, or write to such devices.

Organizations may also limit the use of portable storage devices to only approved devices including devices provided by the organization, devices provided by other approved organizations, and devices that are not personally owned. Finally, organizations may control the use of portable storage devices based on the type of device, prohibiting the use of writeable, portable devices, and implementing this restriction by disabling or removing the capability to write to such devices. Malicious code protection mechanisms include anti-virus signature definitions and reputation-based technologies. Many technologies and methods exist to limit or eliminate the effects of malicious code. Pervasive configuration management and comprehensive software integrity controls may be effective in preventing execution of unauthorized code. In addition to commercial off-the-shelf software, malicious code may also be present in custom-built software. This could include logic bombs, back doors, and other types of cyber-attacks that could affect organizational missions/business functions. Traditional malicious code protection mechanisms cannot always detect such code. In these situations, organizations rely instead on other safeguards including secure coding practices, configuration management and control, trusted procurement processes, and monitoring practices to help ensure that software does not perform functions other than the functions intended.

### FURTHER DISCUSSION

Removable media are any type of media storage that you can remove from your computer or machine (e.g., CDs, DVDs, diskettes, and USB drives). Write a specific policy for removable media. The policy should cover the various types of removable media (e.g., write-once media and rewritable media) and should discuss the company’s approach to removable media. Ensure the following controls are considered and included in the policy:

* limit the use of removable media to the smallest number needed; and
* scan all removable media for viruses.

**Example**

You are in charge of IT operations. You establish a policy for removable media that includes USB drives [a]. The policy information such as:

* only USB drives issued by the organization may be used; and
* USB drives are to be used for work purposes only [a].

You set up a separate computer to scan these drives before anyone uses them on the network. This computer has anti-virus software installed that is kept up to date.

**Potential Assessment Considerations**

* Are removable media allowed [a]?
* Are policies and/or procedures in use to control the use of removable media [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.8.7