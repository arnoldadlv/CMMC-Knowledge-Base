# MA.L2-3.7.3 – Equipment Sanitization

## Security Requirement Ensure equipment removed for off-site maintenance is sanitized of any CUI. |

## Assessment Objectives [a] equipment to be removed from organizational spaces for off-site maintenance is sanitized of any CUI. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## MA.L2-3.7.3 – EQUIPMENT SANITIZATION

### SECURITY REQUIREMENT

Ensure equipment removed for off-site maintenance is sanitized of any CUI.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] equipment to be removed from organizational spaces for off-site maintenance is sanitized of any CUI.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System maintenance policy; procedures addressing controlled system maintenance; maintenance records; manufacturer or vendor maintenance specifications; equipment sanitization records; media sanitization records; system security plan; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with system maintenance responsibilities; personnel with information security responsibilities; personnel responsible for media sanitization; system or network administrators].

**Test**

[SELECT FROM: Organizational processes for scheduling, performing, documenting, reviewing, approving, and monitoring maintenance and repairs for systems; organizational processes for sanitizing system components; mechanisms supporting or implementing controlled maintenance; mechanisms implementing sanitization of system components].

### DISCUSSION

This requirement addresses the information security aspects of system maintenance that are performed off-site and applies to all types of maintenance to any system component (including applications) conducted by a local or nonlocal entity (e.g., in-contract, warranty, in-house, software maintenance agreement).

NIST SP 800-88 provides guidance on media sanitization.

### FURTHER DISCUSSION

Sanitization is a process that makes access to data infeasible on media such as a hard drive. The process may overwrite the entire media with a fixed pattern such as binary zeros. In addition to clearing the data an organization could purge (e.g., degaussing, secure erasing, or disassembling) the data, or even destroy the media (e.g., incinerating, shredding, or pulverizing). Performing one of these activities ensures that the data is extremely hard to recover, thus ensuring its confidentiality.

For additional guidance on which specific sanitization actions should be taken on any specific type of media, review the description of the Purge actions given in NIST SP 800-88 Revision 1 – Guidelines for Media Sanitization.

**Example**

You manage your organization’s IT equipment. A recent DoD project has been using a storage array to house CUI. Recently, the array has experienced disk issues. After troubleshooting with the vendor, they recommend several drives be replaced in the array. Knowing the drives may contain CUI, you reference NIST 800-88 Rev. 1 and determine a strategy you can implement on the defective equipment – processing the drives with a degaussing unit [a].Once all the drives have been wiped, you document the action and ship the faulty drives to the vendor.

**Potential Assessment Considerations**

* Is there a process for sanitizing (e.g., erasing, wiping, degaussing) equipment that was used to store, process, or transmit CUI before it is removed from the facility for off-site maintenance (e.g., manufacturer or contracted maintenance support) [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.7.3