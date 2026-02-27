# IA.L2-3.5.11 – Obscure Feedback

## Security Requirement Obscure feedback of authentication information. |

## Assessment Objectives [a] authentication information is obscured during the authentication process. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## IA.L2-3.5.11 – OBSCURE FEEDBACK

### SECURITY REQUIREMENT

Obscure feedback of authentication information.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] authentication information is obscured during the authentication process.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Identification and authentication policy; procedures addressing authenticator feedback; system security plan; system design documentation; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with information security responsibilities; system or network administrators; system developers].

**Test**

[SELECT FROM: Mechanisms supporting or implementing the obscuring of feedback of authentication information during authentication].

### DISCUSSION

The feedback from systems does not provide any information that would allow unauthorized individuals to compromise authentication mechanisms. For some types of systems or system components, for example, desktop or notebook computers with relatively large monitors, the threat (often referred to as shoulder surfing) may be significant. For other types of systems or components, for example, mobile devices with small displays, this threat may be less significant, and is balanced against the increased likelihood of typographic input errors due to the small keyboards. Therefore, the means for obscuring the authenticator feedback is selected accordingly. Obscuring authenticator feedback includes displaying asterisks when users type passwords into input devices or displaying feedback for a very limited time before fully obscuring it.

### FURTHER DISCUSSION

Authentication information includes passwords. When users enter a password, the system displays a symbol, such as an asterisk, to obscure feedback preventing others from seeing the actual characters. Feedback is obscured based on a defined policy (e.g., smaller devices may briefly show characters before obscuring).

**Example**

As a system administrator, you configure your systems to display an asterisk when users enter their passwords into a computer system [a].For mobile devices, the password characters are briefly displayed to the user before being obscured. This prevents people from figuring out passwords by looking over someone’s shoulder.

### Potential Assessment Considerations

* Is the feedback immediately obscured when the authentication is presented on a larger display (e.g., desktop or notebook computers with relatively large monitors) [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.5.11