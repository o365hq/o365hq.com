+++
title = "9 Easy and Smart Ways to Enhance your Security with Microsoft 365 Business"
description = "In the previous article, we  discussed the best practices that will enhance the cybersecurity of your Office 365 Business. This time, let’s discover what Microsoft 365 has to offer in terms of security. Let’s clarify a few things before we move on, as Office 365 and Microsoft 365 are often mixed up. Microsoft 365 is a bundle solution that comprises Office 365 Business Premium, Windows 10 Pro, and Enterprise Mobility + Security. Keep this in mind if you’d like to make sure your employees can collaborate effectively, stay mobile, and feel secure from cyber threats 24/7."
date = 2019-01-10

[taxonomies]
tags = ["cloud security", "microsoft 365"]
+++

A little spoiler - Microsoft 365 (M365) is supercool in terms of
security because you get everything you need in one package and you can
control all the great features from one portal. It enjoys all the best
from Office 365 but also includes features available only as add-ons for
Office package, plus, of course, Windows Defender and EMS.
Let's see what these features are.

### Office message encryption

In M365 Business, a functionality of message encryption is available. It
makes it possible to:

\*send encrypted emails to anyone inside or outside your organization,
to any email address, including Office 365, Microsoft accounts (like
Hotmail or Outlook.com), and Google ID, to name just a few;\

-   receive encrypted messages and open them from any app on any device;
-   be sure that recipients won't be able to forward the email to
    others, as encrypted emails are sent with a "Do Not Forward"
    setting.

Encryption can easily make your corporate communication a lot safer. 

![](https://o365hq.com/images/198.png)

### Anti-phishing protection (ATP)

Social engineering brought phishing scams to a new level, where they
look almost genuine. But where humans can be tricked, artificial
intelligence (AI) will trace suspicious details. M365 Business includes
Office 365 Advanced Threat Protection (ATP), where specialized
code unmasks phishing attacks trying to penetrate the organization via
corporate email. Often, such attacks are impersonation-based. You can
easily set it right by choosing among various policy options to better
identify and prevent phishing and spoofing attempts.

Check [how to set up anti-phishing policy
here.](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-anti-phishing-policies)

![](https://o365hq.com/images/199.png)

###  ATP safe attachments and safe links

The ATP safe attachments tool opens every attached file in a
virtual environment before releasing it to the user. The possible
outcomes are:

-   safe attachment will be open right away after scanning;
-   attachments containing malicious content will be removed and a
    warning message will be displayed.

![](https://o365hq.com/images/200.png)

What if an email containing malicious content manages to squeeze into
a user's inbox folder? The ATP safe links policy can still save you
-- when the user clicks on a link, ATP verifies the web address included in the email or Office document. If for some
reason the link does not pass verification, one of the warning alerts
will pop up:

![](https://o365hq.com/images/201.png)

Read more on how to set up [safe
attachments](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-atp-safe-attachments-policies)
and [safe
links](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-atp-safe-links-policies)
policies.

### Exchange Online Archiving

Organizations often need to keep their business correspondence for
litigation, compliance, or other purposes. Online Archiving can complete
the task of backing up your emails the most convenient way. When Online
Archiving is enabled:

-   an archive mailbox is created within the user's primary mailbox;
-   users may use both their archives and primary mailboxes;
-   deleted items or even a deleted mailbox can be recovered;
-   retention tags may be applied both by users (personal tags) and by
    admins (retention policy tags). A retention tag specifies how long the
    message is kept and the action taken when retention time expires;
    retention policy is a method of applying a group of retention tags
    to the mailbox. It defines the time emails, folder(s), or the whole
    mailbox will be retained and whether it will be then deleted or
    preserved to comply with litigation or government requirements;
-   if a retention tag is not applied, the default retention tag will be
    applied to the file.

Check out [this link to enable archive
mailboxes.](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes)

![](https://o365hq.com/images/202.png)

### Azure Information protection

Given the exponential amount of data generated in our environments
today, it is obvious that an instrument able to find sensitive
information in those gigabytes of data and protect it is needed. This
instrument is Azure Information Protection. It offers capabilities for
detecting, classifying, and labelling files. Once applied, the label makes
them confidential, general, or some other level of protection you choose. AIP can
classify and label your data:

-   at rest
-   in use
-   in motion

And wherever it may reside:

-   Microsoft's Cloud
-   SaaS apps
-   non-Microsoft Clouds
-   your own data center in on-premises file servers
-   other platforms, such as Apple/Mac
-   non-Microsoft file types (e.g., PDFs in Adobe Reader)

This is pretty cool! It means that your data is protected no matter
which service it actually ends up in, because all these services
recognize the labels; thus protections, implied by labels, are always
going to be respected.

![](https://o365hq.com/images/203.png)

### Intune

Microsoft developed Intune, a tool that helps an organization reach
outside of its perimeter, managing and controlling both Microsoft and
non-Microsoft devices. It's compatible with the most common devices and
apps in the marketplace, so the employees' mobility grows
considerably. The best thing about Intune is that with such a great
number of various devices supervised, it still guarantees corporate data
security.

To learn more about Intune and how to get started using it, please [see
here.](https://docs.microsoft.com/en-us/intune/)

![](https://o365hq.com/images/204.png)

### Data loss prevention

Data loss prevention (DLP) is a specific policy that may
assist you in detecting personal sensitive data stored in various
locations, like SharePoint or OneDrive, etc., and prevent your users from
inadvertently sharing it. They are offered policy tips that help them to
comply with your DLP policies and still won't interfere with
their work. Here is where you can find the [overview of DLP
policies](https://docs.microsoft.com/en-us/office365/securitycompliance/data-loss-prevention-policies).

![](https://o365hq.com/images/205.png)

### Windows Defender

Windows Defender in M365 is protecting end points running Windows in
your organization. Similar to O365 and Azure AD, Windows Defender has
its own Advanced Threat Protection, and these three ATPs
actually collaborate. Windows ATP uses a sensor that monitors
activity on the operating system on the end point, trying to identify
anomalous activity that might be indicative of a potential threat
having taken hold of that machine.

Windows Defender Exploit Guard has many useful attributes.

-   Exploit protection detects the possible intrusion and use mitigation
    techniques to protect you from advanced threats, like zero-day
    exploits
-   Reduced attack surface configuring rules help to find apps and
    files that act like malware, infecting machines
-   Network protection capabilities block traffic to low
    reputation destinations by applying reputation analyses. This
    prevents users from accessing phishing and exploit sites and
    downloading malicious files
-   Controlled folder access protects files from malicious software
    (like ransomware). It assesses all apps, and doesn't let malicious or
    suspicious ones make changes to files in protected folders.

![](https://o365hq.com/images/206.png)

### Microsoft 365 Secure Score

Office 365 Secure Score was already mentioned in [a previous
article](o365hq.com/blog/top-8-solutions-to-secure-your-office-365-business)
, but with M365 it is also more advanced, as it analyses how well both
Office 365 and Windows are secured and gives recommendations, suggesting
specific controls you can apply to improve your security positioning.
It's easy to use and helps to understand where you are in terms of
security.

![](https://o365hq.com/images/207.png)

Summarizing the above, let's note that M365 offers many more advanced
security features that will turn threat protection into an exciting
journey of customizing its instruments to meet all your needs and
requirements, helping your business flourish and you sleep with a
peaceful mind. But if all this customization becomes confusing, don't
hesitate to reach out, and we'll be glad to assist you.
