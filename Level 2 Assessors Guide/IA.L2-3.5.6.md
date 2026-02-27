# IA.L2-3.5.6 – Identifier Handling

## Security Requirement Disable identifiers after a defined period of inactivity. |

## Assessment Objectives [a] a period of inactivity after which an identifier is disabled is defined; and  [b] identifiers are disabled after the defined period of inactivity. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## IA.L2-3.5.6 – IDENTIFIER HANDLING

### SECURITY REQUIREMENT

Disable identifiers after a defined period of inactivity.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] a period of inactivity after which an identifier is disabled is defined; and
:   [b] identifiers are disabled after the defined period of inactivity.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Identification and authentication policy; procedures addressing identifier management; procedures addressing account management; system security plan; system design documentation; system configuration settings and associated documentation; list of system accounts; list of identifiers generated from physical access control devices; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with identifier management responsibilities; personnel with information security responsibilities; system or network administrators; system developers].

**Test**

[SELECT FROM: Mechanisms supporting or implementing identifier management].

### DISCUSSION

Inactive identifiers pose a risk to organizational information because attackers may exploit an inactive identifier to gain undetected access to organizational devices. The owners of the inactive accounts may not notice if unauthorized access to the account has been obtained.

### FURTHER DISCUSSION

Identifiers are uniquely associated with an individual, account, process, or device. An inactive identifier is one that has not been used for a defined extended period of time. For example, a user account may be needed for a certain time to allow for transition of business processes to existing or new staff. Once use of the identifier is no longer necessary, it should be disabled as soon as possible. Failure to maintain awareness of accounts that are no longer needed yet still active could allow an adversary to exploit IT services.

**Example**

One of your responsibilities is to enforce your company’s inactive account policy: any account that has not been used in the last 45 days must be disabled [a]. You enforce this by writing a script that runs once a day to check the last login date for each account and generates a report of the accounts with no login records for the last 45 days. After reviewing the report, you notify each inactive employee’s supervisor and disable the account [b].

### Potential Assessment Considerations

* Are user accounts or identifiers monitored for inactivity [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.5.6