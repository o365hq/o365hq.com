+++
title = "Your Office 365 account has been compromised or hacked. What’s next?"
description = "One of the most common security support requests from our customers is for assistance with remediating an account compromise. The most common scenario is that a member of their organization became the victim of a phishing scam and the attacker obtained the password for their account. "
date = 2019-11-01

[taxonomies]
tags = ["cloud app security", "cloud security", "security"]
+++

So, that happened... One way or another, your credentials leaked outside
of your organization and bad
actors^[1](#fn11128003305dfd0fba79395-1)^ gained access to your
account. Maybe you clicked on the link in the
[phishing](https://en.wikipedia.org/wiki/Phishing) email and typed in
your login and password on the legitimate-looking phishing website. Or
someone stole your notebook that was not protected with the password
and Bitlocker encryption, or something else happened...

Now, expect the worst -- bad actors downloaded a copy of your mailbox
with all your emails, contacts, attachments, calendar items, tasks, etc.
Also, they have all your OneDrive for Business documents and documents
shared with you and documents and information that they can access using
your account permissions in your company infrastructure. This
information could be stored indefinitely and used against you at any
time.

Depending on what bad actors see in your mailbox, inside your
documents and your organization's systems, they may treat your account
differently. The best outcome is when they don't see any opportunity to
steal money or information and they use your account to spread
laterally^[2](#fn11128003305dfd0fba79395-2)^ **INSIDE** and
**OUTSIDE** of your organization. They start sending hundreds
of phishing emails to your contacts using your name, and your account gets
blocked by Office 365 protection mechanisms and that's it. The worst
outcome is when bad actors see some potential to steal something and
they hide and wait and learn how you and your organization operates over
the long-term, often measured in months. During that time, they don't make
any obvious and noticeable changes or actions but gather information and
try to spread laterally **INSIDE** your organization to get
access to other user accounts, systems, and services that will help them
achieve their malicious goals.

So, what's next? {#so-whats-next style="text-align:center;"}
----------------

1.  **Block the user** from signing in.
2.  **Contact your CSP** and let them know about what happened.
    We at **IT Partner** provide a free 24/7 [Security Incident Response
    service](https://buymssoft.com/constructor/services?item=ITPWW220MSPRC)
    for all our clients who purchase Office 365 subscriptions through
    us. If you are not our client -- please call anyway, we would be
    happy to help.
3.  Try to **understand the intentions** of the bad actor(s).
    1.  Study your Office 365 sign-in logs and security reports. What
        services have they accessed? For how long? Using what devices? From
        what locations? Start with [AAD sign-ins
        log](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade/AllUsers).
    2.  Did they send any emails? To whom? How many? Go to the [Exchange
        Online Admin Panel](https://outlook.office365.com/ecp), click
        "Message flow", then select the "Message Trace" tab. While in
        EXO Admin Center, also check the Transport Rules and
        Connectors tabs.
    3.  Did they create any personal email rules?
    4.  Did they set up an email forwarding outside your organization?
    5.  Did they manage to install anything on your devices?
    6.  If you have a CAS subscription, you will be able to see
        each and every action of the user, every single accessed file
        for up to six (6) months after the incident.
4.  **[Delete the Inbox email
    rules](https://support.office.com/en-us/article/inbox-rules-in-outlook-web-app-edea3d17-00c9-434b-b9b7-26ee8d9f5622)**
    not created by the user. Criminals often create rules to delete all
    or a portion of the incoming email to slow down the incident response
    actions.
5.  **Inform your colleagues** inside or outside of your organization
    about what happened if bad actors sent a phishing email to them.
6.  **[Remove a user from the Restricted Users
    portal](https://docs.microsoft.com/en-us/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)**,
    if needed.
7.  **Install all the updates** for Windows OS and Office Suite.
8.  Make sure you have Windows OS **Firewall feature enabled** and
    properly configured.
9.  Check the **recovery email address** and phone number associated
    with the user account.
10. **[Enable and Enforce
    MFA](https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/set-up-multi-factor-authentication?view=o365-worldwide)**
    (Multi-Factor Authentication) for this user. MFA is the
    single most efficient protection from all attacks based on
    phishing techniques. It must be enabled at all times for all the
    users in your organization. We recommend setting up a Baseline
    Security Policy or enabling the Security Defaults for your
    AAD tenant.
11. **Disable the IMAP protocol** for all your mailboxes.
    IMAP is often used for Password
    Spray^[3](#fn11128003305dfd0fba79395-3)^ attacks, which are
    practically undetectable.
12. **Reset user password** and **unlock the account**.
13. **Educate your users**.
14. OPTIONAL: Think about adding the [Cloud App
    Security](https://buymssoft.com/license/CSP-ELIT-00e8ff14e7b2)
    subscription to all or some of your users.
15. OPTIONAL: Think about subscribing all or some of your users
    to [Office 365 Advanced Threat Protection Plan
    1](https://buymssoft.com/license/CSP-ELIT-0c69e5c76b63).
16. OPTIONAL: Think about your historic emails and documents
    that are now at the bad actor's disposal. What can they find there? Can
    you take any proactive steps to prevent them from using that
    information?

Again, we strongly recommend setting multi-factor authentification (MFA) for
all users and follow all other prioritized security-related
recommendations provided by Microsoft Secure Score service, which is a
free service provided by Microsoft as part of your Office 365
subscription.

These instructions will help you take immediate action to recover
from the incident. Unfortunately, you will not be able to delete and
revoke the messages sent from your account under your name or prevent
bad actors from using the information they stole. But with the right
combination of user training, internal anti-phishing mail flow rules,
MFA, and spam protection, you can easily prevent such account
compromises in the future.

### IT Partner is always [ready to help you](https://o365hq.com/services/) build a safe and secure environment and protect your sensitive data. {#it-partner-is-always-ready-to-help-you-build-a-safe-and-secure-environment-and-protect-your-sensitive-data. style="text-align:center;"}

.

#### Footnotes:

^1^ *Bad actor* -- A cybersecurity adversary that is interested in
attacking information technology systems.

^2^ *Lateral movement* refers to techniques cyberattackers use to
progressively move through a network, searching for targeted key data
and assets.

^3^ *Password spraying* is the attack method that takes a large number
of usernames (millions) and loops them with a single password. Bad
actors can use multiple iterations using a number of different
passwords, but the number of passwords attempted is usually low when
compared to the number of users attempted. This method avoids password
lockouts, and it is often more effective at uncovering weak passwords
than targeting specific users with multiple passwords.
