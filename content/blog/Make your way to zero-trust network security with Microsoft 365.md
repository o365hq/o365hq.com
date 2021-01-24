+++
title = "Make your way to zero-trust network security with Microsoft 365"
description = "Previously, we discussed the subject of zero-trust network security, but at the Security and Compliance Virtual Conference that took place recently, experts talked a lot about zero-trust architecture in the Microsoft 365 environment, and we’ve decided to share some of the most interesting insights from the conference."
date = 2019-05-29

[taxonomies]
tags = ["cloud security", "microsoft 365"]
+++

The notion of zero-trust was introduced back in 2010 by John Kindervag,
but recently it has gained extra notoriety and interest in the security
industry, primarily due to the volume of data breaches we've seen across
organizations. These breaches proved that traditional network perimeter
architectures have serious flaws and just don't work in today's world
of progressive workforce mobility, a movement to cloud services, and
[BYOD]{.caps} model.

The crux of the zero-trust concept is about making sure that every time a
resource is accessed, you can assess how trustworthy that access or
request is.

When we think about zero trust, it's more like zero trust in the
network, where:

-   *Every asset* you have is available *on the open internet* (because
    that's the way things are in real life).
-   You *assume breach*, supposing that somebody's already in the
    network and you have to set up policies and controls to avoid data
    leakage.
-   There's *no inherited trust*, and you must *always verify*.

Organizations today are connected to a variety of complex ecosystems --
they have broad on-premises infrastructure, they are leveraging cloud
services, have a vast array of partners with access to their network; they
may be using IoT devices to manage buildings and infrastructure,
industrial control systems, and have supply chains in terms of doing B2B
types of transactions. Handling all that requires a complex
approach to integrated protection and governance of sensitive data
across devices, apps, and cloud services. This is what Microsoft has to
offer:

![](https://o365hq.com/images/345.png)

The zero-trust concept here is built around identity and conditional access.
Creating a policy, you may use various conditions under which controls and
managing access to data are implemented. For example, your company will
be able to define conditions based on things like which users are
trying to sign in, with which application, which device they are using,
and where in the world they are trying to sign in from.

Let's see how zero trust works from the position of admins, setting up
policies, and the perspective of users doing their job. At the end,
we'll share some best practices.

### Admin's view

The main portal for admins to configure conditional access will be Azure
Active Directory ([AAD]{.caps}). As an example, let's set [MFA]{.caps}
for every access to SharePoint. Basically, you have two elements:
*Assignments* and *Access controls*. Under the Assignments, conditions
are listed, and they are the selectors for the policy. If these
conditions are met, [AAD]{.caps} will fire the policy.

Microsoft has recently added two cool features to these conditions. The
first one is that now *conditional access policies may be assigned by
roles*, so if you want, your Exchange admin to be under a
specific policy, for example, that's much easier to do. The other new thing is that
you'll have full support for B2B, as you may grant access to
business partners under conditions you prefer.

![](https://o365hq.com/images/340.png)

Every internal and external application, whether it's Microsoft, a
third-party SaaS, or your on-premises applications (connected through
the app proxy), may be under the management of the conditional access,
creating a consistent security model for all workloads.

![](https://o365hq.com/images/346.png)

Below, the setting of sign-in risk as a selector is shown --- one just
has to pick the proper risk levels to fire that policy.

![](https://o365hq.com/images/338.png)

It's high time to look at the controls that are applied when the policy
matches. In the first section of *Grant* controls, you pick extra things
users will be required to do (like [MFA]{.caps}) or to have (like a
complaint or [AAD]{.caps} joined device) to get access.

![](https://o365hq.com/images/339.png)

In this example, we'll select [MFA]{.caps}. One of the side benefits of
[MFA]{.caps} is it gives you the step up into the second factor of
authentication if something risky is detected, but it will also
eliminate some prompts if a situation looks safe enough. For example,
if users are within an IP range that [AAD]{.caps} knows and trusts
(like your own set of IPs), in a location that users are always logging
in from (maybe their home), and the same device all the time, [AAD]{.caps}
can actually start to reduce some second-factor obstacles, still
preserving the same security level.

Granting access is just a beginning. There's also the ability to
instruct the system to do downstream things with *Session controls*.
Selecting *Use app enforced restrictions*, you let apps provide only
limited capabilities under certain conditions. If [AAD]{.caps} detects
something suspicious about the session, it will pass this additional
information to the cloud app, which in turn will enable a limited
experience, without the ability to download, print, or sync files.

Conditional access app control lets you invoke Microsoft Cloud App
Security ([MCAS]{.caps}) to get some rich front signal and auditing
while monitoring user behavior within the app in question. Let's say
you have a user who's at risk because of a sketchy login, and you may
want to see what that assumed attacker is doing: literally and
laterally follow him/her. This gives you incredible power in terms of
thinking about your security model and additional controls needed. While
using this feature, you're verifying and controlling everything by
redirecting a user through a [MCAS]{.caps} reverse proxy (not to the app
itself), which lets you inspect and export traffic logs.

![](https://o365hq.com/images/343.png)

### User experience

From the user's perspective, let's view the device-based conditional access
policy. Trying to sign in from an unmanaged, untrusted personal device
will result in the [MFA]{.caps} challenge and ban downloading, printing, or
syncing information (to control the data flow).

The situation on a managed device will be frictionless with true app
single sign-on ([SSO]{.caps}), and without the need for additional
[MFA]{.caps} challenges. Thus, the user experience improves and
security controls are maintained because of the certificate-based
nature of the environment, in which we do device-based conditional
access.

![](https://o365hq.com/images/349.png)

Conditional access and identity security are not limited only to signing
in to your applications. It is possible to incorporate these into data
itself with Azure Information Protection ([AIP]{.caps}). Labels may be
applied automatically or by users creating the file in Office and
third-party apps. Through this classification, you can apply encryption
at the file level, and only the proper identity can unlock the
information. Encrypted files can be stored in any location (OneDrive,
Dropbox, [USB]{.caps} key, email, etc.), but for the person or system
to get access to it, credentials should be entered to prove the
identity.

### Best practices

**Block legacy authentication**

This recently added capability is intended to exclude legacy protocols
that won't allow the carrying out of the [MFA]{.caps} challenge and monitoring the
session. Turning on this policy is important, as the attackers are using
tools relying on protocols like [POP]{.caps}, [IMAP]{.caps},
[SMTP]{.caps}, etc. When you stop the use of these clients altogether,
you eliminate all the vulnerabilities that come along with these
protocols. Microsoft has found statistically that this policy stops 66%
of the compromises in your work.

Excited to try this out? Look for *Conditions*, then *Client apps*
and choose *Other clients* to not let in any apps using legacy
authentication.

![](https://o365hq.com/images/341.png)

This is what the denial to log in resulting from this policy will look
like with Pegasus client.

![](https://o365hq.com/images/348.png)

**Require [MFA]{.caps} for admins**

Having experience in the investigations of major breaches, Microsoft
is creating a set of turnkey baseline policies that you just simply
turn on. Among these is configuring stronger credentials for admins.

![](https://o365hq.com/images/344.png)

**Identity Secure Score**

Extending a little bit farther in terms of guidance, best practices, and
how to create a very secure environment in the zero trust mindset,
Identity Secure Score was introduced.

Secure Score has been around for a while in Office 365, and then in
Microsoft 365. Eventually, specific places were defined for different
admin roles: there's an identity-specific place for the identity admin,
a network-specific place for the network admin, the infrastructure
admin, and so forth. The Identity Secure Score is what identity folks
can address to see what makes the biggest impact on improving the
security posture, and then build a plan around it.

![](https://o365hq.com/images/347.png)

On top of the *Improvement actions* are *Enable [MFA]{.caps} for Azure
AD privileged users*. Clicking on it, you will see the quick explanation
of what to do, and at the bottom, there is a *Get started* button, which
will take you right back to that baseline policy to turn it on. If this
recommendation is enabled by a *Third-party product*, or if you want to
*Ignore it*, as it doesn't apply to your environment, you have such
options under the *Status* drop-down.

![](https://o365hq.com/images/337.png)

### Conclusion

Building a zero-trust network is the right way to achieve security goals.
By putting conditional access restrictions in place, you extend the
horizon of productivity, as employees work effectively while the data
remains protected from downloading to the local drive and from the
attacks, as [MFA]{.caps} has 99.9% effectiveness in blocking
identity-based attacks. Knowledge is power; start empowering your
company now!
