# IA.L2-3.5.3 – Multifactor Authentication

## Security Requirement Use multifactor authentication for local and network access to privileged accounts and for network access to non-privileged accounts. |

## Assessment Objectives [a] privileged accounts are identified;  [b] multifactor authentication is implemented for local access to privileged accounts;  [c] multifactor authentication is implemented for network access to privileged accounts; and  [d] multifactor authentication is implemented for network access to non-privileged accounts. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## IA.L2-3.5.3 – MULTIFACTOR AUTHENTICATION

### SECURITY REQUIREMENT

Use multifactor authentication for local and network access to privileged accounts and for network access to non-privileged accounts.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] privileged accounts are identified;
:   [b] multifactor authentication is implemented for local access to privileged accounts;
:   [c] multifactor authentication is implemented for network access to privileged accounts; and
:   [d] multifactor authentication is implemented for network access to non-privileged accounts.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Identification and authentication policy; procedures addressing user identification and authentication; system security plan; system design documentation; system configuration settings and associated documentation; system audit logs and records; list of system accounts; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with authenticator management responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Mechanisms supporting or implementing authenticator management capability].

### DISCUSSION

Multifactor authentication requires the use of two or more different factors to authenticate. The factors are defined as something you know (e.g., password, personal identification number [PIN]); something you have (e.g., cryptographic identification device, token); or something you are (e.g., biometric).Multifactor authentication solutions that feature physical authenticators include hardware authenticators providing time-based or challenge- response authenticators and smart cards. In addition to authenticating users at the system level (i.e., at logon), organizations may also employ authentication mechanisms at the application level, when necessary, to provide increased information security. Access to organizational systems is defined as local access or network access. Local access is any access to organizational systems by users (or processes acting on behalf of users) where such access is obtained by direct connections without the use of networks. Network access is access to systems by users (or processes acting on behalf of users) where such access is obtained through network connections (i.e., nonlocal accesses). Remote access is a type of network access that involves communication through external networks. The use of encrypted virtual private networks for connections between organization-controlled and non-organization controlled endpoints may be treated as internal networks with regard to protecting the confidentiality of information.

NIST SP 800-63-3 provides guidance on digital identities.

### FURTHER DISCUSSION

Implement a combination of two or more factors of authentication to verify privileged account holders’ identity regardless of how the user is accessing the account. Implement a combination of two or more factors for non-privileged users accessing the system over a network.

The implementation of multi-factor authentication will depend on the environment and business needs. Although two-factor authentication directly on the computer is most common, there are situations (e.g., multi-factor identification for a mission system that cannot be altered) where additional technical or physical solutions can provide security. Multifactor authentication is not required for access to mobile devices such as smartphones or tablets – which are not considered to be network devices or information systems.

This practice, IA.L2-3.5.3, requires multifactor authentication for network access to non- privileged accounts and complements five other practices dealing with remote access (AC.L2-3.1.12, AC.L2-3.1.14, AC.L2-3.1.13, AC.L2-3.1.15, and MA.L2-3.7.5:

* AC.L2-3.1.12 requires the control of remote access sessions.
* AC.L2-3.1.14 limits remote access to specific access control points.
* AC.L2-3.1.13 requires the use of cryptographic mechanisms when enabling remote sessions.
* AC.L2-3.1.15 requires authorization for privileged commands executed during a remote.
* Finally, MA.L2-3.7.5 requires the addition of multifactor authentication for remote maintenance sessions.

This practice, IA.L2-3.5.3, also enhances IA.L1-3.5.2, which is a requirement for a less rigorous form of user authentication.

**Example**

You decide to implement multifactor authentication (MFA) to improve security of your network. Your first step is enabling MFA on VPN access to your internal network [c,d]. When users initiate remote access, they will be prompted for the additional authentication factor.

Because you also use a cloud-based email solution, you require MFA for access to that resource as well [c,d]. Finally, you enable MFA for both local and network logins for the system administrator accounts used to patch and manage servers [a,b,c].

### Potential Assessment Considerations

* Does the system uniquely identify and authenticate users, including privileged accounts [b,c,d]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.5.3