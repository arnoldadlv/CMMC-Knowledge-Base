# AC.L2-3.1.21 – Portable Storage Use

## Security Requirement Limit use of portable storage devices on external systems. |

## Assessment Objectives [a] the use of portable storage devices containing CUI on external systems is identified and documented;  [b] limits on the use of portable storage devices containing CUI on external systems are defined; and  [c] the use of portable storage devices containing CUI on external systems is limited as defined. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.21 – PORTABLE STORAGE USE

### SECURITY REQUIREMENT

Limit use of portable storage devices on external systems.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the use of portable storage devices containing CUI on external systems is identified and documented;
:   [b] limits on the use of portable storage devices containing CUI on external systems are defined; and
:   [c] the use of portable storage devices containing CUI on external systems is limited as defined.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; procedures addressing the use of external systems; system security plan; system configuration settings and associated documentation; system connection or processing agreements; account management documents; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with responsibilities for restricting or prohibiting use of organization-controlled storage devices on external systems; system or network administrators; personnel with information security responsibilities].

**Test**

[SELECT FROM: Mechanisms implementing restrictions on use of portable storage devices].

### DISCUSSION

Limits on the use of organization-controlled portable storage devices in external systems include complete prohibition of the use of such devices or restrictions on how the devices may be used and under what conditions the devices may be used. Note that while “external” typically refers to outside of the organization’s direct supervision and authority that is not always the case. Regarding the protection of CUI across an organization, the organization may have systems that process CUI and others that do not. Among the systems that process CUI there are likely access restrictions for CUI that apply between systems. Therefore, from the perspective of a given system, other systems within the organization may be considered “external" to that system.

### FURTHER DISCUSSION

A portable storage device is a system component that can be inserted or attached and easily removed from a system. It is used to store data or information. Examples of portable storage devices include:

* compact/digital video disks (CDs/DVDs);
* Universal Serial Bus (USB) drives;
* external hard disk drives;
* flash memory cards/drives; and
* floppy disks.

This practice can be implemented in two ways:

* identifying the portable storage device usage restrictions, identifying portable storage devices that may be used on external systems, identifying associated external systems on which a portable storage device may be used, and administratively (through the use of a written policy) limiting the usage of the devices to those systems; or
* configuring devices to work only when connected to a system to which the portable storage device can authenticate, limiting the devices’ use on external systems to those that the contractor has the ability to manage.

**Example**

Your organization has a written portable device usage restriction policy. It states that users can only use external storage devices such as thumb dives or external hard disks that belong to the company. When needed for a specific business function, a user checks the device out from IT and returns it to IT when no longer needed [a,b].

**Potential Assessment Considerations**

* Are the portable storage devices authorized for external use identified and documented : [a]?
* Are the circumstances defined in which portable storage devices containing CUI may be used on external systems (e.g., with management approval) [b]?
* Are limitations stipulated for the use of portable storage devices containing CUI on external systems (e.g., authorized personnel only, encrypted drives required) [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.21