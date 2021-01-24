+++
title = "Azure AD Tenant-to-Tenant Staged Transition"
description = "Azure Active Directory migration from one Office 365 tenant to another. Usually, you will need this type of migration when a company merges or acquires another company, or you would like to migrate to a different geographic region."
date = 2019-07-10

[taxonomies]
products = ["Microsoft Azure"]
types = ["Migration"]

[extra]
sku = "ITPWW430MIGOT"
price = "$1300 + $2 per user"
duration = ""
manager = "Roman Sotnik"
+++

This service will allow you to transfer Azure AD data from one tenant to
another. We can move users and groups, saving all current logins. Please
note that export of passwords from Azure AD is impossible, so saving the
current user passwords will not work. The users will be assigned a
temporary password they can use to create a permanent password of their own.

Staged Azure AD Tenant-to-Tenant migration describes the staged
migration of users and Azure resource sharing setup. This scenario will
suit you if your company has many users who use Azure AD authorization
on their workstations, or for a large number of other resources hosted
in Azure.\
Staged migration allows a number of users to log into the new domain, but
with the help of the access settings, it is also possible to save the
ability to work with resources, SharePoint, or VM in the old domain.
This approach allows reconfiguring of all PCs while saving data,
using less human resources and reducing possible downtime.

You can also consider a cut-over migration, during which all data will be
transferred at once.

### IT Partner responsibilities

1.  Source tenant data analysis
2.  Preparation of the migration plan, including resource list, migrated
    user groups, and their access to data in the source tenant
3.  Providing informational messages for users
4.  Staged export of data from the source tenant in accordance with the
    migration plan and uploading data into a new tenant
5.  Providing users of the new tenant with access to resources in the
    source tenant
6.  Consultation on technical issues related to the work of Azure AD

### Client responsibilities

1.  Coordinate Client resources and staff schedules
2.  Provide a dedicated point of contact responsible for working with IT
    Partner
3.  Coordinate any outside vendor resources and schedules
4.  Provide administrative access to source and destination tenant
5.  Change settings of applications using Azure AD, if any
6.  Notify users about changes
7.  Change PC settings if Azure AD authorization is used
8.  Review and approve engagement deliverables in a timely manner

### Additional cost items not provided by the project

1.  Migration of other data from Azure, such as applications, mail,
    virtual machines, and databases (can be purchased as an additional
    service)
2.  Resource sharing setup between the source tenant and the destination
    tenant
3.  Workstation configuration. Please note that if employees use Azure
    AD authorization on their PCs, they will need to disconnect from the
    current tenant and connect to a new one; a new user profile will be
    created as a result. Services for PC setup and transferring data
    stored in a user profile can be purchased as an additional service

Upon completion of the project, we will provide a project closeout
report. This document will indicate the final project status, including
acceptance criteria matching, outstanding issues, and the final budget.
If you require more extensive documentation, it can be provided for an
additional fee.

### Prerequisites

1.  You have administrative access to the source tenant
2.  You have administrative access to the destination tenant and
    licenses similar to the source tenant, or you are ready to purchase
    them

### Plan

The plan may vary depending on your needs.

1.  Kickoff meeting
2.  Source tenant data analysis
3.  Preparation and coordination of the migration plan
4.  Preparing for migration and informing users
5.  Data migration according to the developed plan
6.  Verification and fixing issues

### Success Criteria

1.  All users and groups are migrated from the source tenant to the
    destination tenant without data loss
2.  It is possible to authorize all users in the new domain
