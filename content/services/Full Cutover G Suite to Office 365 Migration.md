+++
title = "Full Cutover G Suite to Office 365 Migration"
description = "G Suite (Google Apps) migration to Office 365. We will move all your mailboxes with calendars, tasks, contacts, and other information to Exchange Online. Files and documents from Google Drive to OneDrive for Business will also be migrated. "
date = 2018-02-01

[taxonomies]
products = ["Exchange Online"]
types = ["Migration"]

[extra]
sku = "ITPWW140MIGOT"
price = "$300 + $25 per mailbox"
duration = "1 week"
manager = "Mike Mackey"
+++

*Note that if you only need mailbox migration, you should
order IMAP migration from G Suite to Office 365.*

This migration occurs with the help of a special utility that allows us to
move any amount of mail data, calendars, and other information in the
shortest time, avoiding possible errors during manual data transfer.

Our objective is to provide a plan and design a way to migrate to Office
365, including email, contacts, calendars, tasks, files, and data. The
project will be considered successful when all user data is fully
migrated from Gmail and Google Drive to the Office 365 tenant.

### IT Partner responsibilities

1.  Gather information and verify the original G Suite
2.  Configure the destination Office 365 tenant
3.  Create and configure users
4.  License assignment
5.  Create and configure a migration plan
6.  Provide informational messages for users
7.  Start and control the data migration process
8.  Provide a OneDrive (SharePoint) profile for each user being migrated

### Client responsibilities

1.  Coordinate Client resources and staff schedules
2.  Provide a dedicated point of contact responsible for working with IT
    Partner and coordinate any outside vendor resources and schedules as needed
3.  Review and approve engagement deliverables in a timely manner
4.  Configure all network equipment, such as load balancers, routers,
    firewalls, and switches
5.  Perform changes to internal and external DNS, as required
6.  Assist with identification of high-risk users (top executives
    and VIP users, users with 50 GB mailboxes or larger and/or
    30 GB deleted folders or larger)
7.  Ensure IMAP Access is enabled for all users
8.  Ensure contact and calendar services are turned on for all users
9.  Users should not modify any documents in their Google Drive accounts
    during the migration, because any modifications will not be included
    in the migration
10. End user support

### Additional cost items not provided by the project

1.  Customer team training (could be added as an additional service)
2.  Corporate documents migration to SharePoint Online (could be added
    as an additional service)
3.  Desktop software settings

**Here are some limitations to be aware of**

1.  SharePoint Online and OneDrive for Business have a limitation in
    file path length and file names. These limitations may cause issues
    during the migration from Google Drive. We may implement automatic
    solutions that can minimize such issues, but preparation is still an
    important part of the process
2.  The actual maximum  file path length within OneDrive for Business
    is 260 characters. However, library names and usernames are
    included in that limit, so the actual file path could be much
    smaller than 260 characters long. Also, certain characters need to
    be encoded and will reduce the available size even more
3.  File/folder name extension limitation
4.  There is a list of file extensions that are not allowed to be
    created inside of SharePoint Online and OneDrive for Business

Upon completion of the project, we will provide a project closeout
report. This document will indicate the final project status,
including acceptance criteria matching, outstanding issues (if any), and the
final budget. If you require more extensive documentation, it can be
provided for an additional fee.  

This service offers a simple, secure, and cost-effective way to migrate
to Office 365, including email, contacts, calendars, tasks, files, and
data.

### Prerequisites

1.  You must have an Office 365 tenant with Exchange Online licenses
2.  You must have access to your email domain DNS zone
3.  You must have admin access to G Suite
4.  The source must be a paid version of Google Drive; free Google Drive
    accounts are not supported
5.  The destination must be OneDrive for Business, not a personal
    OneDrive version
6.  Each user in the destination environment must be assigned to a
     [SKU]{.caps} license that contains OneDrive for Business

### Plan

The plan may vary depending on your needs.

1.  Kickoff meeting
2.  Pre-migration source system health check
3.  User creation or AD connect tool configuration
4.  Email and data migration start
5.  Migration process verification
6.  MX record to a new Office 365 tenant 
7.  Final email and data migration
8.  Verification and fixing of issues, if any

### Success criteria

1.  Users can access Exchange Online on their desktop PCs, mobile phones,
    and tablets from any place, any time 
2.  G Suite data is successfully migrated to Office 365 tenant and
    is accessible by all user profiles
3.  All necessary transport rules are created and working 
4.  Mail can be sent and received using Exchange Online 
5.  Exchange Online Protection is configured and working 
