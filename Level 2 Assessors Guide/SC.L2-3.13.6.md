# SC.L2-3.13.6 – Network Communication by Exception

## Security Requirement Deny network communications traffic by default and allow network communications traffic by exception (i.e., deny all, permit by exception). |

## Assessment Objectives [a] network communications traffic is denied by default; and  [b] network communications traffic is allowed by exception. |

## Further Discussion & Examples

**Source of Reference: The official [CMMC Level 2 Assessment Guide](https://dodcio.defense.gov/cmmc/Resources-Documentation/) from the Department of Defense Chief Information Officer (DoD CIO).**

For inquiries and reporting errors on this wiki, please [contact us](mailto:support@cmmctoolkit.org). Thank you.

## SC.L2-3.13.6 – NETWORK COMMUNICATION BY EXCEPTION

### SECURITY REQUIREMENT

Deny network communications traffic by default and allow network communications traffic by exception (i.e., deny all, permit by exception).

### ASSESSMENT OBJECTIVES

Determine if:

:   [a] network communications traffic is denied by default; and
:   [b] network communications traffic is allowed by exception.

### POTENTIAL ASSESSMENT METHODS AND OBJECTS

**Examine**

[SELECT FROM: System and communications protection policy; procedures addressing boundary protection; system security plan; system design documentation; system configuration settings and associated documentation; system audit logs and records; other relevant documents or records].

**Interview**

[SELECT FROM: System or network administrators; personnel with information security responsibilities; system developer; personnel with boundary protection responsibilities].

**Test**

[SELECT FROM: Mechanisms implementing traffic management at managed interfaces].

### DISCUSSION

This requirement applies to inbound and outbound network communications traffic at the system boundary and at identified points within the system. A deny-all, permit-by-exception network communications traffic policy ensures that only those connections which are essential and approved are allowed.

### FURTHER DISCUSSION

Block all traffic entering and leaving the network, but permit specific traffic based on organizational policies, exceptions, or criteria. This process of permitting only authorized traffic to the network is called whitelisting and limits the number of unintentional connections to the network.

This practice, SC.L2-3.13.6, requires a deny-all permit by exception approach for all network communications. In doing so, it adds specifics for SC.L2-3.13.1, which only requires monitoring, control, and protection of communication channels.

**Example**

You are setting up a new environment to house CUI. To properly isolate the CUI network, you install a firewall between it and other networks and set the firewall rules to deny all traffic [a]. You review each service and application that runs in the new environment and determine that you only need to allow http and https traffic outbound [b]. You test the functionality of the required services and make some needed adjustments, then comment each firewall rule so there is documentation of why it is required. You review the firewall rules on a regular basis to make sure no unauthorized changes were made.

**Potential Assessment Considerations**

* Are network communications traffic on relevant system components (e.g., host and network firewalls, routers, gateways) denied by default (e.g., configured with an implicit deny rule that takes effect in the absence of any other matching traffic rules) [a]?
* Are network communications traffic on relevant system components (e.g., host and network firewalls, routers, gateways) allowed by exception (e.g., configured with explicit allow rules that takes effect only when network traffic matches one or more rules) [b]?

### KEY REFERENCES

* NIST SP 800-171 Rev 2 3.13.6