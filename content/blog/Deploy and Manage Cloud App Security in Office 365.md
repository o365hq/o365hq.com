+++
title = "Deploy and Manage Cloud App Security in Office 365"
description = "Before we jump into the cloud app security implementation or the management process, let's talk about the cloud app security; what it is, and why we need it. It’s a Microsoft cloud-based solution that gives you insights into suspicious user activities."
date = 2019-06-04

[taxonomies]
tags = ["cloud security", "microsoft 365", "office 365", "tenant security"]
+++

![](https://o365hq.com/images/357.png)

You can generate an email and configure some
remediations against security alerts based on the user's activities.
Cloud app security is a requirement if you have been looking at implementing
Office 365, a cloud-based application, to protect your data and get
insights into your security solutions. 
A firewall or IPS does not have the capability to
give you insights on what users are doing in the cloud and how they are
accessing or sharing the data with external parties.

![](https://o365hq.com/images/351.png)

Cloud App Security is a complete framework that gives you insights on
a user's activities. Firstly, you can get insights on the user's activities
by having the discovery of your network. You can do the discovery by
uploading your end user or firewall logs or the user activity logs to
your server. You can do this in a one-time upload to get a snapshot
report where you can see the sanctioned or unsanctioned applications
being used by the users.

Next, you have information protection based on the 
DLP policies in Office 365 or Azure information protection
policies to apply the production on your data in Office 365. That
includes the ability to encrypt the data in the cloud,
or you can actually block access based on the DLP policies.

Third is threat prevention, where you define the
behavior-based activities and the alerts against, for example, users that are
trying to download data from an unmanaged device, and what actions
should be taken to stop users from downloading the data. You can suspend
user accounts or you can ask users to sign back in to the application,
or go with the security procedures you have in your company.

Lastly is in-session control. This is a new-ish feature within the application
that was announced 6 to 8 months ago. In-session control is where you 
have the users go through particular activities if they are trying to do 
something within these applications. For example, if a user is trying to share 
their data through OneDrive for Business with external parties, you can go in 
with the inspection controls to have the company policies on top of that to restrict 
the user from sharing data with third parties.

![](https://o365hq.com/images/352.png)

Cloud app security architecture is the very first step in cloud app security. 
How it works is, you have a discovery component where you can 
have discovery of your network to see the sanctioned and unsanctioned applications. 
You can get this particular report by uploading your firewall logs and the one-time 
report, giving you this snapshot. Or you can have automatic log configurations 
that can upload the logs to cloud app security.

We highly recommend that you use automatic firewall logs uploaded to the
Office 365 cloud app security so you can have a continuous report
on your end users' activities, and insights within your on-premises
network as well.

Once you have the insights on, the next step is the sanctioned and
unsanctioned applications. In a recent survey, more
than 80% of employees admitted that they were using
unsanctioned applications within the infrastructure to do their
day-to-day jobs.\
This means you have 80% risky users within the company
that are using unsanctioned applications in doing their day-to-day job,
which can cause data breach concerns for you and other security personnel.

Within the cloud app security, the app connector uses APIs on the back end 
for your different third-party application integrations to give you insights 
from Salesforce. Or if you are using CRM or third-party
SaaS applications, you can have the APIs integrate with them
to get the insights of user activities within the third-party
applications as well.

Conditional Access is based on the Azure Active
Directory, where you can have the conditional access
policies in force on the end users for the cloud app security based on
their activities. You can have the users sign back in or you
can have user access blocked based on their activities.
Another control within the cloud app security is the Policy-Based
control, where you can have controls on the end users when they are
trying to access the applications from an unmanaged platform, where 
you can enforce the user policy-based action
controls on what the user can do from an unmanaged device versus the
managed device in the organization. This is all being driven through
the cloud app security policies.

![](https://o365hq.com/images/350.png)

In order for you to deploy the cloud app security, there are four basic
steps. 

1. You can have cloud app security as part of 
your E5 license, or you can sign up for a trial tenant.

2. Once we have a trial tenant set up, you can upload your network
firewall logs or you can have a manual logs uploader. (Again, we
highly recommend that you upload configured automatic uploads of the
logs.) This can be done directly through the firewalls or you can have a
server on-premises that can collect the logs from all of your devices
and then upload those logs to the Office 365 cloud app security. 

3. Once you have the logs uploaded, connect your
sanctioned applications and block access to the
unsanctioned applications. The Microsoft team of analysts has about 30,000-plus applications that
are ranked based on their regularity requirements and security
controls.

4. Configuration of policies. By default, when you enable cloud app security,
it gives you 10 built-in policies for your configuration,
which gives you suspicious behavior of users, user sign-in from
risky locations, and/or unexpected travel by the user.

![](https://o365hq.com/images/353.png)

Within the discovery phase of the cloud, cloud app security gives
you Shadow ID discovery. It gives a cloud application risk
assessment and alerts on risky cloud usage.

Shadow IT discovery is the usage of unapproved ID applications that
are being used by end users.

The cloud application risk assessment is based on ID
security controls and the regulatory requirements of the company. It does 
have some policies from the Microsoft team of analysts as
well that access each and every application against more than 60-plus
controls from Microsoft to ensure whether this application is risky or 
safe to use within the organization. You can customize
these particular controls based on your requirements on your security
posture and it will give you the ranking and rating of the application,
whether this application can be used within the organization or not. Or
if it's risky, whether you want to allow this application to be used in
your organization.\
With alerts on risky activities, you can configure the alerts in the 
Azure cloud app security. Alerts are generated on suspicious activities 
within five minutes of your users performing risky activities, like having 
unexpected travel to somewhere that is not possible, or downloading from 
Sharepoint or OneDrive from an IP from where the user never logged into 
Office 365 before.

![](https://o365hq.com/images/355.png)

Information protection is paramount. So once we have the discovery
and the insights on, if we have some malicious activities or
a user trying to download data or some other alert, you can apply automatic 
policies to protect the data or stop the user's
behaviors; you can use the office DLP policies or Azure
information protection policy. This is where you can restrict downloading the
data from an unprotected device or from a risky network (outside your company 
network). You can apply the Azure information protection to encrypt the data 
in the cloud, as well as the data that is being downloaded.

![](https://o365hq.com/images/356.png)

Regarding threat detection, once you have the policies in force and information 
protection policies applied, you can remediate against those threats. In
cloud app security, you can have automatic remediation against threats, and you 
can configure the policies and actions against them. And those actions can be 
applied based on your configurations; for example, if someone is trying to access 
data from a risky location, you can suspend that user.

![](https://o365hq.com/images/354.png)

In-Session control is fairly new, having been released eight months
ago. With in-session control you can define the user's behavior and
if the user is accessing a certain application.

When the user is performing some malicious activity within the application,
you can block access or revoke access to that application. This can be achieved 
by integration with Azure Active Directory.

Go to the Microsoft website and on the cloud app security portal, you can
sign up for the trial. This allows you to experiment with the cloud app
security and then you can modify it to your specific needs. Or you can have the
cloud app security available as part of the Office 365 E5 license or the
EMS licenses.
