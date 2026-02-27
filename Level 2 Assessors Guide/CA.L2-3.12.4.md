# CA.L2-3.12.4 – System Security Plan

## Security Requirement Develop, document, and periodically update system security plans that describe system boundaries, system environments of operation, how security requirements are implemented, and the relationships with or connections to other systems. |

## Assessment Objectives [a] a system security plan is developed;  [b] the system boundary is described and documented in the system security plan;  [c] the system environment of operation is described and documented in the system security plan;  [d] the security requirements identified and approved by the designated authority as non-applicable are identified;  [e] the method of security requirement implementation is described and documented in the system security plan;  [f] the relationship with or connection to other systems is described and documented in the system security plan;  [g] the frequency to update the system security plan is defined; and  [h] system security plan is updated with the defined frequency. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## CA.L2-3.12.4 – SYSTEM SECURITY PLAN

### SECURITY REQUIREMENT

Develop, document, and periodically update system security plans that describe system boundaries, system environments of operation, how security requirements are implemented, and the relationships with or connections to other systems.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] a system security plan is developed;
:   [b] the system boundary is described and documented in the system security plan;
:   [c] the system environment of operation is described and documented in the system security plan;
:   [d] the security requirements identified and approved by the designated authority as non-applicable are identified;
:   [e] the method of security requirement implementation is described and documented in the system security plan;
:   [f] the relationship with or connection to other systems is described and documented in the system security plan;
:   [g] the frequency to update the system security plan is defined; and
:   [h] system security plan is updated with the defined frequency.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Security planning policy; procedures addressing system security plan development and implementation; procedures addressing system security plan reviews and updates; enterprise architecture documentation; system security plan; records of system security plan reviews and updates; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with security planning and system security plan implementation responsibilities; personnel with information security responsibilities].

**Test**

[SELECT FROM: Organizational processes for system security plan development, review, update, and approval; mechanisms supporting the system security plan].

### DISCUSSION

System security plans relate security requirements to a set of security controls. System security plans also describe, at a high level, how the security controls meet those security requirements, but do not provide detailed, technical descriptions of the design or implementation of the controls. System security plans contain sufficient information to enable a design and implementation that is unambiguously compliant with the intent of the plans and subsequent determinations of risk if the plan is implemented as intended. Security plans need not be single documents; the plans can be a collection of various documents including documents that already exist. Effective security plans make extensive use of references to policies, procedures, and additional documents (e.g., design and implementation specifications) where more detailed information can be obtained. This reduces the documentation requirements associated with security programs and maintains security-related information in other established management/operational areas related to enterprise architecture, system development life cycle, systems engineering, and acquisition. Federal agencies may consider the submitted system security plans and plans of action as critical inputs to an overall risk management decision to process, store, or transmit CUI on a system hosted by a nonfederal organization and whether it is advisable to pursue an agreement or contract with the nonfederal organization.

NIST SP 800-18 provides guidance on developing security plans.

### FURTHER DISCUSSION

A system security plan (SSP) is a document that outlines how an organization implements its security requirements. At a minimum, an SSP must include:

* Description of the CMMC Assessment Scope;
* CMMC Assessment Scope Description: high-level description of the assets within the assessment scope;
* Description of the Environment of Operation: physical surroundings in which an information system processes, stores, and transmits information;
* Identified and Approved Security Requirements: requirements levied on an information system that are derived from applicable laws, Executive Orders, directives, policies, standards, instructions, regulations, procedures, or organizational mission/business case needs to ensure the confidentiality, integrity, and availability of the information being processed, stored, or transmitted;
* Implementation Method for Security Requirements: description of how the identified and approved security requirements are implemented with the system or environment;
* Connections and Relationships to Other Systems and Networks: description of related, dependent, and interconnected systems; and
* Defined Frequency of Updates: typically at least annually.

In addition to the requirements above, an SSP often includes:

* general information system description: technical and functional description;
* design philosophies: defense-in-depth strategies and allowed interfaces and network protocols; and
* roles and responsibilities: description of the roles and responsibilities for key personnel, which may include the system owner, system custodian, authorizing officials, and other stakeholders

This practice, CA.L2-3.12.4, which requires developing, documenting, and updating system security plans, promotes effective information security within organizational systems required by SC.L2-3.13.2, as well as other system and communications protection practices.

**Example**

You are in charge of system security. You develop an SSP and have senior leadership formally approve the document [a]. The SSP explains how your organization handles CUI and defines how that data is stored, transmitted, and protected [d,e]. The criteria outlined in the SSP is used to guide configuration of the network and other information resources to meet your company’s goals. Knowing that it is important to keep the SSP current, you establish a policy that requires a formal review and update of the SSP each year [g,h].

**Potential Assessment Considerations**

* Do mechanisms exist to develop and periodically update an SSP [a,g]?
* Are security requirements identified and approved by the designated authority as non-applicable documented [d]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.12.4