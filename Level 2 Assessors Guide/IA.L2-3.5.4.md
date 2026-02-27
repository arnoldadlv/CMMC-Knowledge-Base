# IA.L2-3.5.4 – Replay-Resistant Authentication

## Security Requirement Employ replay-resistant authentication mechanisms for network access to privileged and non-privileged accounts. |

## Assessment Objectives [a] replay-resistant authentication mechanisms are implemented for network account access to privileged and non-privileged accounts. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## IA.L2-3.5.4 – REPLAY-RESISTANT AUTHENTICATION

### SECURITY REQUIREMENT

Employ replay-resistant authentication mechanisms for network access to privileged and non-privileged accounts.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] replay-resistant authentication mechanisms are implemented for network account access to privileged and non-privileged accounts.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Identification and authentication policy; procedures addressing user identification and authentication; system security plan; system design documentation; system configuration settings and associated documentation; system audit logs and records; list of privileged system accounts; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with system operations responsibilities; personnel with account management responsibilities; personnel with information security responsibilities; system or network administrators; system developers].

**Test**

[SELECT FROM: Mechanisms supporting or implementing identification and authentication capability or replay resistant authentication mechanisms].

### DISCUSSION

Authentication processes resist replay attacks if it is impractical to successfully authenticate by recording or replaying previous authentication messages. Replay-resistant techniques include protocols that use nonces or challenges such as time synchronous or challenge- response one-time authenticators.

NIST SP 800-63-3 provides guidance on digital identities.

### FURTHER DISCUSSION

When insecure protocols are used for access to computing resources, an adversary may be able to capture login information and immediately reuse (replay) it for other purposes. It is important to use mechanisms that resist this technique.

**Example**

To protect your IT infrastructure, you understand that the methods for authentication must not be easily copied and re-sent to your systems by an adversary. You select Kerberos for authentication because of its built-in resistance to replay attacks. As a next step you upgrade all of your web applications to require Transport Layer Security (TLS), which also is replay- resistant. Your use of MFA to protect remote access also confers some replay resistance.

### Potential Assessment Considerations

* Are only anti-replay authentication mechanisms used [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.5.4