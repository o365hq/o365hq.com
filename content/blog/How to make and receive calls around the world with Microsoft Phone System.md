+++
title = "How to make and receive calls around the world with Microsoft Phone System"
description = "Microsoft offers enterprise voice capabilities both for internal communication within the organization and for calling externally to any device or landline, irrespective of location."
date = 2019-08-28

[taxonomies]
tags = ["cloud phone system", "microsoft teams"]
+++

Employees' expectations about voice communications are changing. Voice remains a
critical and essential workload, as people
[report](https://news.virginia.edu/content/qa-how-much-workplace-collaboration-too-much)
that 80% of their time at work is spent collaborating (i.e., in
meetings, calls). But how do you capture important information in voice?
Typing at a PC or making analog recordings doesn't meet expectations
anymore. Microsoft is delivering voice with things like transcription
and translation. So, when you missed the meeting and are trying to figure out
if the boss talked about you, you can literally ask Office 365 if your
name was mentioned and it'll search through the meeting file, coming
back with the results you need. Instead of listening to the meeting
recording for 75 minutes, you can spend 5 minutes doing a little
search in Office 365. Isn't it awesome?

Now let's hop in and start by explaining how Phone System works.

### What is Phone System and what features does it provide?

For better understanding of Office 365 Phone System, let's take a look at
the elements of a traditional telephone system within an organization,
or Private Branch Exchange (PBX).

![](https://o365hq.com/images/493.png)

Traditional PBX deployment consists of three parts: 1) the
endpoints for employees to place and receive calls, 2) the PBX
connecting calls between internal users, as well as sending them to
external users, and 3) the PSTN (Public Switched Telephone
Network) with all the external users. Phone System in Office 365 has the
exact same building blocks. Every Teams client, whether it's Windows,
Mac, Web (currently Edge only), iOS, Android, or IP phones, can be an
endpoint and use PBX features in addition to other Teams
features that you know and love.

Phone System is completely cloud- and software-based, so you may start
replacing hardware in your infrastructure and getting rid of
PBX servers, saving money and moving everything in one single
place. This is especially relevant for customers who are multi-national
and have vendor by country for the PBXs. With Phone System,
these organizations can centralize the software, increase
availability, and develop a uniform approach to management.

### How you can connect Phone System to the PSTN

Going back to our anatomy of traditional phone deployment, we are
now looking at the trunk portion. Connections between your PBX
and PSTN are made through either a Calling plan or Direct Routing
(or a mix of both).

