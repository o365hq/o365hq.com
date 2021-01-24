+++
title = "Microsoft Defender Advanced Threat Protection"
description = "Microsoft Defender ATP is a security that keeps endpoints safe from cyber threats, identifies sophisticated attacks, and automates security incidents. It is built into Windows 10, not bolted on, so there is nothing to deploy. "
date = 2020-06-03

[taxonomies]
tags = ["cloud security", "microsoft 365", "tenant security"]
+++


All it requires is to run a small onboarding script on each of the
endpoint machines to onboard them to the service. The script sets the
registry on the machines to report activities to the MDATP
service. There's no agent to install/run on the machines.

![](https://o365hq.com/images/748.png)

Besides Windows, MDATP can onboard and monitor non-Windows
endpoints, including Linux, Mac OS, iOS, and Android. The SecOps team can
also choose the deployment method that's convenient for the
organization, such as System Center Config Manager, MDM/Intune,
or Group Policy.

The MDATP Dashboard is an operational view of the
organization's endpoints and users that gives the SecOps user an
aggregated view of the latest alerts, their severity, and when they were
observed. It also provides a listing of the machines most at risk, with
several alerts related to each machine and indicates users at risk,
providing insight into the activities, actions, and relationships to the
machine. The security operations dashboard in MDATP provides a
single pane and centralized management.

![](https://o365hq.com/images/749.png)

Alerts are any security-related incidents collected from the
organization's endpoints and flagged by the MDATP service. The
SecOps user can see the latest alerts from all machines that are
onboarded in the entire company, along with the severity of each alert.
Severity in this context is the potential impact the associated malware
may have on an organization as a whole -- not just to a single endpoint
or a single user.

Microsoft Defender Security Center allows the SecOps user to set alert
status, set classification types, or create a rule to suppress the alert
next time it occurs in a specific machine or anywhere in the
organization. The alert story displays the alert and related evidence
together with other events that occurred within the same execution
context and time.

![](https://o365hq.com/images/752.png)

Attackers need not inject a physical file in a victim's machine to take
control -- attacks can happen through scripts. Detection of such scripts
is difficult because administrators also often run scripts remotely to
carry out various administrative activities. By default, Microsoft
Defender ATP will wait for SecOp's approval before
proceeding, but they could also configure it under the machine group
settings to skip this step and apply remediation automatically.

The machine view page provides SecOps with an overview of
security-relevant details, such as logged-on users, high-level machine
status, and risk profile.

Here they can also see that the Microsoft Defender Security Center
supports multiple endpoint types, including Windows Server 2019, Linux
Machines, as well as Apple clients running MacOS.

![](https://o365hq.com/images/750.png)

Additionally, they can view a rich and detailed timeline that shows all
events observed from this machine, as far back as six months.
Additionally, they can interactively hunt, search, and explore historical
data across all the endpoints. SecOps can reduce the verbosity by using
search or filter functionality.

Drilling in, the detailed view of the alert shows the SecOps team what
services were involved in the alert, as well as what files are
affected.\
Here, SecOps can see that the malware in question was introduced via an
email, and with the deep integration with Office ATP, we can
also get more details on who else in the organization received this
mail, including *Delivery Actions* (Delivered, Delivered to Junk, or
Blocked), as well as the *Delivery Location* (Inbox, Junk, or
Quarantine).

![](https://o365hq.com/images/751.png)

Enterprises often deal with cyber threats. The threat analytics
dashboard offers several overviews about the threats described in the
reports. It also contains worldwide impact and detection information, plus
mitigation recommendations.\
Diving into security recommendations, the SecOps user can see that
MDATP is providing a list of actionable recommendations to
improve the vulnerability posture of the organization, both in relation
to software vulnerabilities and endpoint misconfigurations.\
This page contains a dynamic prioritized list of security
recommendations for the entire organization across all operating systems
and software.

![](https://o365hq.com/images/753.png)

These recommendations are prioritized based on the potential exposure
improvement impact that applying them would generate, to help security
admins focus on the vulnerabilities that are currently posing the
highest exposure risk.

There are two types of mitigating actions.

1.  Creating a remediation request -- this is the primary mitigation
    option for a security recommendation.
2.  Creating an exception -- in some cases, it is not possible to apply
    the primary remediation, and security admins can choose to create an
    exception instead.

![](https://o365hq.com/images/754.png)

The area of Threat & Vulnerability Management (TVM) allows the
viewing, monitoring, and controlling of the progress/status of remediation requests
and exceptions that were created in the company.

The remediation progress is a real-time reflection of the endpoint patch
state that is continuously assessed by the MDATP sensor. The
SecOps user can view activities that are currently active/in progress,
as well as expired and completed activities. The Software Inventory area
of Threat & Vulnerability Management (TVM) provides visibility
into all the first- and third-party software installed across all devices in
the company.

Also, the SecOps user can drill down into any of the software products
listed in the software inventory for a full, detailed overview of this
software and its related TVM data -- security recommendations,
related vulnerabilities, version distribution, missing security updates
(KBs), and more.

This page provides all available data related to the vulnerabilities
that software is introducing into the company, their exposure impact, and
related security recommendations.

The machine page in MDATP has been enriched with TVM
data, providing full vulnerability context for the machine entity --
security recommendations, software vulnerabilities, software inventory,
and overall exposure level.

![](https://o365hq.com/images/755.png)

This enrichment serves the SecOps, who can now
easily see any gaps in a machine's defenses while investigating an alert
and gaining insights into possible weaknesses that were exploited by an
attacker.

The *Weaknesses* page is essentially a knowledge base listing all the
vulnerabilities (CVEs) that are known to TVM -- both
CVEs that apply to your organization at this time, and
those that aren't. The SecOps team is interested in understanding how
exposed the organization is to a specific CVE -- so this is the
place to review it.

For each vulnerability, the SecOps user can view the severity using the
*Common Vulnerability Scoring System (CVSS)* rating. This
includes the *Vulnerability description* for the CVE, as well
as its prevalence within the organization, any related software, or a
corresponding breach. The SecOps user can also review the vulnerability
details, which include detailed information on severity, age, and any
known related software. The SecOps team has access to detailed *Threat
insights*, which includes information relating to the threat landscape
for this vulnerability, such as public exploits and exploit kits.

Also, with endpoint management, you have detailed data as an
exportable list on any *Exposed machines* exposed to this vulnerability
from within the organization.

![](https://o365hq.com/images/756.png)

The SecOps team can take advantage of the advanced hunting capabilities
on MDATP with TVM. Here they have a saved query for
identifying machines that have an active High Alert status for software
threat vulnerabilities. They are then able to run this query to see what
machines in the environment need remediation.

The Alert window allows SecOps to see how this vulnerability in software
has allowed for some malicious activity. Under Actions, there is an
option to consult a *Microsoft Threat Expert*. If they choose to submit
a request, a Microsoft expert would review the alert and give detailed
recommended actions.

All Threat & Vulnerability Management (TVM) pages can be viewed
in the context of specific machine groups -- this helps to understand
your vulnerabilities and exposure for different parts of the company.
The machine group filter remains persistent when moving across and drilling
downing through different TVM pages.

The live response is created to improve analysis by authorizing the
SecOps user to gather forensic data fast, send suspicious entities for a
thorough check, and hunt for new threats. It provides instant access to a
machine and allows in-depth investigative work and taking immediate
response actions to promptly contain identified threats -- in real time.

![](https://o365hq.com/images/758.png)

Usually, enterprise SecOps teams rely on dependable reporting
visualizations to make crucial security decisions.\
Power BI is a business analytics service that delivers insights to
enable fast, informed decisions. Here in the PowerBI home page, there is
a dashboard pinned that contains some of our MDATP reporting
data. Inside this Workspace, the SecOps user can see a pinned Dashboard
where the data is easily accessible.

The MDATP dashboard helps SecOps check reports being shown. The
PowerBI Report is leveraging the MDATP Advanced Hunting
API; they can take a closer look at the report by clicking the
*Events Report*. The report can be shared, exported, and even subscribed
to as a feed, so the SecOps team can get this report directly into their
inbox as part of their daily routine.

![](https://o365hq.com/images/757.png)

The Machine actions allows the SecOps user to see what actions, both
manually initiated and automatically initiated, have been
performed within the environment. It has a breakdown of these actions
per machine so they can see which machines are most active.

Microsoft Defender Advanced Threat Protection is a platform designed to
help enterprise networks prevent, identify, explore, and respond to
advanced threats.

![](https://o365hq.com/images/759.png)
