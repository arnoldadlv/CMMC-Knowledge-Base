# SC.L2-3.13.10 – Key Management

## Security Requirement Establish and manage cryptographic keys for cryptography employed in organizational systems. |

## Assessment Objectives [a] cryptographic keys are established whenever cryptography is employed; and  [b] cryptographic keys are managed whenever cryptography is employed. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SC.L2-3.13.10 – KEY MANAGEMENT

### SECURITY REQUIREMENT

Establish and manage cryptographic keys for cryptography employed in organizational systems.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] cryptographic keys are established whenever cryptography is employed; and
:   [b] cryptographic keys are managed whenever cryptography is employed.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and communications protection policy; procedures addressing cryptographic key establishment and management; system security plan; system design documentation; cryptographic mechanisms; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; personnel with responsibilities for cryptographic key establishment and management].

**Test**

[SELECT FROM: Mechanisms supporting or implementing cryptographic key establishment and management].

### DISCUSSION

Cryptographic key management and establishment can be performed using manual procedures or mechanisms supported by manual procedures. Organizations define key management requirements in accordance with applicable federal laws, Executive Orders, policies, directives, regulations, and standards specifying appropriate options, levels, and parameters.

NIST SP 800-56A and NIST SP 800-57-1 provide guidance on cryptographic key management and key establishment.

### FURTHER DISCUSSION

Develop processes and technical mechanisms to protect the cryptographic keys’ confidentiality, authenticity, and authorized use in accordance with industry standards and regulations. Key management systems provide oversight, assurance, and the capability to demonstrate the cryptographic keys are created in a secure manner and protected from loss or misuse throughout their lifecycle (e.g., active, expired, revoked). For a small number of keys, this can be accomplished with manual procedures and mechanisms. As the number of keys and cryptographic units increase, automation and tool support will be required.

The first intent of this practice is to ensure cryptographic keys are properly created in a secure manner that prevents them from being reproduced by an adversary. The second intent of this practice is to ensure cryptographic keys are managed in a secure manner that prevents them from being stolen by an adversary.

Key establishment involves the creation of keys and coordination among parties that will use the keys of the methodology for generating the final keying material. This is discussed in detail in SP 800-56A, B, and C.

Key management involves protecting keys when they are distributed, when they are stored, when they are being used, and when they are being recovered.

Key establishment best practices are identified in NIST SP 800-56A, B, and C. Key management best practices are identified in NIST SP 800-57 Parts 1, 2, and 3.

This practice, SC.L2-3.13.10, complements AC.L2-3.1.19 by specifying that any cryptographic keys in use must be protected.

**Example 1**

You are a system administrator responsible for providing key management. You have generated a public-private key pair to exchange CUI [a]. You require all system administrators to read the key management policy before you allow them to install the private key on their machines [b]. No one else is allowed to know or have a copy of the private key per the policy. You provide the public key to the other parties who will be sending you CUI and test the Public Key Infrastructure (PKI) to ensure the encryption is working [a]. You set a revocation period of one year on all your certificates per organizational policy [b].

**Example 2**

You encrypt all of your company’s computers using the disk encryption utility built into the operating system. As you configure encryption on each device, it generates a cryptographic key. You associate each key with the correct computer in your inventory spreadsheet and restrict access to the spreadsheet to the system administrators whose work role requires them to manage the computers [b].

**Potential Assessment Considerations**

* Are cryptographic keys established whenever cryptography is employed (e.g., digital signatures, authentication, authorization, transport, or other cryptographic mechanisms) [a]?
* Are cryptographic keys maintained whenever cryptography is employed (e.g., key storage, backup, recovery, revocation, destruction, etc.) [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.13.10