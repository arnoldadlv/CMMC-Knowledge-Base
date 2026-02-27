# AC.L2-3.1.18 – Mobile Device Connection

## Security Requirement Control connection of mobile devices. |

## Assessment Objectives [a] mobile devices that process, store, or transmit CUI are identified;  [b] mobile device connections are authorized; and  [c] mobile device connections are monitored and logged. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.18 – MOBILE DEVICE CONNECTION

### SECURITY REQUIREMENT

Control connection of mobile devices.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] mobile devices that process, store, or transmit CUI are identified;
:   [b] mobile device connections are authorized; and
:   [c] mobile device connections are monitored and logged.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; authorizations for mobile device connections to organizational systems; procedures addressing access control for mobile device usage (including restrictions); system design documentation; configuration management plan; system security plan; system audit logs and records; system configuration settings and associated documentation; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel using mobile devices to access organizational systems; system or network administrators; personnel with information security responsibilities].

**Test**

[SELECT FROM: Access control capability authorizing mobile device connections to organizational systems].

### DISCUSSION

A mobile device is a computing device that has a small form factor such that it can easily be carried by a single individual; is designed to operate without a physical connection (e.g., wirelessly transmit or receive information); possesses local, non-removable or removable data storage; and includes a self-contained power source. Mobile devices may also include voice communication capabilities, on-board sensors that allow the device to capture information, or built-in features for synchronizing local data with remote locations. Examples of mobile devices include smart phones, e-readers, and tablets.

Due to the large variety of mobile devices with different technical characteristics and capabilities, organizational restrictions may vary for the different types of devices. Usage restrictions and implementation guidance for mobile devices include: device identification and authentication; configuration management; implementation of mandatory protective software (e.g., malicious code detection, firewall); scanning devices for malicious code; updating virus protection software; scanning for critical software updates and patches; conducting primary operating system (and possibly other resident software) integrity checks; and disabling unnecessary hardware (e.g., wireless, infrared). The need to provide adequate security for mobile devices goes beyond this requirement. Many controls for mobile devices are reflected in other CUI security requirements. NIST SP 800-124 provides guidance on mobile device security.

### FURTHER DISCUSSION

Establish guidelines and acceptable practices for proper configuration, use, and management of mobile devices. Devices that process, store, or transmit CUI must be identified with a device-specific identifier. There are many different types of identifiers, and it is important to select one that can accommodate all devices and be used in a consistent manner. These identifiers are important for facilitating the required monitoring and logging function.

In addition to smartphones, consider the security of other portable devices such as e-readers and tablets.

AC.L2-3.1.16, AC.L2-3.1.17, and AC.L2-3.1.18 are complementary practices in that they all establish requirements to control the connection of mobile devices and wireless devices through the use of authentication, authorization, and encryption mechanisms.

**Example**

Your organization has a policy stating that all mobile devices, including iPads, tablets, mobile phones, and Personal Digital Assistants (PDAs), must be approved and registered with the IT department before connecting to the network. The IT department uses a Mobile Device Management solution to monitor mobile devices and enforce policies across the enterprise [b,c].

**Potential Assessment Considerations**

* Is a list of mobile devices that are permitted to process, store, or transmit CUI maintained : [a,b]?
* Is the system configured to only permit connections from identified, authorized mobile devices [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.18