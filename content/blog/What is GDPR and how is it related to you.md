+++
title = "What is GDPR and how is it related to you?"
description = "As the new technologies evolve and in the online-first world we migrate our lives to the web, legislation appears to protect the individual's privacy as they share sensitive personal data on the Internet. Obviously, that’s great, but it implies profound changes in the IT infrastructure of every organization dealing with personally identifiable information (PII). Let’s take this challenge and find out what pitfalls you may face trying to meet GDPR demands."
date = 2019-05-07

[taxonomies]
tags = ["gdpr"]
+++

### What is GDPR?

The General Data Protection Regulation (GDPR), to those of you
who don't know, is a European Union law that applies to companies
dealing with PII of EU residents.

![](https://o365hq.com/images/330.png)

The key takeaways from the picture above are that it has improved
privacy rights and more responsibility for data security. There are
mandatory breach requirements, so if you're in the US, that's already
pretty familiar to you because almost all states already have data
breach reporting requirements. There are also significant penalties for
noncompliance -- it can be up to 4 percent of your annual revenue for
the worst-case scenario.

### What does that mean to your organization?

![](https://o365hq.com/images/332.png)

The GDPR have enforceable data subject rights, meaning
customers can ask for a copy of their data or demand to be forgotten (a
right to ask that your data be deleted), or exercise the right for data
portability (i.e., the data should be in an exportable, machine-readable
format, something like a .pst file for Outlook or similar).

In terms of controls and notifications, there's a requirement for
appropriate security measures, but it doesn't specify any particular
technologies, as these change very quickly. There are breach
notifications requirements, requirements to get consent, and to keep
detailed records for processing. To prove the transparency of your
policies, you should describe processing purposes and define what you're
going to do with the information. There's also such a thing as a Data
Protection Impact Assessment -- a DPIA (which is basically a
risk assessment) that you might be required to do for high-risk
processing if you're doing things like managing health records or
surveillance data from surveillance cameras.

And then, of course, IT and training -- there are all kinds of training
that would be required to re-engineer your institutions, including in
some cases employing a data protection officer, and GDPR has
some guidelines for when to do that.

You may wonder, what if GDPR doesn't apply to me; why should I
bother? Well, the GDPR may not be affecting you now, but you
really should pay attention to it and start thinking about how you might
want to make changes in the future, because we're seeing not just
Europe, but countries like Japan, Canada, Argentina, and others looking
at GDPR-like legislation and planning to enact something
similar. Additionally, companies such as Microsoft are implementing data
subject rights standards across the entire globe, because they really
like the idea of having one broad standard that is easier to comply
with than with a whole bunch of different standards. Alternatively,
consumers have become more discerning about consent and data collection
thanks to high-profile stories.

### What can your organization do to become GDPR-compliant?

It's a complicated process because there are 99 articles to the
GDPR. Some of them are technical, some of them are not; many of
them are sort of policy related. If you are fully on-prem, all the
responsibility will be your own. If you are to any extent in the cloud,
you are eligible for a shared responsibility model, where some of the
requirements are taken by Microsoft as a cloud service provider, and some
of them should be taken by the customers. Your GDPR journey may
comprise the following steps:

**1. Assess and manage risk**

Performing risk assessment with your data in the cloud is a lot easier
thanks to the Compliance Manager, which is a one-stop shop for managing
your entire compliance posture. With this tool, Microsoft shares
everything about how and what it does to secure your data and also
informs about your responsibility and gives you guidance on how to
implement your own controls to protect the data. Compliance Manager is a
powerful way to track and manage your privacy and compliance based on a
risk assessment score. (If you missed the article about this tool, you
can find it
[here](https://o365hq.com/blog/facilitate-your-compliance-work-with-a-new-tool-from-microsoft)
).

**2. Discover personal data**

After you assess your compliance risk, the next step is to think about
how you discover personally identifiable information within the
Microsoft cloud and beyond it. As you think about your data landscape
today, everyone is facing exponential growth in electronic data across
the organization. The complexity of that data and where that data is
stored is growing as well -- you've got data that is on devices, in
apps, in services, on premises, in the cloud, and it's flowing around all
those different environments. In addition, the types of data that you're
storing no longer are relegated to documents and email -- you have
voice mails, text messages, posts, mp3 files, etc. You have to ensure
that it is maintained in a compliant and secure manner across your whole
environment.

You can start off with basic understanding of the scope -- look at the data
and rationalize its use, the reasoning of the purpose it was collected
for, the intent that it's being used for, who is using it, et cetera, et
cetera, et cetera.

![](https://o365hq.com/images/331.png)

The scope estimation will help you to define what your data policy is
going to look like. Once you have a policy in place, then you can pretty
much easily convert that into some sort of an engineering toolset, and
then you can manage this much better across your organization.

With that in mind, obviously, every organization has a lot of unneeded
personal data or old data sitting there that you have not touched for a
while. Thanks to GDPR, you can rethink what's needed and what's
not and start cleaning it up. That reduces the surface area of your
liability for all your GDPR purposes. And a very good side
effect of such a cleanup is a huge cost savings, as storing and managing
data is very costly.

Once you have reduced the scope and the surface area, then you start
defining the policies under question. There is always a standard corporate
retention policy that you have across your organization that will be x
number of years, x number of months, whatever it is. With GDPR,
you should look at the data and the intent of its usage and then set
retention policies much more granularly depending on the type of data
that you have.\
Variance or exceptions also are key, so make sure that if there is a
certain dataset that you want to have an exception on, you have it very
well defined in the policy. If there is an audit, which is required for
legal purposes or managing a business, you will have an exception
process in place on how you manage and govern that data.

Then you can define what datasets you have to enable for all your
DRS rights, like the right to be forgotten or right to export
or view.\
Following these steps, you can create a framework to handle and manage
data.

**3. Protect and govern your data**

Microsoft offers you tools to protect data at the identity, document, and
network levels. Data protection through identity is about understanding
who has access to the data. At this level, you consider implementing
controls to ensure you have access governance properly implemented
throughout your organization and there are things like multi-factor
authentication or conditional access, privileged identity management and
hardware protection for credentials across your environment.

![](https://o365hq.com/images/329.png)

To protect information at the data level there is a solution called
Azure Information Protection (AIP), which allows you to attach
consistent labels to documents, and those labels are connected to
policies related to both protection and governance. Those policies can
be around encryption, watermarking, or retention of the document records
management or deletion.

Furthermore, labels are not just confined to Microsoft 365, as you can
take the same labels that you've put in the Microsoft Security and
Compliance Center, run the AIP scanner agent on your
on-premises file server, and classify those documents as well. The label
is persistent, and as those documents migrate from on-premises to online,
cloud systems will recognize that this document has a confidential label
with encryption policy, restricted access policy, retention policy, and
will enact each one of those policies on that document automatically.
You can even auto-classify documents using the auto-classification engine
within the Security and Compliance Center to look for data or patterns,
such as documents containing social security numbers, and if the engine
finds those documents, it will label them with SSN and apply
respective policies.

Protecting at the access level and at the document level is good, but we
cannot forget about threat protection. You should ensure that external
malicious actors aren't getting access to the data and if they do
somehow get access to your environment, that there's a system in place
that spans identity, device, and environment, and can take appropriate
actions when the machine, user, or document are regarded as infected. The
picture below shows the tools that have been put in place to ensure that
your data is protected across Microsoft 365.

![](https://o365hq.com/images/334.png)

### Respond efficiently

The last piece of the puzzle is related to efficient response, and part
of that response is how you manage the data subject requests (that might
be inundating your organization) in an efficient and timely manner,
ensuring that the data that was being shared with the person requesting
it is appropriate. There are solutions within Microsoft 365 to help you
manage your own data subject requests for the data that's located within
the Microsoft 365 environment, and a similar sort of software in Azure
and Dynamics that allow you to process requests for identities or
customer records (possibly stored in Dynamics). Within the Office 365
environment, you can search across Exchange Online, SharePoint Online,
OneDrive for Business (including Teams and Groups) and public folders.
There are over 80 supported sensitive data types, but a
GDPR-specific data type was published as well, and it looks for
specific EU personal data identifiers and looks across the 28 different
EU countries and puts that into one template that you can apply across
your data in these environments.

If you want to either forget the user or to export the data of the user,
you have to be an admin on that subscription to make such a request. You
can do this through the Service trust portal, clicking on Privacy plate and
scrolling down. You will see links for data log export, forget user's
data, or go to Security and Compliance center and find these options
right there.

![](https://o365hq.com/images/333.png)

Depending on the time and amount of data that you have about that user,
it will take probably somewhere between 1 to 30 days to get you the
data back.

The data that you may get could be huge in size, so you'd better set up
certain configurations to review the most essential pieces. For example,
if you pick the *Inclusive and the pivots* filter, you will see the near
duplicates of the file connected with the data subject, which will save
a ton of time.

![](https://o365hq.com/images/336.png)

In the *Annotate view* you can read the content and redact any piece of
it that you don't want to share with the data subject before you export
it out.

![](https://o365hq.com/images/335.png)

### Conclusion

The GDPR is really focused on the personal privacy rights of
individuals, and becoming compliant with it is a long journey where you
have to discover what sensitive data you have, where it resides, and how
to protect it. You need to have tools in place to govern that data to
ensure that it's not being shared inappropriately, that it's not being
deleted inadvertently, or that when you actually need to be able to find
it for a data subject request, you can do so in an efficient manner, in
a way that actually saves you time and money. Remember, you are not
alone in this -- IT Partner can provide guidance and help, and
make your IT infrastructure not only GDPR compliant, but make it
a better and safer place altogether.
