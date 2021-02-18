+++
title = "Skype for Business to Teams migration from the admin’s perspective"
description = "Moving from Skype for Business (SfB) to Tеams is a challenge for users, as they are expected to master a totally new collaboration tool. But what about admins and their experience? Let’s find out."
date = 2019-07-29

[taxonomies]
tags = ["microsoft teams", "migration"]
+++

### How to upgrade from SfB Online and what is migrate?

For admin, the upgrade means just turning the switch on the back end by
assigning TeamsUpgradePolicy with a *"TeamsOnly"* mode in PowerShell.
Another way is to visit the modern Tеams admin center, where a nice little
*"Tеams upgrade"* button helps to control coexistence and complete the
migration. Just keep in mind that it may take up to four hours to apply
the policy changes, so be patient and plan it beforehand.

![](https://o365hq.com/images/480.png)

One little notice, for a flawless experience, users should already have an
account in SfB Online.

When this policy is in place, the auto-start of SfB while logging into
Windows will be disabled. If people are stubborn and still go to SfB,
they'll be notified that their organization is now using Teams, and
nicely asked to log in to their new account.

All the existing SfB meetings will be shown in the app and in the
Calendar as Tеams meetings, and all the participants will get a
notification via email with the new link. SfB client will still be
installed in case people need to join SfB meetings (or they can use
the Skype Meetings app), but Tеams will be their primary client. All calls
and chats will be routed to Teams no matter where they come from.
Meetings scheduled in Outlook will be available only in Tеams.

Improved performance is reached thanks to the advantages of a
cloud-managed service: every time you complain about Teams and file a
bug report or a report saying that something is slow, broken, or not
user-friendly, it is fixed. All the users can benefit from it, as each
month Microsoft pushes out about two new releases with these updates. As
an example, the quality of the Teams meetings is higher than the SfB
ones because clients are running the latest media stack in the
background.

Any existing contact list will be transferred to Teams from SfB Online
in two phases. Even if you're not Tеams only, the very first time
somebody logs in to Tеams, all the contacts will be migrated. New
contacts made in Skype afterward won't be in Tеams, and vice
versa. That's why there's a second and final contact migration before
moving to full Tеams mode. New contacts will be pulled from SfB and
merged into Teams.

### How to upgrade from on-prem SfB and what is migrated

The first and foremost prerequisite for the transition from on-premises
is enabling SfB Hybrid. It will ensure that all msRTCSIP attributes from
on-prem are synced to Azure Active Directory. Surely, you can do without
it, but in this case, on-prem users won't have interop or federation
with their Tеams client.

For versions earlier than SfB Server 2015 CU8, the upgrade will
require two steps: first moving SfB users online with Move-CsUser, and
then executing grant-csTeamsUpgradePolicy. These are two little
PowerShell steps, but it's a single migration, not two migrations, and
it should be planned and tested accordingly.

In the latest CU for Server 2015 and in Server 2019, the code is
updated, and Move-CsUser contains a new switch called MoveToTeams, so
it's a one-step migration.

![](https://o365hq.com/images/478.png)

There might be a problem, looking like this:

![](https://o365hq.com/images/482.png)

Don't panic, everything is fine. What happened is that the settings for
the SfB on-prem users provide them with audio conferencing and
Enterprise Voice (EV). During migration, the system assumes that you
want them to have that same capability. Without a license for the
above-mentioned features, the user is blocked by default so as not to end up
in a misconfigured state. This misunderstanding is worked around in
PowerShell with BypassAudioConferencingCheck and
BypassEnterpriseVoiceCheck.

![](https://o365hq.com/images/481.png)

On-prem users are not going to have their contacts list when they first
log on to Tеams (because migration is conducted from SfB Online). But
when they are finally migrated over in the full version of Teams, they
will have them, as starting from Lync 2013 the contacts can be moved to
SfB Online and pulled over to Tеams afterwards, as was described
before.

When upgrading from the latest version of SfB Server, the meetings will
go to Tеams directly for versions earlier than Server 2015 CU8 to SfB
Online.

### Upgrade tracks

When planning migration, you can choose between two different tracks.

-   IT admin-driven, where you'll be in charge
-   Microsoft-driven automated upgrade, where Microsoft (MS) will
    control it

The difference between these options is who initiates the migration.
Underneath, everything from user experience to core mechanics is the
same.\
The first track is applicable to any organization, but is more suited to
larger online companies (with an SfB admin) or organizations with
on-prem or hybrid users. The admin initiates the migration through
various toolsets (in Teams Admin Center or PowerShell). Depending on
your situation, the users may be upgraded selectively or downgraded for
whatever reason.

The second track presumes Microsoft automatically migrating the whole
Office 365 tenant at once. This track is intended for purely online small
organizations with limited IT resources. As a first step, Microsoft
provides advance notice (typically 30-60 days) sent through the Message
Center, email, and Admin UI, and followed by multiple reminders. Before
the upgrade, admin has an option to postpone it once. Being subject to
automatic upgrade, you can still start it yourself using features of the
first track to self-migrate. Analyzing SfB feature usage, Microsoft can
estimate an organization's eligibility for this track.

Here's a quick table summarizing the above-mentioned tracks.

![](https://o365hq.com/images/479.png)

So, technically, moving to Tеams won't require much attention from admin,
but you need to prepare your users for it to make it go smoothly. 
We already discussed this topic in a previous post, so for more detail, [see
here](o365hq.com/blog/what-are-the-options-to-upgrade-from-skype-for-business-online-to-teams)
. If you've made the move but your users turned out not to be perfectly
ready, you can roll them back to SfB in about five minutes, changing the
org-wide settings.

If you're interested in how your users are doing after the upgrade, you can
track operational excellence with tools like advanced call analytics,
call quality dashboard, and usage reports. These will help you see how
much is being used, and what the common problems are people are walking
into.

Bon chance in your journey to the modern digital workplace!
