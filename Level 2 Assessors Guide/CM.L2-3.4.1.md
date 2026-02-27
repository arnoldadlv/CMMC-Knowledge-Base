# CM.L2-3.4.1 – System Baselining

## Security Requirement Establish and maintain baseline configurations and inventories of organizational systems (including hardware, software, firmware, and documentation) throughout the respective system development life cycles. |

## Assessment Objectives [a] a baseline configuration is established;  [b] the baseline configuration includes hardware, software, firmware, and documentation;  [c] the baseline configuration is maintained (reviewed and updated) throughout the system development life cycle;  [d] a system inventory is established;  [e] the system inventory includes hardware, software, firmware, and documentation; and  [f] the inventory is maintained (reviewed and updated) throughout the system development life cycle. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## CM.L2-3.4.1 – SYSTEM BASELINING

### SECURITY REQUIREMENT

Establish and maintain baseline configurations and inventories of organizational systems (including hardware, software, firmware, and documentation) throughout the respective system development life cycles.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] a baseline configuration is established;
:   [b] the baseline configuration includes hardware, software, firmware, and documentation;
:   [c] the baseline configuration is maintained (reviewed and updated) throughout the system development life cycle;
:   [d] a system inventory is established;
:   [e] the system inventory includes hardware, software, firmware, and documentation; and
:   [f] the inventory is maintained (reviewed and updated) throughout the system development life cycle.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Configuration management policy; procedures addressing the baseline configuration of the system; procedures addressing system inventory; system security plan; configuration management plan; system inventory records; inventory review and update records; enterprise architecture documentation; system design documentation; system architecture and configuration documentation; system configuration settings and associated documentation; change control records; system component installation records; system component removal records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with configuration management responsibilities; personnel with responsibilities for establishing the system inventory; personnel with responsibilities for updating the system inventory; personnel with information security responsibilities; system or network administrators].

**Test**

[SELECT FROM: Organizational processes for managing baseline configurations; mechanisms supporting configuration control of the baseline configuration; organizational processes for developing and documenting an inventory of system components; organizational processes for updating inventory of system components; mechanisms supporting or implementing the system inventory; mechanisms implementing updating of the system inventory].

### DISCUSSION

This requirement establishes and maintains baseline configurations for systems and system components including for system communications and connectivity. Baseline configurations are documented, formally reviewed, and agreed-upon sets of specifications for systems or configuration items within those systems. Baseline configurations serve as a basis for future builds, releases, and changes to systems. Baseline configurations include information about system components (e.g., standard software packages installed on workstations, notebook computers, servers, network components, or mobile devices; current version numbers and update and patch information on operating systems and applications; and configuration settings and parameters), network topology, and the logical placement of those components within the system architecture. Baseline configurations of systems also reflect the current enterprise architecture. Maintaining effective baseline configurations requires creating new baselines as organizational systems change over time. Baseline configuration maintenance includes reviewing and updating the baseline configuration when changes are made based on security risks and deviations from the established baseline configuration.

Organizations can implement centralized system component inventories that include components from multiple organizational systems. In such situations, organizations ensure that the resulting inventories include system-specific information required for proper component accountability (e.g., system association, system owner). Information deemed necessary for effective accountability of system components includes hardware inventory specifications, software license information, software version numbers, component owners, and for networked components or devices, machine names and network addresses. Inventory specifications include manufacturer, device type, model, serial number, and physical location.

NIST SP 800-128 provides guidance on security-focused configuration management.

### FURTHER DISCUSSION

An effective cybersecurity program depends on consistent, secure system and component configuration and management. Build and configure systems from a known, secure, and approved configuration baseline. This includes:

* documenting the software and configuration settings of a system;
* placement within the network; and
* other specifications as required by the organization.

**Example**

You are in charge of upgrading the computer operating systems of your office’s computers. You research how to set up and configure a workstation with the least functionality and highest security and use that as the framework for creating a configuration that minimizes functionality while still allowing users to do their tasks. After testing the new baseline on a single workstation, you document this configuration and apply it to the other computers [a].You then check to make sure that the software changes are accurately reflected in your master system inventory [e]. Finally, you set a calendar reminder to review the baseline in three months [f].

**Potential Assessment Considerations**

* Do baseline configurations include software versions and patch level, configuration parameters, network information, and communications with connected systems [a,b]?
* Are baseline configurations updated as needed to accommodate security risks or software changes [c]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.4.1