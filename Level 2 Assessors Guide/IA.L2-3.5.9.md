# IA.L2-3.5.9 – Temporary Passwords

## Security Requirement Allow temporary password use for system logons with an immediate change to a permanent password. |

## Assessment Objectives [a] an immediate change to a permanent password is required when a temporary password is used for system logon. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## IA.L2-3.5.9 – TEMPORARY PASSWORDS

### SECURITY REQUIREMENT

Allow temporary password use for system logons with an immediate change to a permanent password.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] an immediate change to a permanent password is required when a temporary password is used for system logon.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Identification and authentication policy; password policy; procedures addressing authenticator management; system security plan; system configuration settings and associated documentation; system design documentation; password configurations and associated documentation; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with authenticator management responsibilities; personnel with information security responsibilities; system or network administrators; system developers].

**Test**

[SELECT FROM: Mechanisms supporting or implementing password-based authenticator management capability].

### DISCUSSION

Changing temporary passwords to permanent passwords immediately after system logon ensures that the necessary strength of the authentication mechanism is implemented at the earliest opportunity, reducing the susceptibility to authenticator compromises.

### FURTHER DISCUSSION

Users must change their temporary passwords the first time they log in. Temporary passwords often follow a consistent style within an organization and can be more easily guessed than passwords created by the unique user. This approach to temporary passwords should be avoided.

**Example**

One of your duties as a systems administrator is to create accounts for new users. You configure all systems with user accounts to require users to change a temporary password upon initial login to a permanent password [a]. When a user logs on for the first time, they are prompted to create a unique password that meets all of the defined complexity rules.

### Potential Assessment Considerations

* Are temporary passwords only valid to allow a user to perform a password reset [a]?
* Does the system enforce an immediate password change after logon when a temporary password is issued [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.5.9