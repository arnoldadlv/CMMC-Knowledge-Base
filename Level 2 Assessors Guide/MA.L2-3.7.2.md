# MA.L2-3.7.2 – System Maintenance Control

## Security Requirement Provide controls on the tools, techniques, mechanisms, and personnel used to conduct system maintenance. |

## Assessment Objectives [a] tools used to conduct system maintenance are controlled;  [b] techniques used to conduct system maintenance are controlled;  [c] mechanisms used to conduct system maintenance are controlled; and  [d] personnel used to conduct system maintenance are controlled. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## MA.L2-3.7.2 – SYSTEM MAINTENANCE CONTROL

### SECURITY REQUIREMENT

Provide controls on the tools, techniques, mechanisms, and personnel used to conduct system maintenance.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] tools used to conduct system maintenance are controlled;
:   [b] techniques used to conduct system maintenance are controlled;
:   [c] mechanisms used to conduct system maintenance are controlled; and
:   [d] personnel used to conduct system maintenance are controlled.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System maintenance policy; procedures addressing system maintenance tools and media; maintenance records; system maintenance tools and associated documentation; maintenance tool inspection records; system security plan; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with system maintenance responsibilities; personnel with information security responsibilities].

**Test**

[SELECT FROM: Organizational processes for approving, controlling, and monitoring maintenance tools; mechanisms supporting or implementing approval, control, and monitoring of maintenance tools; organizational processes for inspecting maintenance tools; mechanisms supporting or implementing inspection of maintenance tools; organizational process for inspecting media for malicious code; mechanisms supporting or implementing inspection of media used for maintenance].

### DISCUSSION

This requirement addresses security-related issues with maintenance tools that are not within the organizational system boundaries that process, store, or transmit CUI, but are used specifically for diagnostic and repair actions on those systems. Organizations have flexibility in determining the controls in place for maintenance tools, but can include approving, controlling, and monitoring the use of such tools. Maintenance tools are potential vehicles for transporting malicious code, either intentionally or unintentionally, into a facility and into organizational systems. Maintenance tools can include hardware, software, and firmware items, for example, hardware and software diagnostic test equipment and hardware and software packet sniffers.

### FURTHER DISCUSSION

Tools used to perform maintenance must remain secure so they do not introduce viruses or other malware into your system. Controlling your maintenance techniques prevents intentional or unintentional harm to your network and systems. Additionally, the personnel responsible for maintenance activities should be supervised considering their elevated privilege on company assets.

**Example**

You are responsible for maintenance activities on your company’s machines. To avoid introducing additional vulnerability into the systems you are maintaining, you make sure that all maintenance tools are approved and their usage is monitored and controlled [a,b]. You ensure the tools are kept current and up-to-date [a]. You and your backup are the only people authorized to use these tools and perform system maintenance [d].

**Potential Assessment Considerations**

* Are physical or logical access controls used to limit access to maintenance tools to authorized personnel [a]?
* Are physical or logical access controls used to limit access to system documentation and organizational maintenance process documentation to authorized personnel [b]?
* Are physical or logical access controls used to limit access to automated mechanisms (e.g., automated scripts, scheduled jobs) to authorized personnel [c]?
* Are physical or logical access controls used to limit access to the system entry points that enable maintenance (e.g., administrative portals, local and remote console access, and physical equipment panels) to authorized personnel [d]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.7.2