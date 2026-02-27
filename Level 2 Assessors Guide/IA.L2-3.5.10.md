# IA.L2-3.5.10 – Cryptographically-Protected Passwords

## Security Requirement Store and transmit only cryptographically-protected passwords. |

## Assessment Objectives [a] passwords are cryptographically protected in storage; and  [b] passwords are cryptographically protected in transit. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## IA.L2-3.5.10 – CRYPTOGRAPHICALLY-PROTECTED PASSWORDS

### SECURITY REQUIREMENT

Store and transmit only cryptographically-protected passwords.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] passwords are cryptographically protected in storage; and
:   [b] passwords are cryptographically protected in transit.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Identification and authentication policy; system security plan; procedures addressing authenticator management; procedures addressing user identification and authentication; system design documentation; list of system authenticator types; system configuration settings and associated documentation; change control records associated with managing system authenticators; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with authenticator management responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Mechanisms supporting or implementing authenticator management capability].

### DISCUSSION

Cryptographically-protected passwords use salted one-way cryptographic hashes of passwords.

See NIST Cryptographic Standards and Guidelines.

### FURTHER DISCUSSION

All passwords must be cryptographically protected using a one-way function for storage and transmission. This type of protection changes passwords into another form, or a hashed password. A one-way transformation makes it theoretically impossible to turn the hashed password back into the original password, but inadequate complexity (IA.L2-3.5.7) may still facilitate offline cracking of hashes.

**Example**

You are responsible for managing passwords for your organization. You protect all passwords with a one-way transformation, or hashing, before storing them. Passwords are never transmitted across a network unencrypted [a,b].

### Potential Assessment Considerations

* Are passwords prevented from being stored in reversible encryption form in any company systems [a]?
* Are passwords stored as one-way hashes constructed from passwords [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.5.10