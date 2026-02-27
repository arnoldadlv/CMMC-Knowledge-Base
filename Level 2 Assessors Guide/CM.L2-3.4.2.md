# CM.L2-3.4.2 – Security Configuration Enforcement

## Security Requirement Establish and enforce security configuration settings for information technology products employed in organizational systems. |

## Assessment Objectives [a] security configuration settings for information technology products employed in the system are established and included in the baseline configuration; and  [b] security configuration settings for information technology products employed in the system are enforced. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## CM.L2-3.4.2 – SECURITY CONFIGURATION ENFORCEMENT

### SECURITY REQUIREMENT

Establish and enforce security configuration settings for information technology products employed in organizational systems.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] security configuration settings for information technology products employed in the system are established and included in the baseline configuration; and
:   [b] security configuration settings for information technology products employed in the system are enforced.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Configuration management policy; baseline configuration; procedures addressing configuration settings for the system; configuration management plan; system security plan; system design documentation; system configuration settings and associated documentation; security configuration checklists; evidence supporting approved deviations from established configuration settings; change control records; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with security configuration management responsibilities; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Organizational processes for managing configuration settings; mechanisms that implement, monitor, and/or control system configuration settings; mechanisms that identify and/or document deviations from established configuration settings; processes for managing baseline configurations; mechanisms supporting configuration control of baseline configurations].

### DISCUSSION

Configuration settings are the set of parameters that can be changed in hardware, software, or firmware components of the system that affect the security posture or functionality of the system. Information technology products for which security-related configuration settings can be defined include mainframe computers, servers, workstations, input and output devices (e.g., scanners, copiers, and printers), network components (e.g., firewalls, routers, gateways, voice and data switches, wireless access points, network appliances, sensors), operating systems, middleware, and applications.

Security parameters are those parameters impacting the security state of systems including the parameters required to satisfy other security requirements. Security parameters include: registry settings; account, file, directory permission settings; and settings for functions, ports, protocols, and remote connections. Organizations establish organization-wide configuration settings and subsequently derive specific configuration settings for systems. The established settings become part of the systems configuration baseline.

Common secure configurations (also referred to as security configuration checklists, lockdown and hardening guides, security reference guides, security technical implementation guides) provide recognized, standardized, and established benchmarks that stipulate secure configuration settings for specific information technology platforms/products and instructions for configuring those system components to meet operational requirements. Common secure configurations can be developed by a variety of organizations including information technology product developers, manufacturers, vendors, consortia, academia, industry, federal agencies, and other organizations in the public and private sectors.

NIST SP 800-70 and SP 800-128 provide guidance on security configuration settings.

### FURTHER DISCUSSION

Information security is an integral part of a company’s configuration management process. Security-related configuration settings are customized to satisfy the company’s security requirements and are applied them to all systems once tested and approved. The configuration settings must reflect the most restrictive settings that are appropriate for the system. Any required deviations from the baseline are reviewed, documented, and approved.

**Example**

You manage baseline configurations for your company’s systems. As part of this, you download a secure configuration guide for each of your asset types (servers, workstations, network components, operating systems, middleware, and applications) from a well-known and trusted IT security organization. You then apply all of the settings that you can while still ensuring the assets can perform the role for which they are needed. Once you have the configuration settings identified and tested, you document them to ensure all applicable machines can be configured the same way [a,b].

**Potential Assessment Considerations**

* Do security settings reflect the most restrictive settings appropriate [a]?
* Are changes or deviations to security settings documented [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.4.2