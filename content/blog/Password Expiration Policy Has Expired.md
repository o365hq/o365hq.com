+++
title = "Password Expiration Policy Has Expired"
description = "Microsoft released the May 2019 update of security requirements for desktop and server systems, in which regular periodic password changes no longer appear."
date = 2019-06-27

[taxonomies]
tags = ["azure", "cloud security", "security"]
+++

IT security is considered an important priority for business. Regularly
requiring password change as one of the possible ways to provide safety
is widespread in modern practice, although this process is
undesirable for users and its efficiency is questionable. Some people
consider it sufficient to simply change one character at the end of the
line to create a new password.

The practice of regular password change causes a lot of inconveniences
-- you need to create a new password, remember it, and enter it on several
devices. Besides, entering a really strong password from a mobile phone
is an extremely uncomfortable process. All this distracts attention,
takes a lot of time and interrupts work, but many people have to take
such measures for the sake of safety. But is it really necessary to
suffer from all these inconveniences now?

![](https://o365hq.com/images/422.jpg)

*Microsoft Cyber Defense Operations Center*

Microsoft released the May 2019 update of security requirements for
desktop and server systems in which regular periodic password changes
no longer appear. Here is an [official blog
post](https://blogs.technet.microsoft.com/secguide/2019/05/23/security-baseline-final-for-windows-10-v1903-and-windows-server-v1903/)
with a list of changes to the Windows 10 v 1903 version (pay attention
to the phrase Dropping the password-expiration policies that require
periodic password changes). The rules and system policies of Windows 10
Version 1903 and Windows Server 2019 Security Baseline are included in
the [Microsoft Security Compliance Toolkit 1.0
package.](https://www.microsoft.com/en-us/download/details.aspx?id=55319)

**Now that this requirement can be considered outdated, the modern realities
of the IT world have changed.**

Considering the importance of password security and the fact that it was
difficult for the IT department to solve this problem for a long time,
Microsoft explains why they abandoned this practice and mentions the
following points:

-   If an employee sets their own password, it is often too simple and
    easy enough to guess or predict, having some information about the
    employee.
-   If an employee is assigned a complex password automatically, this
    password cannot be remembered and too often people write it down so
    that it can be seen by others, or store passwords in an unsafe
    repository as plain text, which makes it very convenient to steal a
    password, even for a non-skilled attacker.
-   Such regular password change leads to simple adding or changing
    predictable characters. And if the password or its hash is
    compromised, this can be extremely difficult to detect.

How many days is it acceptable for an attacker to use a password?
Windows default time is 42 days, but don't you think this is
impermissible long?

And even more frequent password change will turn the work of employees
into agony.

### What to do?

The new security standard is created for companies that have modern
security management solutions implemented, appropriate policies and
restrictions configured, regular monitoring of activity, and timely
response to suspicious activity.

It also can serve as a guide for auditors. If such an organization
has implemented banned password lists, multi factor authentication,
brute-force password attack and abnormal login attempt detection, does a
password need to be periodically expired? And if they have not
implemented modern protection solutions, will password expiration help
them?

Microsoft principles are simple and clear. There are two options.

1.  The company has modern protection solutions implemented.
2.  The company does not have modern protection solutions implemented.

In the first case, regular password changes only create problems for
employees but do not increase the level of security.

In the second case, regular password changes are simply useless.

Thus, multifactor authentication must be used first instead of the
password expiration. Additional security measures are listed above:
banned password lists, brute-force password attack, and abnormal login
attempt detection.

### Conclusion

If a company forces users to regularly change passwords, what can a
third-party observer think?

**Given:** the company uses an archaic security solution.\
**Supposition:** the company had not implemented modern protection
solutions.\
**Conclusion:** these passwords are easier to access and use.

It turns out that the periodic password change makes the company a more
attractive target for attacks.

We agree with the Microsoft policy and strongly recommend that you start
using modern methods of security management and data protection.

Get a discount on security-related services by providing a promo code --
Modern Security.
