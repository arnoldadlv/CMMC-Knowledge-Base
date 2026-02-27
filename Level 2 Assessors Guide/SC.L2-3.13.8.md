# SC.L2-3.13.8 – Data in Transit

## Security Requirement Implement cryptographic mechanisms to prevent unauthorized disclosure of CUI during transmission unless otherwise protected by alternative physical safeguards. |

## Assessment Objectives [a] cryptographic mechanisms intended to prevent unauthorized disclosure of CUI are identified;  [b] alternative physical safeguards intended to prevent unauthorized disclosure of CUI are identified; and  [c] either cryptographic mechanisms or alternative physical safeguards are implemented to prevent unauthorized disclosure of CUI during transmission. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SC.L2-3.13.8 – DATA IN TRANSIT

### SECURITY REQUIREMENT

Implement cryptographic mechanisms to prevent unauthorized disclosure of CUI during transmission unless otherwise protected by alternative physical safeguards.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] cryptographic mechanisms intended to prevent unauthorized disclosure of CUI are identified;
:   [b] alternative physical safeguards intended to prevent unauthorized disclosure of CUI are identified; and
:   [c] either cryptographic mechanisms or alternative physical safeguards are implemented to prevent unauthorized disclosure of CUI during transmission.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and communications protection policy; procedures addressing transmission confidentiality and integrity; system security plan; system design documentation; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; system developer].

**Test**

[SELECT FROM: Cryptographic mechanisms or mechanisms supporting or implementing transmission confidentiality; organizational processes for defining and implementing alternative physical safeguards].

### DISCUSSION

This requirement applies to internal and external networks and any system components that can transmit information including servers, notebook computers, desktop computers, mobile devices, printers, copiers, scanners, and facsimile machines. Communication paths outside the physical protection of controlled boundaries are susceptible to both interception and modification. Organizations relying on commercial providers offering transmission services as commodity services rather than as fully dedicated services (i.e., services which can be highly specialized to individual customer needs), may find it difficult to obtain the necessary assurances regarding the implementation of the controls for transmission confidentiality. In such situations, organizations determine what types of confidentiality services are available in commercial telecommunication service packages. If it is infeasible or impractical to obtain the necessary safeguards and assurances of the effectiveness of the safeguards through appropriate contracting vehicles, organizations implement compensating safeguards or explicitly accept the additional risk. An example of an alternative physical safeguard is a protected distribution system (PDS) where the distribution medium is protected against electronic or physical intercept, thereby ensuring the confidentiality of the information being transmitted.

### FURTHER DISCUSSION

The intent of this practice is to ensure CUI is cryptographically protected during transit, particularly on the internet. The most common way to accomplish this is to establish a TLS tunnel between the source and destination using the most current version of TLS. This practice does not specify a mutually authenticated handshake, but mutual authentication is the most secure approach to creating a tunnel.

When CMMC requires cryptography, it is to protect the confidentiality of CUI. FIPS-validated cryptography means the cryptographic module has to have been tested and validated to meet FIPS 140-1 or-2 requirements. Simply using an approved algorithm is not sufficient – the module (software and/or hardware) used to implement the algorithm must be separately validated under FIPS 140. Accordingly, FIPS-validated cryptography is required to meet CMMC practices that protect CUI when transmitted or stored outside the protected environment of the covered contractor information system (including wireless/remote access). Encryption used for other purposes, such as within applications or devices within the protected environment of the covered contractor information system, would not need to be FIPS-validated.

This practice, SC.L2-3.13.8, requires cryptographic mechanisms be used to prevent the disclosure of CUI in-transit and leverages SC.L2-3.13.11, which specifies that the algorithms used must be FIPS-validated.

**Example**

You are a system administrator responsible for configuring encryption on all devices that contain CUI. Because your users regularly store CUI on laptops and take them out of the office, you encrypt the hard drives with a FIPS-validated encryption tool built into the operating system. For users who need to share CUI, you install a Secure FTP server to allow CUI to be transmitted in a compliant manner [a]. You verify that the server is using a FIPS- validated encryption module by checking the NIST Cryptographic Module Validation Program website [c].You turn on the “FIPS Compliance” setting for the server during configuration because that is what is required for this product in order to use only FIPS- validated cryptography [c].

**Potential Assessment Considerations**

* Are cryptographic mechanisms used to prevent unauthorized disclosure of information during transmission unless otherwise protected by alternative physical measures (e.g., PDS) [c]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.13.8