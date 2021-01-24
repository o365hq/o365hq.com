+++
title = "Cutover G Suite to Office 365 Migration - Just Email and Email Folders"
description = "Migration of email data and email folders from G Suite (Google Apps) to Office 365 / Exchange Online."
date = 2018-02-02

[taxonomies]
products = ["Exchange Online"]
types = ["Migration"]

[extra]
sku = "ITPWW150MIGOT"
price = "$3 per mailbox"
duration = "1 week"
manager = "Mike Mackey"
+++

*Note: If you have contacts, tasks, and calendars in your mailbox and you
need to migrate this data in addition to your email messages and email
folders, then you need a different Service -- G Suite to Office 365.*

We can migrate the content of user mailboxes from your source email
system to Office 365. We will use the Internet Message Access Protocol
(IMAP) to migrate email. Please note that only email and email
folders will be migrated.

Our objective is to provide planning, design, and migration from G Suite
mailboxes to Office 365 tenant via IMAP protocol without
downtime or data loss and with minimal user disruption.

The migration project will be considered successful if all mailboxes are
moved to Office 365.

### IT Partner responsibilities

1.  Gather information and verify the original G Suite
2.  Configure the destination Office 365 tenant
3.  Create and configure users
4.  License assignment
5.  Create and configure a migration plan
6.  Provide informational messages for users
7.  Start and control the data migration process

### Client responsibilities

1.  Provide a dedicated point of contact responsible for working with IT
    Partner and coordinate any outside vendor resources and schedules
2.  Coordinate Client resources and staff schedules
3.  Review and approve engagement deliverables in a timely manner
4.  Provide admin-level access to the source email system OR a list of
    users with individual passwords
5.  Perform changes to internal and external DNS, as required
6.  Assist with identification of high-risk users (top executives
    and VIP users, users with 50 GB mailboxes or larger and/or
    30 GB deleted folders or larger)
7.  Ensure IMAP Access is enabled for all users

### Additional cost items not provided by the project

1.  Informing users about the migration
2.  Customer team training (could be added as an additional service)
3.  Migration of Corporate documents to SharePoint Online (could be
    added as an additional service)
4.  Desktop software settings
5.  Migration of anything except email and email folders

Upon completion of the project, we will provide a project closeout
report. This document will indicate the final project status,
including acceptance criteria matching, outstanding issues (if any), and the
final budget. If you require more extensive documentation, it can be
provided for an additional fee.  

Our migration solution has been proven through numerous implementations
to provide high user satisfaction with Office 365 after switching from G
Suite.

### Prerequisites

1.  You must have an Office 365 tenant with Exchange Online licenses
2.  You must have access to your email domain DNS zone
3.  You must have admin access to G Suite
4.  The Source must be a paid version of Google Drive. Free Google Drive
    accounts are not supported

**Here are some limitations to be aware of**:

1.  We can only migrate items in a user inbox or other mail folders.
    This type of migration does not include contact, calendar item, or
    task migration.
2.  We can migrate a maximum of 500,000 items from a user mailbox
    (emails are migrated from newest to oldest)
3.  The biggest email we can migrate is 35 MB
4.  Regular, non-paid Google apps or Gmail accounts do not have
    administrative credentials. We will need to migrate these accounts
    using the individual user names and passwords for each account.
    Without admin credentials, your account may be temporarily locked by
    Google.
5.  Google does not have a folder hierarchy for email, but a virtual
    view called Google Labels. Google Labels cannot be transferred
    properly to other messaging systems. Messages are stored as a single
    instance within the Google mail store, although they may appear
    under several labels within the web interface. When an IMAP
    client, such as Outlook or your mobile device, is connected to
    Google, the labels appear as folders, and the email with several
    labels will be downloaded several times, taking up additional
    storage space

### Plan

The plan may vary depending on your needs.

1.  Kickoff meeting
2.  Pre-migration source system health check
3.  User creation or AD connect tool configuration
4.  Email and data migration start
5.  Migration process verification
6.  MX record to a new Office 365 tenant 
7.  Final email and data migration
8.  Verification and fixing issues

### Results

1.  Users can access Exchange Online on their desktop PCs, mobile phones,
    and tablets from any place, any time 
2.  All emails are successfully migrated to Office 365 tenant and are accessible
    by all user profiles
3.  All necessary Transport rules are created and working 
4.  Mail can be sent and received using Exchange Online 
5.  Exchange Online Protection configured and working 
