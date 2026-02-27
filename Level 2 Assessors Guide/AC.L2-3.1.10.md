# AC.L2-3.1.10 – Session Lock

## Security Requirement Use session lock with pattern-hiding displays to prevent access and viewing of data after a period of inactivity. |

## Assessment Objectives [a] the period of inactivity after which the system initiates a session lock is defined;  [b] access to the system and viewing of data is prevented by initiating a session lock after the defined period of inactivity; and  [c] previously visible information is concealed via a pattern-hiding display after the defined period of inactivity. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.10 – SESSION LOCK

### SECURITY REQUIREMENT

Use session lock with pattern-hiding displays to prevent access and viewing of data after a period of inactivity.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the period of inactivity after which the system initiates a session lock is defined;
:   [b] access to the system and viewing of data is prevented by initiating a session lock after the defined period of inactivity; and
:   [c] previously visible information is concealed via a pattern-hiding display after the defined period of inactivity.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; procedures addressing session lock; procedures addressing identification and authentication; system design documentation; system configuration settings and associated documentation; system security plan; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; system developers].

**Test**

[SELECT FROM: Mechanisms implementing access control policy for session lock].

### DISCUSSION

Session locks are temporary actions taken when users stop work and move away from the immediate vicinity of the system but do not want to log out because of the temporary nature of their absences. Session locks are implemented where session activities can be determined, typically at the operating system level (but can also be at the application level). Session locks are not an acceptable substitute for logging out of the system, for example, if organizations require users to log out at the end of the workday.

Pattern-hiding displays can include static or dynamic images, for example, patterns used with screen savers, photographic images, solid colors, clock, battery life indicator, or a blank screen, with the additional caveat that none of the images convey controlled unclassified information.

### FURTHER DISCUSSION

Session locks can be initiated by the user or, more fundamentally, enabled automatically when the system has been idle for a period of time, for example, five minutes. Session locks are a quick way to prevent unauthorized use of the systems without having a user log off. Minimum configuration requirements are left up to the organization to define.

A locked session shows pattern-hiding information on the screen to mask the data on the display.

**Example**

You are a system administrator. You notice that employees leave their offices without locking their computers. Sometimes their screens display sensitive company information. You configure all machines to lock after five minutes of inactivity [a,b]. You also remind your coworkers to lock their systems when they walk away [a].

**Potential Assessment Considerations**

* Does the session lock hide previously visible information (e.g., replacing what was visible with a lock screen or screensaver that does not include sensitive information) [c]?
* If session locks are not managed centrally, how are all computer users made aware of the requirements and how to configure them [a,b,c]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.10