![](https://o365hq.com/images/491.png)

#### Calling Plans

It's Microsoft's white-glove approach to PSTN availability in
your tenant. In other words, PSTN connectivity is provided
directly by Microsoft, so you have a single contract for all the
features, including PSTN calling, and a single party to deal
with. Microsoft partners on the backend take care of the PSTN
trunks, but you never see that partner. The exceptions are Australia and
Japan, where third parties provide calling plans. But they are very
tightly integrated with Microsoft.

In terms of compliance, Calling Plans meet all the legal requirements in
the participating countries, the list of which is limited to countries
where Microsoft operates as a regulated utility. At this time these include
the United States, the United Kingdom, Spain, the Netherlands, Puerto Rico, Ireland,
Germany, France, Canada, and Belgium. Australia and Japan are
special cases, where you get Calling Plans, but third parties (Telstra in
Australia, and Softbank in Japan) are providing the Calling Plan
features. This list is constantly being updated, so [check it
here](https://docs.microsoft.com/en-us/microsoftteams/country-and-region-availability-for-audio-conferencing-and-calling-plans/country-and-region-availability-for-audio-conferencing-and-calling-plans)
.

This PSTN connection solution is completely cloud-based and
doesn't require any infrastructure on-premises. Phone numbers can be
requested from Microsoft or brought in from your current provider.

The licensing model offers different management options. You can give a
bunch of people in a building a license for a year, and then if you
change the operation, you can easily redeploy those licenses to other
folks. For users calling only domestically, you can go for the cheaper
domestic Calling Plan. For other users, calling internationally, you can
get international calling, mixing and matching these as required.

#### Direct Routing

Essentially, this option brings your trunks to the party. Office 365
will be connected to the customer infrastructure, letting you use your
existing PBX or your existing carrier contracts. Also, there's
no need to port any phone numbers, since you'll remain in the same pool
of phone numbers.

![](https://o365hq.com/images/492.png)

On the very right side of the picture above, the user is being connected
to the Phone System. It is, in its turn, connected over the Internet to
the session border controller (SBC) on-premises, certified by
Microsoft, which is the key component. The SBC might be
connected to an existing PBX or some third-party voice apps
(supported by the certified SBC partners). Over the voice
trunk, SBC is connected to the PSTN provider.

This is a simplified architecture. A vast majority of deployments won't
look like this. Every company is different, and you might want to engage
a partner to host the SBC so you can get into a zero-hardware
deployment in your company. You might also feel that nobody can do it
better and cheaper than you in-house. Whatever setup you choose, it's
just important that it's connected to a certified session border
controller (SBC).

Calling Plans and Direct Routing don't exclude one another; you can
mix these options to achieve what makes the most sense for you.

### Services and voicemail

Calls tab on the navigation rail in the Teams client opens up all the
calling functionality. The picture below highlights some of the features
of the Phone System. On the default page, you can find your own phone
number (very useful in case you ever wonder how people can call you) and
use a dial pad (or just type the digits from the keyboard). The upper
menu contains Contacts, History, and Voicemail. And finally, clicking
your picture will bring you to the call forward settings.

![](https://o365hq.com/images/497.png)

Here are some other features worth mentioning:

**Federated calling**\
Federated calling allows you to call people in other companies on their Teams client
from the contact history.

**Calls escalation**\
Calls escalation allows you to add more participants to your one-to-one call.

**Do-not-disturb breakthrough**\
Do-not-disturb reakthrough capabilities allow you to configure certain people to have
priority access so they can bypass Do not disturb status limitations.

**Delegation**\
Delegation, also known as boss/admin or call-on-behalf, allows your
teammates to receive or make calls on your behalf (when you're out for
vacation, for example, or for any other reason). You can set up one delegate for
multiple bosses, multiple delegates for one boss, or any combination of
these options. Delegation allows you to configure calls to simultaneously
ring the delegates, or ring them after delay.

**Transfer**\
Transfer allows you to do a blind transfer (without informing the person you
plan to transfer it to), or to do a consult transfer (checking in with a
person before transferring a call to them via chat or audio call).

**Voicemail**\
Voicemails are delivered to the Exchange mailbox of the user with a
transcript created for the voicemail. You can optionally enable
profanity masking for the transcript, or disable transcript altogether.
Exchange will be used for deposit, compliance, and archiving of
voicemails.\
Generally, the voicemails can be played from Outlook or Teams, but
please note that when you're using an Exchange server, the voicemails
won't be displayed in the Teams client, and users will have to go to
Outlook to see them (you should have at least Exchange server 2013 CU12
or higher).

**Call queues and Auto-Attendant**\
Call queues and auto-attendant enable companies to automatically route calls to specific
departments, teams, or people in the organization. You can configure the
time when the call queue should be available, as well as music on hold
and custom messaging.

**Service numbers**\
Service numbers are used for scenarios that require high concurrency of
simultaneous calls (potentially, hundreds of concurrent calls). Among
these scenarios in Phone System are Auto-attendant, Call queues, and
Audio Conferencing.

Service numbers are always hosted by Microsoft, and you can get a new
service number or port in your own number. These numbers can be toll or
toll-free (the latter option means that communications credits are used
to charge you for Audio Conferencing and Calling Plan minutes).

### Admin bonuses

#### Administration

The administration portal is mostly used to configure individual settings or
small groups of users. If you want to enable a large group of users or
automate tasks such as user provisioning, you are also offered the full
PowerShell access to script user enablement and configurations.

#### Reporting

A rich set of reports will help you understand if the service is used
and what the quality is. Usage statistics can be found in the usage
reports per workload. There are separate reports on PSTN
calling, showing how many users made how many calls in a certain time
period.

![](https://o365hq.com/images/494.png)

In terms of call quality, you're offered two tools:

*Call Quality Dashboard*, which provides an accumulated view on quality
data. You can slice and dice the data by your needs; for example, by
network segment, audio device, location, etc. Usually, you should use the 
Call Quality Dashboard in a proactive manner and run a number of reports
to find out if call quality is what it should be. The picture below
shows a Call Quality Dashboard example, where you can see the overall
call quality, a graph with call quality per month showing in different
colors, if a call was good or poor, and poor call percentage.

![](https://o365hq.com/images/495.png)

*Call Analytics* for individual calls is a more reactive tool, used when
you get complaints on a bad experience so you can investigate that
specific call and find out the reasons. There are also the Call Detail
records, which give you information on who called whom and how long
that call was.

![](https://o365hq.com/images/496.png)

### Summary

Remaining an important part of employee workload, voice has evolved to encompass the
needs of the contemporary user. Teams offers all the voice capabilities
and makes it easy to take full control of how you want to communicate.

Phone System covers PBX, connecting calls between users,
and PSTN features, which allows reaching external users on the
PSTN phone network. For the latter, you may use Calling Plans
(a completely cloud-based, first-hand offer from Microsoft, removing the
requirement of having any physical servers on-premises), Direct Routing
(which involves your existing infrastructure and certified session
border controller), or both.

Discover how you can enhance collaboration in your company with voice
capabilities from Teams.
