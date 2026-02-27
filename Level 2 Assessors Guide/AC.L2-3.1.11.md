# AC.L2-3.1.11 – Session Termination

## Security Requirement Terminate (automatically) a user session after a defined condition. |

## Assessment Objectives [a] conditions requiring a user session to terminate are defined; and  [b] a user session is automatically terminated after any of the defined conditions |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## AC.L2-3.1.11 – SESSION TERMINATION

### SECURITY REQUIREMENT

Terminate (automatically) a user session after a defined condition.

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] conditions requiring a user session to terminate are defined; and
:   [b] a user session is automatically terminated after any of the defined conditions occur.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: Access control policy; procedures addressing session termination; system design documentation; system security plan; system configuration settings and associated documentation; list of conditions or trigger events requiring session disconnect; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; system developers].

**Test**

[SELECT FROM: Mechanisms implementing user session termination].

### DISCUSSION

This requirement addresses the termination of user-initiated logical sessions in contrast to the termination of network connections that are associated with communications sessions (i.e., disconnecting from the network). A logical session (for local, network, and remote access) is initiated whenever a user (or process acting on behalf of a user) accesses an organizational system. Such user sessions can be terminated (and thus terminate user access) without terminating network sessions. Session termination terminates all processes associated with a user’s logical session except those processes that are specifically created by the user (i.e., session owner) to continue after the session is terminated. Conditions or trigger events requiring automatic session termination can include organization-defined periods of user inactivity, targeted responses to certain types of incidents, and time-of-day restrictions on system use.

### FURTHER DISCUSSION

Configure the system to terminate user sessions based on the organization’s policy. Session termination policies can be simple or sophisticated. Examples are inactivity (end the session after a specified duration (e.g., one hour7) of inactivity), day/time (all sessions are terminated at the end of the established workday), misbehavior (end the session due to an attempted policy violation), and maintenance (terminate sessions to prevent issues with an upgrade or service outage). If there is no automatic control of user sessions, an attacker can take advantage of an unattended session.

**Example 1**

You are the system administrator for your organization and configure the system to terminate all user sessions after 1 hour of inactivity [a]. As the session timeout approaches, the system prompts users with a warning banner asking if they want to continue the session. When the session timeout does occur, the login page pops up, and the users must log in to start a new session [b].

**Example 2**

A user is logged into a corporate database containing CUI but is not authorized to view CUI. The user has submitted a series of queries that unintentionally violate policy, as they attempt to extract CUI that the user is not authorized to view [a]. The session terminates with a warning as a result of a violation of corporate policy [b]. The user must reestablish the session before being able to submit additional legitimate queries.

**Potential Assessment Considerations**

* Are the conditions in which a user session must be terminated described (e.g., after a period of inactivity or after a defined time limit) [a]?
* Are procedures documented that describe how to configure the system to enable automatic termination of user sessions after any of the defined conditions occur [b]?
* Are user sessions terminated based on organizationally defined conditions [a,b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.1.11