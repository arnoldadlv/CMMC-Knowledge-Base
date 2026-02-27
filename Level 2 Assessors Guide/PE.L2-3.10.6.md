# PE.L2-3.10.6 – Alternative Work Sites

## Security Requirement Enforce safeguarding measures for CUI at alternate work sites. |

## Assessment Objectives [a] safeguarding measures for CUI are defined for alternate work sites; and  [b] safeguarding measures for CUI are enforced for alternate work sites. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## PE.L2-3.10.6 – ALTERNATIVE WORK SITES

### SECURITY REQUIREMENT

Enforce safeguarding measures for CUI at alternate work sites.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] safeguarding measures for CUI are defined for alternate work sites; and
:   [b] safeguarding measures for CUI are enforced for alternate work sites.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Physical and environmental protection policy; procedures addressing alternate work sites for personnel; system security plan; list of safeguards required for alternate work sites; assessments of safeguards at alternate work sites; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel approving use of alternate work sites; personnel using alternate work sites; personnel assessing controls at alternate work sites; personnel with information security responsibilities].

**Test**

[SELECT FROM: Organizational processes for security at alternate work sites; mechanisms supporting alternate work sites; safeguards employed at alternate work sites; means of communications between personnel at alternate work sites and security personnel].

### DISCUSSION

Alternate work sites may include government facilities or the private residences of employees. Organizations may define different security requirements for specific alternate work sites or types of sites depending on the work-related activities conducted at those sites. NIST SP 800-46 and NIST SP 800-114 provide guidance on enterprise and user security when teleworking.

### FURTHER DISCUSSION

Many people work from home or travel as part of their job. Define and implement safeguards to account for protection of information beyond the enterprise perimeter. Safeguards may include physical protections, such as locked file drawers, as well as electronic protections such as encryption, audit logging, and proper access controls.

**Example**

Many of your company’s project managers work remotely as they often travel to sponsor locations or even work from home. Because the projects on which they work require access to CUI, you must ensure the same level of protection is afforded as when they work in the office. You ensure that each laptop is deployed with patch management and anti-virus software protection [b]. Because data may be stored on the local hard drive, you have enabled full-disk encryption on their laptops [b]. When a remote staff member needs access to the internal network you require VPN connectivity that also disconnects the laptop from the remote network (i.e., prevents split tunneling) [b].The VPN requires multifactor authentication to verify remote users are who they claim to be [b].

**Potential Assessment Considerations**

* Do all alternate sites where CUI data is stored or processed meet the same physical security requirements as the main site [b]?
* Does the alternate processing site provide information security measures equivalent to those of the primary site [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.10.6