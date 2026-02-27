# MP.L2-3.8.5 – Media Accountability

## Security Requirement Control access to media containing CUI and maintain accountability for media during transport outside of controlled areas. |

## Assessment Objectives [a] access to media containing CUI is controlled; and  [b] accountability for media containing CUI is maintained during transport outside of controlled areas. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## MP.L2-3.8.5 – MEDIA ACCOUNTABILITY

### SECURITY REQUIREMENT

Control access to media containing CUI and maintain accountability for media during transport outside of controlled areas.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] access to media containing CUI is controlled; and
:   [b] accountability for media containing CUI is maintained during transport outside of controlled areas.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System media protection policy; procedures addressing media storage; physical and environmental protection policy and procedures; access control policy and procedures; system security plan; system media; designated controlled areas; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with system media protection and storage responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Organizational processes for storing media; mechanisms supporting or implementing media storage and media protection].

### DISCUSSION

Controlled areas are areas or spaces for which organizations provide physical or procedural controls to meet the requirements established for protecting systems and information. Controls to maintain accountability for media during transport include locked containers and cryptography. Cryptographic mechanisms can provide confidentiality and integrity protections depending upon the mechanisms used. Activities associated with transport include the actual transport as well as those activities such as releasing media for transport and ensuring that media enters the appropriate transport processes. For the actual transport, authorized transport and courier personnel may include individuals external to the organization. Maintaining accountability of media during transport includes restricting transport activities to authorized personnel and tracking and obtaining explicit records of transport activities as the media moves through the transportation system to prevent and detect loss, destruction, or tampering.

### FURTHER DISCUSSION

CUI is protected in both physical and digital formats. Physical control can be accomplished using traditional concepts like restricted access to physical locations or locking papers in a desk or filing cabinet. The digitization of data makes access to CUI much easier. CUI can be stored and transported on magnetic disks, tapes, USB drives, CD-ROMs, and so on. This makes digital CUI data very portable. It is important for an organization to apply mechanisms to prevent unauthorized access to CUI due to ease of transport.

**Example**

Your team has recently completed configuring a server for a DoD customer. The customer has asked that it be ready to plug in and use. An application installed on the server contains data that is considered CUI. You box the server for shipment using tamper-evident packaging and label it with the specific recipient for the shipment [b]. You select a reputable shipping service so you will get a tracking number to monitor the progress. Once the item is shipped, you send the recipients the tracking number so they can monitor and ensure prompt delivery at their facility.

**Potential Assessment Considerations**

* Do only approved individuals have access to media containing CUI [a]?
* Is access to the media containing CUI recorded in an audit log [b]?
* Is all CUI data on media encrypted or physically locked prior to transport outside of secure locations [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.8.5