# AU.L2-3.3.5 – Audit Correlation

## Security Requirement Correlate audit record review, analysis, and reporting processes for investigation and response to indications of unlawful, unauthorized, suspicious, or unusual activity. |

## Assessment Objectives [a] audit record review, analysis, and reporting processes for investigation and response to indications of unlawful, unauthorized, suspicious, or unusual activity are defined; and  [b] defined audit record review, analysis, and reporting processes are correlated. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AU.L2-3.3.5 – AUDIT CORRELATION

### SECURITY REQUIREMENT

Correlate audit record review, analysis, and reporting processes for investigation and response to indications of unlawful, unauthorized, suspicious, or unusual activity.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] audit record review, analysis, and reporting processes for investigation and response to indications of unlawful, unauthorized, suspicious, or unusual activity are defined; and
:   [b] defined audit record review, analysis, and reporting processes are correlated.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Audit and accountability policy; procedures addressing audit record review, analysis, and reporting; system security plan; system design documentation; system configuration settings and associated documentation; procedures addressing investigation of and response to suspicious activities; system audit logs and records across different repositories; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with audit record review, analysis, and reporting responsibilities; personnel with information security responsibilities].

**Test**

[SELECT FROM: Mechanisms supporting analysis and correlation of audit records; mechanisms integrating audit review, analysis and reporting].

### DISCUSSION

Correlating audit record review, analysis, and reporting processes helps to ensure that they do not operate independently, but rather collectively. Regarding the assessment of a given organizational system, the requirement is agnostic as to whether this correlation is applied at the system level or at the organization level across all systems.

### FURTHER DISCUSSION

Companies must review, analyze, and report audit records to help detect and respond to security incidents in a timely manner for the purpose of investigation and corrective actions. Collection of audit logs into one or more central repositories may facilitate correlated review. Small companies may be able to accomplish this manually with well-defined and -managed procedures. Larger companies will use an automated system for analysis that correlates log data from across the entire enterprise. Some companies may want to orchestrate the analysis process to include the use of Application Programming Interfaces (APIs) for collection, correlation, and the automation of responses based on programed rulesets.

**Example**

You are a member of a cyber defense team responsible for audit log analysis. You run an automated tool that analyzes all the audit logs across a Local Area Network (LAN) segment simultaneously looking for similar anomalies on separate systems at separate locations. After extracting anomalous information and performing a correlation analysis [b], you determine that four different systems have had their event log information cleared between 2:00 AM to 3:00 AM, although the associated dates are different. The team monitors all systems on the same LAN segment between 2:00 AM to 3:00 AM for the next 30 days.

**Potential Assessment Considerations**

* Are mechanisms used across different repositories to integrate audit review, analysis, correlation, and reporting processes [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.3.5