+++
title = "What are the options to upgrade from Skype for Business Online to Teams?"
description = " Switching from Skype for Business (SfB) to Teams is a hot topic. There are a few reasons why organizations are considering it. New Microsoft 365 tenants will be provisioned with Teams only, as it can already offer more features and capabilities than SfB Online, and it’s innovating rapidly. Users get better state-of-art cross-platform mobile experiences. The Teams client is built on a modern infrastructure, which improves operational performance. "
date = 2019-07-09

[taxonomies]
tags = ["microsoft teams"]
+++

At the same time Microsoft is developing on-premises SfB, and it's
already released SfB Server 2019. So, now  clients have the following
options:

![](https://o365hq.com/images/442.png)

When you think about Teams and SfB, you cannot simply compare features
or see Teams as SfB in a different skin on the front end. It takes your
organization to the next level and brings it into the digitally transformed
modern workplace. It is a hub for everything teamwork-related, bringing
all the tooling and products of Microsoft 365 under one umbrella. By
2018, Teams had become the fastest-growing app within Microsoft --- over
300,000 companies were using it.

If your organization is planning to upgrade from SfB to Teams but you're
confused about technical paths and coexistence options, these hints
will help you design your journey.

### Holistic approach

Migration can't be focused on the technical aspect, you need a holistic
approach, and there's a framework for a seamless transition.

![](https://o365hq.com/images/439.png)

Your first step may be getting the right stakeholders, sponsors, IT
department, adoption, and change managers, and everyone in between, that
really has a stake in the game to help make this a successful
transition. Together they will define the vision and the scope of the
project, define your goals, timeline, and indicators that will signal that
you can move to the next level. You might have this big, broad vision of
going all in with teamwork, but the scope at this point in time might be just
to deploy Teams. This project definition will be your foundation and
blueprint to work from in the coming weeks and months. Technical and
user readiness should be organized as parallel work streams, as user
readiness does not happen after the fact of migration. You're testing
the network for quality, but also onboarding your users. From there, you
may run a pilot validating your technical readiness and user adoption.
Then at some point in time, all your users will migrate to Teams and
you'll work on operational strategy. This framework is kind of a bridge
built to get you from Skype to Teams; however, how you cross that bridge
is up to you.\
Every organization is unique, but there's a recommendation from
Microsoft on how to upgrade from online, hybrid, or on-premises SfB, and you
can customize that path to your needs. This guidance is flexible and
adaptable enough to accommodate different deployment scenarios. There
are 5 modes that are the building blocks of the upgrade.

### Teams-only mode

It is the destination of your migration, which will guarantee the most
innovative teamwork and collaboration experience for end users.

![](https://o365hq.com/images/441.png)

Four other modes are stages, or building blocks, you may use in
combination with one another to get to Teams only. During the journey,
you can still preserve some amount of interoperability between SfB and
Teams so that your upgraded users can communicate with non-upgraded
ones internally (within your organization) and externally (with
partners using SfB).

### Islands mode or side-by-side deployment

This deployment mode is recommended for purely online organizations (with
SfB Online) that are relatively simple-structured, small, and probably
don't have a dedicated IT department. Islands mode means that users will
enjoy using Skype and Teams simultaneously, getting the full benefit as
they run both. Teams offers chat, calling, meetings scheduling, the
ability to do teams in channels, integrate third-party applications, and
more, for the richest possible experience of Teams. Every time users want
to contact somebody, they have a choice, and look at both SfB and Teams
to check for new messages. When they schedule meetings, they have two
plug-ins in Outlook and have a choice again. This rich, out-of-the-box
experience should help to get to Teams more quickly.

![](https://o365hq.com/images/440.png)

### Teams without the UC functionality, or SfB with Teams Collab

This mode is recommended for SfB on-prem, hybrid, or even online
organizations if they have concerns that doing the same stuff in two
different apps would cause confusion. You keep SfB for UC functionality
(by the way, UC stands for unified communications, and here means chat,
meetings, and calling), and add in Teams without the UC. Nothing will
change from a SfB perspective; employees will do what they've always
been doing. They will just get some stuff that is brand-new, like
channels or third-party apps integration and much more for group
collaboration.

Eventually, when you feel your users are ready, you shift them to the 
Teams-only mode, taking the UC functionality out of Skype and moving it to
Teams. What's fundamentally different from the previous approach is that
these users never could do the same thing in more than one app.

![](https://o365hq.com/images/443.png)

You might be wondering what happens if a Teams-only employee needs to
talk to a SfB user. Throughout the phase of the transition, each person
has one client where the calls and chats will always land. The routing
assures that if it's a Teams user, the message is going to Teams,
wherever it came from. The same applies to SfB. It's better to go quickly
through this phase, and don't hang out in the middle state. Decommission
all the other stuff as soon as possible and end up with everybody in
Teams.

### SfB with Teams Collab and Meetings

This scenario is for organizations that are excited about going to Teams
only, but it might take them a while because of some constraints around
Enterprise Voice on-prem, for example. They might be bound by contracts
for X number of years, or they've got to amortize some old legacy
equipment, or they've got a boss who can't agree to go to Teams only.
This mode is a variation of a previous one, where you add Teams without
UC functionality, but the next step is to switch the Meetings out of
Skype and into Teams. Under Meetings we mean meeting scheduling, so SfB
users will schedule their meetings in Teams. Any Skype user can join
the meeting in Teams, and any Teams user can join the meeting in Skype,
so only scheduling will eventually matter.

![](https://o365hq.com/images/444.png)

Let's explain how the notion of Meetings in different clients works. To
join a meeting, you need a client that knows how to talk to the relevant
service. Teams and SfB are different sets of code with different
services underneath, so there does not exist one client that talks to
both. However, any user can join either, thanks to a web client. If
you're a Teams-only user invited to a SfB meeting, the Skype web
client will help you out. The reverse is also true; if you're a Skype
user who never used Teams before but was invited to a Teams meeting, you
can join in thanks to a lightweight browser plug-in.

![](https://o365hq.com/images/445.png)

### Skype-only mode

This is a scenario for companies with strict requirements (e.g., for data
control) or for those that are waiting for certain features on the
roadmap not available at the moment. It is even possible to roll back
to SfB if you need to for any reason.

If you don't migrate your users at once, you're going to be  in a situation 
within your company where you have some
users in SfB and some in Teams. Even after you are a Teams-only entity,
you need to ensure communication between SfB users from other
organizations and your Teams users. This communication, specifically
chatting and calling (as we already know how it works with Meetings), is
achieved thanks to the interop. How does it work? At a basic level, we're
talking about a client in Teams that uses http protocol, and a client
in Skype that uses sip protocol. Somewhere in the cloud there's a
gateway where all the magic happens, and it translates sip to http. There
are some prerequisites to benefit from the magic. Number one, you will
need to set up SfB hybrid topology. Interop and federation (which is the
ability to connect and communicate with SfB users in other
organizations, based on the agreement) are only available when the SfB
user who was originally on-prem gets moved into the cloud. Every Teams
user has a shadow Skype account, and to get interop and federation, this
Skype account should be in the cloud. You can still use Teams prior to
doing that, you just won't have interop or federation. Interop enables
chat (plain text, no gifs) and one-to-one calling.

### Example of a customer journey

In the picture below, a staggered approach, which aligns feature releases
(that are on the roadmap) to users' groups is shown. It starts with
assessing the employees, depending on their work, and the features they
use, and dividing them into cohorts.

![](https://o365hq.com/images/446.png)

Based on the analysis of cohorts, the first two groups were migrated to
Islands mode. The next two cohorts were transferred to Group Collab and
Meetings Only mode. The last cohort was left with Group Collab only, as
they needed the ability to record meetings, not available in Teams at
that time. So, at the evaluation stage, everyone had Teams client,
ability for group collaboration, and ability to join meetings in Teams.
As the timeline moved along, the first two cohorts moved to Teams single
client mode, while the HR and Sales departments stayed with the same mode.
The reasons might be different, like you might be waiting for some
features, or don't want to disrupt their environment at the end of the
fiscal year. Then mapping out users and features, you might find out
that cohort five could now enjoy scheduling meetings in Teams, as all
the features they needed were in place. So, as the journey progressed,
cohorts from 3 to 5 used SfB for chat and calling, could join the Skype
meetings, but scheduled their meetings in Teams. When all the groups
were ready, they were transitioned into Single Client mode.

### Conclusion

Teams is a choice that you're making and a choice that your end users
are making. This is a big change in the way your organization works, and
a big change for end users well-engrained in Skype for Business. There
are five main modes (variations of SfB and Teams coexistence) that may
make the transition smoother. Teams-only mode should be your end goal.
There may be reasons you can't get there right away, but that should be
the end target. If you're a purely online organization and don't have any
complex requirements, the Islands mode with the full functionality of
Teams is recommended. If you're on-prem, or hybrid, or if you know that
your users are going to have a hard time doing the same stuff in more than
one client, then try SfB with Teams Collab, and from there get to Teams
only. A subset may be adding the Teams Meeting scheduling or staying SfB
only.

![](https://o365hq.com/images/447.png)

Now that you've learned how to design your transition, are you excited
to know how to do it from a technical perspective? We'll reveal all
the details in the following article. To be continued...
