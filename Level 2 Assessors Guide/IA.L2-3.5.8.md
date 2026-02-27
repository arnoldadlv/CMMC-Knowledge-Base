# IA.L2-3.5.8 – Password Reuse

## Security Requirement Prohibit password reuse for a specified number of generations. |

## Assessment Objectives [a] the number of generations during which a password cannot be reused is specified; and  [b] reuse of passwords is prohibited during the specified number of generations. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## IA.L2-3.5.8 – PASSWORD REUSE

### SECURITY REQUIREMENT

Prohibit password reuse for a specified number of generations.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] the number of generations during which a password cannot be reused is specified and [b] reuse of passwords is prohibited during the specified number of generations.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Identification and authentication policy; password policy; procedures addressing authenticator management; system security plan; system design documentation; system configuration settings and associated documentation; password configurations and associated documentation; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with authenticator management responsibilities; personnel with information security responsibilities; system or network administrators; system developers].

**Test**

[SELECT FROM: Mechanisms supporting or implementing password-based authenticator management capability].

### DISCUSSION

Password lifetime restrictions do not apply to temporary passwords.

### FURTHER DISCUSSION

Individuals may not reuse their passwords for a defined period of time and a set number of passwords generated.

**Example**

You explain in your company’s security policy that changing passwords regularly provides increased security by reducing the ability of adversaries to exploit stolen or purchased passwords over an extended period. You define how often individuals can reuse their passwords and the minimum number of password generations before reuse [a]. If a user tries to reuse a password before the number of password generations has been exceeded, an error message is generated, and the user is required to enter a new password [b].

### Potential Assessment Considerations

* How many generations of password changes need to take place before a password can be reused [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.5.8