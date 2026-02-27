# SC.L2-3.13.12 – Collaborative Device Control

## Security Requirement Prohibit remote activation of collaborative computing devices and provide indication of devices in use to users present at the device. |

## Assessment Objectives [a] collaborative computing devices are identified;  [b] collaborative computing devices provide indication to users of devices in use; and  [c] remote activation of collaborative computing devices is prohibited. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SC.L2-3.13.12 – COLLABORATIVE DEVICE CONTROL

### SECURITY REQUIREMENT

Prohibit remote activation of collaborative computing devices and provide indication of devices in use to users present at the device.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] collaborative computing devices are identified;
:   [b] collaborative computing devices provide indication to users of devices in use; and
:   [c] remote activation of collaborative computing devices is prohibited.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and communications protection policy; procedures addressing collaborative computing; access control policy and procedures; system security plan; system design documentation; system audit logs and records; system configuration settings and associated documentation; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; system developer; personnel with responsibilities for managing collaborative computing devices].

**Test**

[SELECT FROM: Mechanisms supporting or implementing management of remote activation of collaborative computing devices; mechanisms providing an indication of use of collaborative computing devices].

### DISCUSSION

Collaborative computing devices include networked white boards, cameras, and microphones. Indication of use includes signals to users when collaborative computing devices are activated. Dedicated video conferencing systems, which rely on one of the participants calling or connecting to the other party to activate the video conference, are excluded.

### FURTHER DISCUSSION

Notification that a device is in use can include an indicator light that turns on or a specific text window that appears on screen. If a device does not have the means to alert a user when in use, the organization should provide manual means. Manual means can include, as necessary:

* paper notification on entryways; and
* locking entryways when a collaborative computing device is in use.

This practice is not intended to include technologies that enable users to share the contents of their computer screens via the internet.

**Example**

A group of remote employees at your company routinely collaborate using cameras and microphones attached to their computers [a]. To prevent the misuse of these devices, you disable the ability to turn on cameras or microphones remotely [c]. You ensure the machines alert users when the camera or microphone are in use with a light beside the camera and an onscreen notification [b]. Although remote activation is blocked, this enables users to see if the devices are active.

**Potential Assessment Considerations**

* Are the collaborative computing devices configured to provide indication to users when in use (e.g., a light, text notification, or audio tone) or are users alerted before entering a space (e.g., written notice posted outside the space) where they are in use [b]?
* Are the collaborative computing devices configured to prevent them from being turned on without user interaction or consent [c]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.13.12