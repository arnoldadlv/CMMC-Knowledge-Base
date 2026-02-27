# IA.L2-3.5.7 – Password Complexity

## Security Requirement Enforce a minimum password complexity and change of characters when new passwords are created. |

## Assessment Objectives [a] password complexity requirements are defined;  [b] password change of character requirements are defined;  [c] minimum password complexity requirements as defined are enforced when new passwords are created; and  [d] minimum password change of character requirements as defined are enforced when new passwords are created. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## IA.L2-3.5.7 – PASSWORD COMPLEXITY

### SECURITY REQUIREMENT

Enforce a minimum password complexity and change of characters when new passwords are created.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] password complexity requirements are defined;
:   [b] password change of character requirements are defined;
:   [c] minimum password complexity requirements as defined are enforced when new passwords are created; and
:   [d] minimum password change of character requirements as defined are enforced when new passwords are created.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Identification and authentication policy; password policy; procedures addressing authenticator management; system security plan; system configuration settings and associated documentation; system design documentation; password configurations and associated documentation; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with authenticator management responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Mechanisms supporting or implementing authenticator management capability].

### DISCUSSION

This requirement applies to single-factor authentication of individuals using passwords as individual or group authenticators, and in a similar manner, when passwords are used as part of multifactor authenticators. The number of changed characters refers to the number of changes required with respect to the total number of positions in the current password. To mitigate certain brute force attacks against passwords, organizations may also consider salting passwords.

### FURTHER DISCUSSION

Password complexity means using different types of characters as well as a specified number of characters. This applies to both the creation of new passwords and the modification of existing passwords. Characters to manage complexity include numbers, lowercase and uppercase letters, and symbols. Minimum complexity requirements are left up to the organization to define. Define the lowest level of password complexity required. Define the number of characters that must be changed when an existing password is changed. Enforce these rules for all passwords. Salting passwords adds a string of random characters (salt) to a password prior to hashing. This ensures the randomness of the resulting hash value.

**Example**

You work with management to define password complexity rules and ensure they are listed in the company’s security policy. You define and enforce a minimum number of characters for each password and ensure that a certain number of characters must be changed when updating passwords [a,b]. Characters include numbers, lowercase and uppercase letters, and symbols [a]. These rules help create hard-to-guess passwords, which help to secure your network.

### Potential Assessment Considerations

* Is a degree of complexity specified for passwords, (e.g., are account passwords a minimum of 12 characters and a mix of upper/lower case, numbers, and special characters), including minimum requirements for each type [a,b,c]?
* Is a change of characters required when new passwords are created [d]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.5.7