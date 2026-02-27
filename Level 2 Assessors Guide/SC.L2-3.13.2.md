# SC.L2-3.13.2 – Security Engineering

## Security Requirement Employ architectural designs, software development techniques, and systems engineering principles that promote effective information security within organizational systems. |

## Assessment Objectives [a] architectural designs that promote effective information security are identified;  [b] software development techniques that promote effective information security are identified;  [c] systems engineering principles that promote effective information security are identified;  [d] identified architectural designs that promote effective information security are employed;  [e] identified software development techniques that promote effective information security are employed; and  [f] identified systems engineering principles that promote effective information security are employed. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SC.L2-3.13.2 – SECURITY ENGINEERING

### SECURITY REQUIREMENT

Employ architectural designs, software development techniques, and systems engineering principles that promote effective information security within organizational systems.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] architectural designs that promote effective information security are identified;
:   [b] software development techniques that promote effective information security are identified;
:   [c] systems engineering principles that promote effective information security are identified;
:   [d] identified architectural designs that promote effective information security are employed;
:   [e] identified software development techniques that promote effective information security are employed; and
:   [f] identified systems engineering principles that promote effective information security are employed.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Security planning policy; procedures addressing system security plan development and implementation; procedures addressing system security plan reviews and updates; enterprise architecture documentation; system security plan; records of system security plan reviews and updates; system and communications protection policy; procedures addressing security engineering principles used in the specification, design, development, implementation, and modification of the system; security architecture documentation; security requirements and specifications for the system; system design documentation; system configuration settings and associated documentation; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with responsibility for determining information system security requirements; personnel with information system design, development, implementation, and modification responsibilities; personnel with security planning and system security plan implementation responsibilities; personnel with information security responsibilities].

**Test**

[SELECT FROM: Organizational processes for system security plan development, review, update, and approval; mechanisms supporting the system security plan; processes for applying security engineering principles in system specification, design, development, implementation, and modification; automated mechanisms supporting the application of security engineering principles in information system specification, design, development, implementation, and modification].

### DISCUSSION

Organizations apply systems security engineering principles to new development systems or systems undergoing major upgrades. For legacy systems, organizations apply systems security engineering principles to system upgrades and modifications to the extent feasible, given the current state of hardware, software, and firmware components within those systems. The application of systems security engineering concepts and principles helps to develop trustworthy, secure, and resilient systems and system components and reduce the susceptibility of organizations to disruptions, hazards, and threats. Examples of these concepts and principles include developing layered protections; establishing security policies, architecture, and controls as the foundation for design; incorporating security requirements into the system development life cycle; delineating physical and logical security boundaries; ensuring that developers are trained on how to build secure software; and performing threat modeling to identify use cases, threat agents, attack vectors and patterns, design patterns, and compensating controls needed to mitigate risk. Organizations that apply security engineering concepts and principles can facilitate the development of trustworthy, secure systems, system components, and system services; reduce risk to acceptable levels; and make informed risk-management decisions.

NIST SP 800-160-1 provides guidance on systems security engineering.

### FURTHER DISCUSSION

Familiarity with security engineering principles and their successful application to your infrastructure will increase the security of your environment. NIST SP 800-160 System Security Engineering: Considerations for a Multidisciplinary Approach in the Engineering of Trustworthy Secure Systems can serve as a source of security engineering and design principles.

Decide which designs and principles to apply. Some will not be possible or appropriate for a given company or for specific systems or components.

Designs and principles should be applied to policies and security standards. Starting with the baseline configuration, they should be extended through all layers of the technology stack (e.g., hardware, software, firmware) and throughout all the components of the infrastructure. The application of these chosen designs and principles should drive you towards a secure architecture with the required security capabilities and intrinsic behaviors present throughout the lifecycle of your technology.

As legacy components age, it may become increasingly difficult for those components to meet security principles and requirements. This should factor into life-cycle decisions for those components (e.g., replacing legacy hardware, upgrading or re-writing software, upgrading run-time environments).

**Example**

You are responsible for developing strategies to protect data and harden your infrastructure. You are on a team responsible for performing a major upgrade to a legacy system. You refer to your documented security engineering principles [c]. Reviewing each, you decide which are appropriate and applicable [c]. You apply the chosen designs and principles when creating your design for the upgrade [f].

You document the security requirements for the software and hardware changes to ensure the principles are followed. You review the upgrade at critical points in the workflow to ensure the requirements are met. You assist in updating the policies covering the use of the upgraded system so user behavior stays aligned with the principles.

**Potential Assessment Considerations**

* Does the organization have a defined system architecture [a,d]?
* Are system security engineering principles applied in the specification, design, development and implementation of the systems [d,e,f]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.13.2