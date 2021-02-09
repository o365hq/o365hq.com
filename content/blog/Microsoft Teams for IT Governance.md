+++
title = "Microsoft Teams for IT Governance"
description = "Governance is the process of planning and executing Teams deployment across an organization. It involves these main areas:"
date = "2020-09-21"

[taxonomies]
tags = ["microsoft teams"]
+++

1.  Group and team creation, naming, and classification
2.  Group and team expiration, retention, and archiving
3.  Teams feature management

Time invested in Teams governance will pay dividends after adoption,
including smoother rollout, better user experience, and fewer helpdesk
calls.

Teams provides rich governance tools to implement policies and
permissions for creating, naming, and classifying teams and for
controlling who can use them.

![](https://o365hq.com/images/825.png)

Teams is one of several Office 365 services built on the Office 365
Groups framework. When someone creates a team, an Office 365 group is
created as well. By default, all users with a mailbox in Exchange Online
have permissions to create Office 365 groups and, therefore, a team in
Microsoft Teams. This certainly eases the burden on admins who might
receive hundreds of requests to create teams, but it can also lead to
issues like team duplication or inadvertent deletion of teams and
content. If you want to have tighter control and restrict the creation
of new teams, you can delegate group creation and management rights to
an Office 365 Security Group in the **Office 365 Admin Center**.

It's important to note that Teams yields the most benefits when there is
a good balance between allowing end-users to create the teams they need,
while restricting an uncontrolled rapid increase in the number of teams
created. Severely restricting the creation of teams is not recommended.

With a security group in place, you can then use **Azure Active
Directory (AD) PowerShell** to configure the permissions. By default,
anyone who creates a team can name it whatever they wish. However,
without proper controls, this can lead to organizational headaches.

![](https://o365hq.com/images/826.png)

To enforce consistent naming conventions for Teams, you can set up a
naming policy for your company tenants using **Azure AD PowerShell**.
For example, you could use prefixes and/or suffixes to communicate
geographic region (as in the above example), the function of a group,
its membership, or who created the group. You can also create a list of
blocked words that cannot be used in a team or group name, such as
Payroll, CEO, HR, etc.

After you set a group naming policy in Azure AD, when a user creates a
group in an Office 365 app, they see:

1.  A preview of the name according to your naming policy appears (with
    prefixes and suffixes) as soon as the user types in the group name.
2.  If the user enters blocked words, they'll see an error message, so
    they can remove the blocked words.

Each team created in Teams automatically comes with an Office 365 Group,
with configurable status (public or private) and optionally,
\*classifications\*---which are labels that administrators can use to
create policies for retention and other content-related requirements in
Office 365. For example, the admin can allow users to set "Public",
"Internal Only", and "Restricted" on teams they create.

![](https://o365hq.com/images/824.png)

Setting up the classification scheme requires Azure Active Directory
PowerShell. Once the classifications are configured, users will see an
option to classify the team they create by editing team details.

In Microsoft Teams, Channels are dedicated sections within a team, open
to all team members, to keep conversations organized.

Using Private Channels, you can create a more focused collaboration
space within a given Team. In such cases, you can add Private channels
to the team for communication, without having to create a separate team.

A guest is someone who isn't an employee, student, or member of your
organization. They don't have a school or work account within your
organization. For example, guests may include partners, vendors,
suppliers, or consultants.

Guest access in Microsoft Teams allows teams to collaborate with people
outside the organization by granting them access to teams and channels.

Anyone with a business or consumer email account, such as Outlook,
Gmail, or others, can participate as a guest in Teams with full access
to team chats, meetings, and files.

You can manage Microsoft Teams guest access features and capabilities
through different levels of authorization, including Azure Active
Directory, Teams, Office 365 Groups, SharePoint Online, and OneDrive for
Business. Each authorization level controls the scope of guest access.

As the number of teams increases, it can create a bit of a mess -- for
instance, when a project is completed but the team and Office 365 group
is still hanging around. Microsoft Teams now shows team owners when
their team is going to expire -- that is, if they use the Office 365
Groups expiration policy.

You can manage the lifecycle of teams by setting an expiration policy in
the **Azure AD admin center**.

![](https://o365hq.com/images/827.png)

An expiration policy can be set for all groups, specific groups, or none
of the groups. Team owners can archive a team when it's no longer
active, but they want to keep it for reference or to reactivate in the
future. The conversations and files in the team become read-only once
archived. Users will still be able to search through it for what they
need.

All team activity is frozen once the team is archived. No one will be
able to start new conversations or reply to posts in a channel, add or
remove channels, edit team settings, or add apps. Team owners will still
be able to add or remove members, update roles, and delete or restore an
archived team.

For most organizations, the volume and complexity of their data is
increasing daily -- email, documents, Teams messages, and more. To
manage or govern this information is important for admins need to:

1.  Comply proactively with industry regulations and internal policies
    that require organizations to retain content for a minimum period.
2.  Reduce their risk in the event of litigation or a security breach by
    permanently deleting old content that organizations are no longer
    required to keep.
3.  Help organizations share knowledge effectively and be more agile by
    ensuring that their users work only with content that's current and
    relevant to them.

With Teams retention labels and policies, admins can decide proactively
whether to retain content, delete content, or both -- retain and then
delete the content based on time.

![](https://o365hq.com/images/829.png)

Retention policies can be configured in the **Compliance center**.
Policies are applied by using content labels that can be either
auto-applied or applied by users. If a new retention label and policy is
needed, you can create a new one.

Another important aspect of governance and lifecycle management for
Teams is the ability to control what features of the service users will
have access to. Teams provides granular capabilities for controlling
features including meetings, messaging, calling, live events, and more.

These settings can be made through policies in the **Teams Admin
Center**. Meeting policies are used to control what features are
available to users when they join Microsoft Teams meetings.

![](https://o365hq.com/images/828.png)

**General meeting** settings cover areas such as enabling Meet Now,
channel meeting scheduling, and the Outlook add-in.

**Audio & video** settings include transcription, recording, and media
bit rate.

**Content sharing** settings include screen sharing, giving and
requesting control, sharing a PowerPoint deck, and more.

**Participants & guests** settings include dial-out to add other
participants, enabling any user to start a meeting, and automatically
admitting participants. An existing policy can be changed and saved, or
you can easily start a new policy from scratch.

![](https://o365hq.com/images/830.png)

With Microsoft Teams live events, users can broadcast video and meeting
content to large online audiences.

Live events bring live video streaming to a new level, encouraging
connection throughout the entire engagement lifecycle with attendees
before, during, and after events.

Live events policies are used to manage event settings for groups of
users. You can use the default org-wide **Global** policy or create new
policies and assign them to users.

Live events policies contain these options:

1.  Allow scheduling (enables a user to schedule a live event).
2.  Allow transcription for attendees.
3.  Set who can join scheduled live events---everyone, everyone in the
    organization, or specific users or groups.
4.  Recording settings---always, never, or meeting organizer only.

Messaging policies are used to control what chat and channel messaging
features are available to users in Teams. As in the case of meetings and
live events policies, you can use the default org-wide **Global** policy
or create one or more custom messaging policies for people in your
organization.

![](https://o365hq.com/images/831.png)

There are several options in a messaging policy, including:

1.  Whether owners and/or individual users can delete or edit a sent
    message
2.  Enabling read receipts
3.  Enabling chat
4.  Enabling Giphys, and controlling their content rating
5.  Using memes and stickers in conversations
6.  Allowing URL previews
7.  Allowing message translation
8.  The Global policy bars owners from deleting sent messages but allows
    users to delete or edit them. Chat, Giphys, memes, and stickers are
    all allowed, as are URL previews and translation of messages.

Teams provides a rich set of tools to implement any governance
capabilities your organization might require.

![](https://o365hq.com/images/832.png)

The time taken to set options and policies for Teams that meet the
unique needs of an organization will bring solid dividends including
strong and smooth user adoption, consistent team naming and life cycles,
and improved data security.