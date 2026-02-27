# PS.L2-3.9.2 – Personnel Actions

## Security Requirement Ensure that organizational systems containing CUI are protected during and after personnel actions such as terminations and transfers. |

## Assessment Objectives [a] a policy and/or process for terminating system access and any credentials coincident with personnel actions is established;  [b] system access and credentials are terminated consistent with personnel actions such as termination or transfer; and  [c] the system is protected during and after personnel transfer actions. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## PS.L2-3.9.2 – PERSONNEL ACTIONS

### SECURITY REQUIREMENT

Ensure that organizational systems containing CUI are protected during and after personnel actions such as terminations and transfers.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] a policy and/or process for terminating system access and any credentials coincident with personnel actions is established;
:   [b] system access and credentials are terminated consistent with personnel actions such as termination or transfer; and
:   [c] the system is protected during and after personnel transfer actions.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Personnel security policy; procedures addressing personnel transfer and termination; records of personnel transfer and termination actions; list of system accounts; records of terminated or revoked authenticators and credentials; records of exit interviews; other relevant documents or records].

**Interview**

[SELECT FROM: Personnel with personnel security responsibilities; personnel with account management responsibilities; system or network administrators; personnel with information security responsibilities].

**Test**

[SELECT FROM: Organizational processes for personnel transfer and termination; mechanisms supporting or implementing personnel transfer and termination notifications; mechanisms for disabling system access and revoking authenticators].

### DISCUSSION

Protecting CUI during and after personnel actions may include returning system-related property and conducting exit interviews. System-related property includes hardware authentication tokens, identification cards, system administration technical manuals, keys, and building passes. Exit interviews ensure that individuals who have been terminated understand the security constraints imposed by being former employees and that proper accountability is achieved for system-related property. Security topics of interest at exit interviews can include reminding terminated individuals of nondisclosure agreements and potential limitations on future employment. Exit interviews may not be possible for some terminated individuals, for example, in cases related to job abandonment, illnesses, and non-availability of supervisors. For termination actions, timely execution is essential for individuals terminated for cause. In certain situations, organizations consider disabling the system accounts of individuals that are being terminated prior to the individuals being notified.

This requirement applies to reassignments or transfers of individuals when the personnel action is permanent or of such extended durations as to require protection. Organizations define the CUI protections appropriate for the types of reassignments or transfers, whether permanent or extended. Protections that may be required for transfers or reassignments to other positions within organizations include returning old and issuing new keys, identification cards, and building passes; changing system access authorizations (i.e., privileges); closing system accounts and establishing new accounts; and providing for access to official records to which individuals had access at previous work locations and in previous system accounts.

### FURTHER DISCUSSION

Employee access to CUI is removed when they change jobs or leave the company. When employment or program access is terminated for any reason, the following actions may occur within the defined time frame:

* all company IT equipment (e.g., laptops, cell phones, storage devices) is returned;
* all identification, access cards, and keys are returned; and
* an exit interview is conducted to remind the employee of their obligations to not discuss CUI, even after employment.

Additionally, perform the following:

* remove access to all accounts granting access to CUI or modify access to CUI as appropriate for a new work role;
* disable or close employee accounts for departing employees; and
* limit access to physical spaces with CUI for departing employees or those who transition to a work role that does not require access to CUI.

This practice, PS.L2-3.9.2, leverages the identification of system users required by IA.L1-3.5.1 in order to ensure that all accesses are identified and removed.

**Example 1**

You are in charge of IT operations. Per organizational policies, when workers leave the company, you remove them from any physical CUI access lists. If you are not their supervisor, you contact their supervisor or human resources immediately and ask them to:

* turn in the former employees’ computers for proper handling;
* inform help desk or system administrators to have the former employees’ system access revoked;
* retrieve the former employees’ identification and access cards; and
* have the former employees attend an exit interview where you or human resources remind them of their obligations to not discuss CUI [b].

**Example 2**

An employee transfers from one working group in your company to another. Human resources team notifies IT of the transfer date, and the employee’s new manager follows procedure by submitting a ticket to the IT help desk to provide information on the access rights the employee will require in their new role. IT implements the rights for the new position and revokes the access for the prior position on the official date of the transfer [c].

**Potential Assessment Considerations**

* Is information system access disabled upon employee termination or transfer [c]?
* Are authenticators/ credentials associated with the employee revoked upon termination or transfer within a certain time frame [b,c]?
* Is all company information system-related property retrieved from the terminated or transferred employee within a certain timeframe [a,c]?
* Is access to company information and information systems formerly controlled by the terminated or transferred employee retained for a certain timeframe [a,c]?
* Is the information security office and data owner of the change in authorization notified within a certain timeframe [a]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.9.2