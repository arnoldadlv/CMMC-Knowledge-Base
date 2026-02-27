# MA.L2-3.7.6 – Maintenance Personnel

## Security Requirement Supervise the maintenance activities of maintenance personnel without required access authorization. |

## Assessment Objectives [a] maintenance personnel without required access authorization are supervised during maintenance activities. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## MA.L2-3.7.6 – MAINTENANCE PERSONNEL

### SECURITY REQUIREMENT

Supervise the maintenance activities of maintenance personnel without required access authorization.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] maintenance personnel without required access authorization are supervised during maintenance activities.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System maintenance policy; procedures addressing maintenance personnel; service provider contracts; service-level agreements; list of authorized personnel; maintenance records; access control records; system security plan; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with system maintenance responsibilities; personnel with information security responsibilities].

**Test**

[SELECT FROM: Organizational processes for authorizing and managing maintenance personnel; mechanisms supporting or implementing authorization of maintenance personnel].

### DISCUSSION

This requirement applies to individuals who are performing hardware or software maintenance on organizational systems, while PE.L1-3.10.1 addresses physical access for individuals whose maintenance duties place them within the physical protection perimeter of the systems (e.g., custodial staff, physical plant maintenance personnel). Individuals not previously identified as authorized maintenance personnel, such as information technology manufacturers, vendors, consultants, and systems integrators, may require privileged access to organizational systems, for example, when required to conduct maintenance activities with little or no notice. Organizations may choose to issue temporary credentials to these individuals based on organizational risk assessments. Temporary credentials may be for one-time use or for very limited time periods.

### FURTHER DISCUSSION

Individuals without proper permissions must be supervised while conducting maintenance on organizational machines. Consider creating temporary accounts with short-term expiration periods rather than regular user accounts. Additionally, limit the permissions and access these accounts have to the most restrictive settings possible.

**Example**

One of your software providers has to come on-site to update the software on your company’s computers. You give the individual a temporary logon and password that expires in 12 hours and is limited to accessing only the computers necessary to complete the work [a]. This gives the technician access long enough to perform the update. You monitor the individual’s physical and network activity while the maintenance is taking place [a] and revoke access when the job is done.

**Potential Assessment Considerations**

* Are there processes for escorting and supervising maintenance personnel without required access authorization (e.g., vendor support personnel, short-term maintenance contractors) during system maintenance [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.7.6