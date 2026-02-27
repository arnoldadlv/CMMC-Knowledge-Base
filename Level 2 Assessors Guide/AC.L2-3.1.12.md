# AC.L2-3.1.12 – Control Remote Access

## Security Requirement Monitor and control remote access sessions. |

## Assessment Objectives [a] remote access sessions are permitted;  [b] the types of permitted remote access are identified;  [c] remote access sessions are controlled; and  [d] remote access sessions are monitored. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.12 – CONTROL REMOTE ACCESS

### SECURITY REQUIREMENT

Monitor and control remote access sessions.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] remote access sessions are permitted;
:   [b] the types of permitted remote access are identified;
:   [c] remote access sessions are controlled; and
:   [d] remote access sessions are monitored.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; procedures addressing remote access implementation and usage (including restrictions); configuration management plan; system security plan; system design documentation; system configuration settings and associated documentation; remote access authorizations; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with responsibilities for managing remote access connections; system or network administrators; personnel with information security responsibilities].

**Test**

[SELECT FROM: Remote access management capability for the system].

### DISCUSSION

Remote access is access to organizational systems by users (or processes acting on behalf of users) communicating through external networks (e.g., the internet).Remote access methods include dial-up, broadband, and wireless. Organizations often employ encrypted virtual private networks (VPNs) to enhance confidentiality over remote connections. The use of encrypted VPNs does not make the access non-remote; however, the use of VPNs, when adequately provisioned with appropriate control (e.g., employing encryption techniques for confidentiality protection), may provide sufficient assurance to the organization that it can effectively treat such connections as internal networks. VPNs with encrypted tunnels can affect the capability to adequately monitor network communications traffic for malicious code.

Automated monitoring and control of remote access sessions allows organizations to detect cyber-attacks and help to ensure ongoing compliance with remote access policies by auditing connection activities of remote users on a variety of system components (e.g., servers, workstations, notebook computers, smart phones, and tablets).

NIST SP 800-46, SP 800-77, and SP 800-113 provide guidance on secure remote access and virtual private networks.

### FURTHER DISCUSSION

Remote access connections pass through untrusted networks and therefore require proper security controls such as encryption to ensure data confidentiality. Initialization of all remote sessions should ensure that only authorized users and devices are connecting. After the remote session is established, the connection is monitored to track who is accessing the network remotely and what files are being accessed during the session.

Remote access sessions can encompass more than just remote connections back to a headquarters network. Access to cloud-based email providers or server infrastructures also are relevant to this practice if those environments contain CUI.

This practice, AC.L2-3.1.12, requires the control of remote access sessions and complements five other practices dealing with remote access (AC.L2-3.1.14, AC.L2-3.1.13, AC.L2-3.1.15, IA.L2-3.5.3, and MA.L2-3.7.5):

* AC.L2-3.1.14 limits remote access to specific access control points.
* AC.L2-3.1.13 requires the use of cryptographic mechanisms when enabling remote sessions.
* AC.L2-3.1.15 requires authorization for privileged commands executed during a remote session.
* IA.L2-3.5.3 requires multifactor authentication for network access to non-privileged accounts.
* Finally, MA.L2-3.7.5 requires the addition of multifactor authentication for remote maintenance sessions.

**Example**

You often need to work from remote locations, such as your home or client sites, and you are permitted to access your organization’s internal networks from those remote locations [a].A system administrator issues you a company laptop with VPN software installed, which is required to connect to the networks remotely [b]. After the laptop connects to the VPN server, you must accept a privacy notice that states that the company’s security department may monitor the connection. This monitoring is achieved through the analysis of data from sensors on the network notifying IT if issues arise. The security department may also review audit logs to see who is connecting remotely, when, and what information they are accessing [d]. During session establishment, the message “Verifying Compliance” means software like a Device Health Check (DHC) application is checking the remote device to ensure it meets the established requirements to connect [c].

**Potential Assessment Considerations**

* Do policies identify when remote access is permitted and what methods must be used : [a,b]?
* Are systems configured to permit only approved remote access sessions (e.g., disallow remote access sessions by default) [c]?
* Are automated or manual mechanisms employed for monitoring remote connections? If the monitoring is manual, does it occur at a frequency commensurate with the level of risk [d]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.12