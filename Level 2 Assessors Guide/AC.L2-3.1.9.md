# AC.L2-3.1.9 – Privacy & Security Notices

## Security Requirement Provide privacy and security notices consistent with applicable CUI rules. |

## Assessment Objectives [a] privacy and security notices required by CUI-specified rules are identified, consistent, and associated with the specific CUI category; and  [b] privacy and security notices are displayed. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.9 – PRIVACY & SECURITY NOTICES

### SECURITY REQUIREMENT

Provide privacy and security notices consistent with applicable CUI rules.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] privacy and security notices required by CUI-specified rules are identified, consistent, and associated with the specific CUI category; and
:   [b] privacy and security notices are displayed.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Privacy and security policies, procedures addressing system use notification; documented approval of system use notification messages or banners; system audit logs and records; system design documentation; user acknowledgements of notification message or banner; system security plan; system use notification messages; system configuration settings and associated documentation; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; personnel with responsibility for providing legal advice; system developers].

**Test**

[SELECT FROM: Mechanisms implementing system use notification].

### DISCUSSION

System use notifications can be implemented using messages or warning banners displayed before individuals log in to organizational systems. System use notifications are used only for access via logon interfaces with human users and are not required when such human interfaces do not exist. Based on a risk assessment, organizations consider whether a secondary system use notification is needed to access applications or other system resources after the initial network logon. Where necessary, posters or other printed materials may be used in lieu of an automated system banner. Organizations consult with the Office of General Counsel for legal review and approval of warning banner content.

### FURTHER DISCUSSION

Every system containing or providing access to CUI has legal requirements concerning user privacy and security notices. One method of addressing this requirement is the use of a system-use notification banner that displays the legal requirements of using the system. Users may be required to click to agree to the displayed requirements of using the system each time they log on to the machine. This agreement can be used in the civil and/or criminal prosecution of an attacker that violates the terms.

The legal notification should meet all applicable requirements. At a minimum, the notice should inform the user that:

* information system usage may be monitored or recorded, and is subject to audit;
* unauthorized use of the information systems is prohibited;
* unauthorized use is subject to criminal and civil penalties;
* use of the information system affirms consent to monitoring and recording;
* the information system contains CUI with specific requirements imposed by the Department of Defense; and
* use of the information system may be subject to other specified requirements associated with certain types of CUI such as Export Controlled information.

**Example**

You are setting up IT equipment including a database server that will contain CUI. You have worked with legal counsel to draft a notification. It contains both general and specific CUI security and privacy requirements [a]. The system displays the required security and privacy information before anyone logs on to your organization’s computers that contain or provide access to CUI [b].

For more information on CUI, refer to <https://www.dodcui.mil/>.

**Potential Assessment Considerations**

* Are requirements identified for privacy and security notices, and do the implemented practices match those identified requirements [a,b]? Discrepancies may indicate a deficient process and/or an incomplete practice.
* Are there any special requirements associated with the specific CUI category [a]?
* Are appropriate notices displayed in areas where paper-based CUI is stored and processed [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.9