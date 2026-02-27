# MA.L2-3.7.4 – Media Inspection

## Security Requirement Check media containing diagnostic and test programs for malicious code before the media are used in organizational systems. |

## Assessment Objectives [a] media containing diagnostic and test programs are checked for malicious code before being used in organizational systems that process, store, or transmit CUI. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## MA.L2-3.7.4 – MEDIA INSPECTION

### SECURITY REQUIREMENT

Check media containing diagnostic and test programs for malicious code before the media are used in organizational systems.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] media containing diagnostic and test programs are checked for malicious code before being used in organizational systems that process, store, or transmit CUI.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System maintenance policy; procedures addressing system maintenance tools; system maintenance tools and associated documentation; maintenance records; system security plan; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with system maintenance responsibilities; personnel with information security responsibilities].

**Test**

[SELECT FROM: Organizational process for inspecting media for malicious code; mechanisms supporting or implementing inspection of media used for maintenance].

### DISCUSSION

If, upon inspection of media containing maintenance diagnostic and test programs, organizations determine that the media contain malicious code, the incident is handled consistent with incident handling policies and procedures.

### FURTHER DISCUSSION

As part of troubleshooting, a vendor may provide a diagnostic application to install on a system. As this is executable code, there is a chance that the file is corrupt or infected with malicious code. Implement procedures to scan any files prior to installation. The same level of scrutiny must be made as with any file a staff member may download.

This practice, MA.L2-3.7.4, extends both SI.L1-3.14.2 and SI.L1-3.14.4. SI.L1-3.14.2 and SI.L1- 3.14.4 require the implementation and updating of mechanisms to protect systems from malicious code, and MA.L2-3.7.4 extends this requirement to diagnostic and testing tools.

**Example**

You have recently been experiencing performance issues on one of your servers. After troubleshooting for much of the morning, the vendor has asked to install a utility that will collect more data from the server. The file is stored on the vendor’s FTP server. The support technician gives you the FTP site so you can anonymously download the utility file. You also ask him for a hash of the utility file. As you download the file to your local computer, you realize it is compressed. You unzip the file and perform a manual antivirus scan, which reports no issues [a]. To verify the utility file has not been altered, you run an application to see that the hash from the vendor matches.

**Potential Assessment Considerations**

* Are media containing diagnostic and test programs (e.g., downloaded or copied utilities or tools from manufacturer, third-party, or in-house support teams) checked for malicious code (e.g., using antivirus or antimalware scans) before the media are used on organizational systems [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.7.4