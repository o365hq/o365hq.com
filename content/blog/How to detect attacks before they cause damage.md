+++
title = "How to detect attacks before they cause damage"
description = "We are excited to start a series of scenarios on how to improve your Office 365 security and productivity, prepared by Microsoft engineers. The first one is about how to detect attacks before they cause damage."
date = 2018-12-04

[taxonomies]
tags = ["advanced threat protection", "cloud security", "microsoft 365", "office 365 tenant"]
+++

Traditionally, security investments were focused on protection. With
Microsoft Solutions such as EM+S, it is imperative to also have good detection
and response. IT organizations should focus on an approach that looks at
how to protect, detect, and respond to threats.

To address the requirements of this scenario, EM+S uses "Advanced
Threats Analytics", [Cloud App
Security](https://buymssoft.com/services/office-365-addons/mobility-and-security/CSP-ELIT-5b5c193d1138)
and [Azure Active Directory
Premium](https://buymssoft.com/license/GN9-00002) . By implementing
these technologies, organizations will be able to:

1.  Detect or identify abnormal behavior using innovative behavioral
    analytics and anomaly detection technologies leveraging machine
    learning.
2.  Detect known malicious attacks (i.e., Pass the Hash, Pass the Ticket)
    and known security vulnerabilities.
3.  Focus on what is important, fast, clear, and relevant attack
    information.
4.  Identify anomalies and policy violations that may be indicative of a
    security breach.

When you open the attack timeline in ATA, you see a
comprehensive report with suspicious activities showing the entities
that were involved in this activity and what the recommendations are.

![](https://o365hq.com/images/182.png)

Let's see the high-priority issues caused by suspicion of identity
theft. According to the report here, the user, Michael Dubinsky's,
credentials may have been stolen and used to gain access to
resources that Michael doesn't usually access. Let's trace the sequence
of events that led to Michael's identity theft.

![](https://o365hq.com/images/183.png)

![](https://o365hq.com/images/186.png)

As with many attacks, this one begins with a reconnaissance phase where
we see the attacker attempting to guess usernames. Ultimately, the
attacker(s) succeeded and guessed three different accounts, including
Michael's user account.

![](https://o365hq.com/images/185.png)

In the next phase of the attack, we will clearly see the attacker
attempting a brute force attack, including them guessing Michael's
password.

![](https://o365hq.com/images/184.png)

![](https://o365hq.com/images/187.png)

Once Michael's account was compromised, we can see the user behaving
abnormally. With the list of alerts prior to this, we have sufficient
evidence to conclude that this user's credentials are now compromised.

![](https://o365hq.com/images/188.png)

As you might see, in this instance, the attack was detected by
ATA with the help of data provided by a third party
SIEM solution that was configured to forward Windows security
events to ATA. The third-party software was already collecting
these events, so no additional configuration was required beyond the
event forwarding itself.

All of ATA's detection algorithms are self-learning, allowing
it to detect suspicious activities from the first minute it's deployed,
without the need to configure or tweak rules, baselines, or thresholds;
you simply plug it in and off it goes. You can also configure
ATA to send an event to your SIEM.

In summary, ATA uses machine learning in its deterministic and
detection engine to establish an understanding of the normal patterns of
behavior for both users and entities, and it's that unique capability
that provides timely and accurate alerts across a huge variety of attack
vectors.

Also, we provide [Free Office 365 Security Assessment](o365hq.com/services/free-office-365-security-assessment-service). We can help you evaluate how secure your business really is and find a
solution that will help to simplify security and reduce costs while
still getting the protection you need.
