# AU.L2-3.3.6 – Reduction & Reporting

## Security Requirement Provide audit record reduction and report generation to support on-demand analysis and reporting. |

## Assessment Objectives [a] an audit record reduction capability that supports on-demand analysis is provided; and  [b] a report generation capability that supports on-demand reporting is provided. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AU.L2-3.3.6 – REDUCTION & REPORTING

### SECURITY REQUIREMENT

Provide audit record reduction and report generation to support on-demand analysis and reporting.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] an audit record reduction capability that supports on-demand analysis is provided; and [b] a report generation capability that supports on-demand reporting is provided.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Audit and accountability policy; procedures addressing audit record reduction and report generation; system design documentation; system security plan; system configuration settings and associated documentation; audit record reduction, review, analysis, and reporting tools; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with audit record reduction and report generation responsibilities; personnel with information security responsibilities].

**Test**

[SELECT FROM: Audit record reduction and report generation capability].

### DISCUSSION

Audit record reduction is a process that manipulates collected audit information and organizes such information in a summary format that is more meaningful to analysts. Audit record reduction and report generation capabilities do not always emanate from the same system or organizational entities conducting auditing activities. Audit record reduction capability can include, for example, modern data mining techniques with advanced data filters to identify anomalous behavior in audit records. The report generation capability provided by the system can help generate customizable reports. Time ordering of audit records can be a significant issue if the granularity of the time stamp in the record is insufficient.

### FURTHER DISCUSSION

Raw audit log data is difficult to review, analyze, and report because of the volume of data. Audit record reduction is an automated process that interprets raw audit log data and extracts meaningful and relevant information without altering the original logs. An example of log reduction for files to be analyzed would be the removal of details associated with nightly backups. Report generation on reduced log information allows you to create succinct customized reports without the need to burden the reader with unimportant information. In addition, the security-relevant audit information must be made available to personnel on demand for immediate review, analysis, reporting, and event investigation support. Performing audit log reduction and providing on-demand reports may allow the analyst to take mitigating action before an adversary completes its malicious actions.

**Example**

You are in charge of IT operations in your company. You are responsible for providing audit record reduction and report generation capability. To support this function, you deploy an open-source solution that will collect and analyze data for signs of anomalies. The solution queries your central log repository to extract relevant data and provide you with a concise and comprehensive view for further analysis to identify potentially malicious activity [a]. In addition to creating on-demand data sets for analysis, you create customized reports explaining the contents of the data set [b].

**Potential Assessment Considerations**

* Does the system support on-demand audit review, analysis, and reporting requirements and after-the-fact security investigations [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.3.6