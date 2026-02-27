# SC.L2-3.13.4 – Shared Resource Control

## Security Requirement Prevent unauthorized and unintended information transfer via shared system resources. |

## Assessment Objectives [a] unauthorized and unintended information transfer via shared system resources is prevented. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SC.L2-3.13.4 – SHARED RESOURCE CONTROL

### SECURITY REQUIREMENT

Prevent unauthorized and unintended information transfer via shared system resources.=== ASSESSMENT OBJECTIVES ===
Determine if:

:   [a] unauthorized and unintended information transfer via shared system resources is prevented.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and communications protection policy; procedures addressing application partitioning; system security plan; system design documentation; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; system developer].

**Test**

[SELECT FROM: Separation of user functionality from system management functionality].

### DISCUSSION

The control of information in shared system resources (e.g., registers, cache memory, main memory, hard disks) is also commonly referred to as object reuse and residual information protection. This requirement prevents information produced by the actions of prior users or roles (or the actions of processes acting on behalf of prior users or roles) from being available to any current users or roles (or current processes acting on behalf of current users or roles) that obtain access to shared system resources after those resources have been released back to the system. This requirement also applies to encrypted representations of information.This requirement does not address information remnants, which refers to residual representation of data that has been nominally deleted; covert channels (including storage or timing channels) where shared resources are manipulated to violate information flow restrictions; or components within systems for which there are only single users or roles.

### FURTHER DISCUSSION

No shared system resource, such as cache memory, hard disks, registers, or main memory may pass information from one user to another user. In other words, when objects are reused no residual information should exist on that object. This protects the confidentiality of the information. This is typically a feature provided by operating system and software vendors.

**Example**

You are a system administrator responsible for creating and deploying the system hardening procedures for your company’s computers. You ensure that the computer baselines include software patches to prevent attackers from exploiting flaws in the processor architecture to read data (e.g., the Meltdown and Spectre exploits). You also verify that the computer operating system is configured to prevent users from accessing other users’ folders [a].

**Potential Assessment Considerations**

* Are shared system resources identified and documented [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.13.4