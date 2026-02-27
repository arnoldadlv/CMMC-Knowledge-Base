# SC.L2-3.13.16 – Data at Rest

## Security Requirement Protect the confidentiality of CUI at rest. |

## Assessment Objectives [a] the confidentiality of CUI at rest is protected. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SC.L2-3.13.16 – DATA AT REST

### SECURITY REQUIREMENT

Protect the confidentiality of CUI at rest.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the confidentiality of CUI at rest is protected.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and communications protection policy; procedures addressing protection of information at rest; system security plan; system design documentation; list of information at rest requiring confidentiality protections; system configuration settings and associated documentation; cryptographic mechanisms and associated configuration documentation; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; system developer].

**Test**

[SELECT FROM: Mechanisms supporting or implementing confidentiality protections for information at rest].

### DISCUSSION

Information at rest refers to the state of information when it is not in process or in transit and is located on storage devices as specific components of systems. The focus of protection at rest is not on the type of storage device or the frequency of access but rather the state of the information. Organizations can use different mechanisms to achieve confidentiality protections, including the use of cryptographic mechanisms and file share scanning. Organizations may also use other controls including secure off-line storage in lieu of online storage when adequate protection of information at rest cannot otherwise be achieved or continuous monitoring to identify malicious code at rest.

### FURTHER DISCUSSION

CUI at rest means information that is not moving through the network; typically this means data currently stored on hard drives, media, and mobile devices. Implement the necessary security controls to protect the confidentiality of CUI at rest. Although an approved encryption method protects data stored at rest, there are other technical and physical solutions. The methods chosen should depend on the environment and business needs.

Implementing encryption for CUI is one approach to this practice, but it is not mandatory. Physical security is often employed to restrict access to CUI, particularly when it resides on servers within a company’s offices. Other approaches for protecting CUI include system- related protections such as configurations and rule sets for firewalls, gateways, intrusion detection/prevention systems, filtering routers, and authenticator content that eliminate attempts at exfiltration. You may also employ other security requirements including secure off-line storage.

This practice, SC.L2-3.13.16, requires confidentially be provided for CUI at rest and complements MP.L2-3.8.9, which requires confidentially of CUI at backup storage locations. This practice, SC.L2-3.13.16, also leverages SC.L2-3.13.11, which specifies that the algorithms used must be FIPS-validated.

**Example 1**

Your company has a policy stating CUI must be protected at rest and you work to enforce that policy. You research Full Disk Encryption (FDE) products that meet the FIPS encryption requirement. After testing, you deploy the encryption to all computers to protect CUI at rest [a].

**Example 2**

You have used encryption to protect the CUI on most of the computers at your company, but you have some devices that do not support encryption. You create a policy requiring these devices to be signed out when needed, stay in possession of the signer when checked out, and to be signed back in and locked up in a secured closet when the user is done with the device [a]. At the end of the day each Friday, you audit the sign-out sheet and make sure all devices are returned to the closet.

**Potential Assessment Considerations**

* Is the confidentiality of CUI at rest protected using encryption of storage devices and/or appropriate physical methods [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.13.16