+++
title = "Hybrid Office 365 Migration from your own Exchange Server"
description = "Hybrid migration provides integration between an on-premises Exchange organization and Office 365 Exchange Online. It can be used in two scenarios: as a method of migration between an on-premises Exchange Server and Office 365 (Exchange Online) or as a permanent state for your on-premises Exchange and Office 365 organizations. "
date = 2018-02-01

[taxonomies]
products = ["Exchange Online"]
types = ["Migration"]

[extra]
sku = "ITPWW120MIGOT"
price = "$800 + $25 per mailbox"
duration = "2 weeks"
manager = "Mike Mackey"
+++

A hybrid deployment offers companies the ability to extend the
functionality of an existing on-premises Microsoft Exchange to Exchange
Online. This provides a single space between an on-premises
Exchange organization and Exchange Online in Microsoft Office 365.

The following topology example provides an overview of a typical
Exchange 2016 deployment. With a single-forest, single-domain
organization with two domain controllers and one Exchange 2016 server
installed, we start deploying and configure a required Azure AD Connect
server and use the Azure AD Connect password synchronization feature to
let users log in with the same credentials for both their on-premises
network account and their Office 365 account. Then we complete the
hybrid deployment prerequisites and use the Hybrid Configuration wizard
to select options for the hybrid deployment.

Your new topology will have the following configuration:

Users can log in to the on-premises and Exchange Online organizations
with the same username and password ("single sign-on").\
User mailboxes located on-premises and in the Exchange Online
organizations will use the same email address domain.

All outbound mail is delivered to the Internet by the on-premises
organization. The on-premises organization controls all messaging
transport and serves as a relay for the Exchange Online organization
("centralized mail transport").

On-premises and Exchange Online organization users can share calendar
free/busy information. Organization relationships configured between
on-premises and Exchange Online also enable cross-premises message
tracking, MailTips, and message search.

The same URL is used for the connection to mailboxes for both
on-premises and Exchange Online users.

### IT Partner responsibilities:

1.  Analyze the current Exchange On-Premises solution
2.  Prepare the current configuration of Exchange and Active Directory
    for synchronization
3.  Set up synchronization of users and passwords
4.  Provide informational letters for users
5.  Migrate mailboxes
6.  Provide break-fix support related to migration issues

### Client responsibilities

1.  Coordinate Client resources and staff schedules
2.  Provide a dedicated point of contact responsible for working with IT
    Partner
3.  Provide access to physical and virtual servers and/or systems and
    services as needed. Provide remote and/or physical access to
    facility and systems required to complete the work 
4.  Configure workstations and mobile devices
5.  Perform changes to internal and external DNS, as required
6.  Assist with identification of high-risk users (top executives
    and VIP users, users with 50 GB mailboxes or larger and/or
    30 GB deleted folders or larger)
7.  Coordinate any outside vendor resources and schedules
8.  Configure all network equipment, such as load balancers, routers,
    firewalls, and switches.
9.  Review and approve engagement deliverables in a timely manner

### Additional cost items not provided by the project

1.  Customer team training (could be added as an additional service)
2.  Desktop software settings
3.  Unified Messaging (US) features cannot be used in a hybrid solution
    in conjunction with Office 365. If you use this feature in your
    infrastructure, additional settings can be required depending on the
    solution you are using.

Upon completion of the project, we will provide a project closeout
report. This document will indicate the final project status,
including acceptance criteria matching, outstanding issues (if any), and the
final budget. If you require more extensive documentation, it can be
provided for an additional fee. 

### Prerequisites

1.  You must have an Office 365 tenant with Exchange Online licenses
2.  You must have access to your email domain DNS zone
3.  You need a full installation of Exchange 2010, 2013, or 2016 server
    in your environment with a valid UCC SSL certificate

### Plan

The plan may vary depending on your needs.

1.  Kickoff meeting
2.  Pre-migration source system health check
3.  Creating users or AD connect tool configuration
4.  Migration planning
5.  Email migration start
6.  Email migration check
7.  Changing MX record to the new Office 365 tenant
8.  Final email migration
9.  Post-migration tasks

### Success Criteria

1.  Users can access Exchange Online on their desktop PCs, mobile
    phones, and tablets from any place, any time
2.  Mailbox data is successfully migrated to Exchange online and
    accessible to all users
3.  All necessary transport rules are created and working
4.  Mail can be sent and received using Exchange online
5.  Exchange Online Protection is configured and working
