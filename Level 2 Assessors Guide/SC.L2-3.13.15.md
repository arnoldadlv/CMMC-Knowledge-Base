# SC.L2-3.13.15 – Communications Authenticity

## Security Requirement Protect the authenticity of communications sessions. |

## Assessment Objectives [a] the authenticity of communications sessions is protected. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SC.L2-3.13.15 – COMMUNICATIONS AUTHENTICITY

### SECURITY REQUIREMENT

Protect the authenticity of communications sessions.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the authenticity of communications sessions is protected.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and communications protection policy; procedures addressing session authenticity; system security plan; system design documentation; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities].

**Test**

[SELECT FROM: Mechanisms supporting or implementing session authenticity]

### DISCUSSION

Authenticity protection includes protecting against man-in-the-middle attacks, session hijacking, and the insertion of false information into communications sessions. This requirement addresses communications protection at the session versus packet level (e.g., sessions in service-oriented architectures providing web-based services) and establishes grounds for confidence at both ends of communications sessions in ongoing identities of other parties and in the validity of information transmitted.

NIST SP 800-77, NIST SP 800-95, and NIST SP 800-113 provide guidance on secure communications sessions.

### FURTHER DISCUSSION

The intent of this practice is to ensure a trust relationship is established between both ends of a communication session. Each end can be assured that the other end is who it is supposed to be. This is often implemented using a mutual authentication handshake when the session is established, especially between devices. Session authenticity is usually provided by a security protocol enforced for a communication session. Choosing and enforcing a protocol will provide authenticity throughout a communications session.

**Example**

You are a system administrator responsible for ensuring that the two-factor user authentication mechanism for the servers is configured correctly. You purchase and maintain the digital certificate and replace it with a new one before the old one expires. You ensure the TLS configuration settings on the web servers, VPN solution, and other components that use TLS are correct, using secure settings that address risks against attacks on the encrypted sessions [a].

**Potential Assessment Considerations**

* Is a communications protocol used that ensures the sending and receiving parties do not change during a communications session [a]?
* Are controls in place to validate the identities and information transmitted to protect against man-in-the-middle attacks, session hijacking, and insertion of false information into communications sessions [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.13.15