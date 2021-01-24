+++
title = "Azure AD Tenant-to-Tenant Basic Transition"
description = "Azure Active Directory migration from one Office 365 tenant to another. Usually, you will need this type of migration when a company merges or acquires another company, or you would like to migrate to a different geographic region."
date = 2019-07-10

[taxonomies]
products = ["Microsoft Azure"]
types = ["Migration"]

[extra]
sku = "ITPWW420MIGOT"
price = "1300"
duration = "5"
manager = "Roman Sotnik"
+++

Azure AD Tenant-to-Tenant migration will allow you to transfer Azure AD
data from one tenant to another. We can move users and groups, saving
all current logins. Please note that export of passwords from Azure AD
is impossible, so saving the current user passwords will not work. The
users will be assigned a temporary password they can enter in
the new tenant and create their own permanent password.

This service involves a cut-over migration, during which all data will
be exported from the source tenant and uploaded to a new one.
After that, all employees will need to reconfigure their devices if they
are using Azure AD authorization. It is also necessary to configure
applications and other services that use Azure AD. This option is
suitable for companies with a small number of employees and resources in
Azure.

You may also want to consider the staged data migration, which will allow
employees to use resources in one tenant and passing authorization in
another.

### IT Partner responsibilities

1.  Source tenant data analysis
2.  Providing informational messages for users
3.  Export of data from the source tenant
4.  Uploading data to a destination tenant
5.  Consultation on technical issues related to the work of Azure AD

### Client responsibilities

1.  Coordinate Client resources and staff schedules
2.  Provide a dedicated point of contact responsible for working with IT
    Partner
3.  Coordinate any outside vendor resources and schedules
4.  Provide administrative access to source and destination tenants
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
    stored in a user profile can be purchased as an additional service.

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
3.  Preparing for migration and informing users
4.  Exporting data from the source tenant and uploading data to a
    destination tenant
5.  Verification and fixing issues

### Success Criteria

1.  All users and groups are migrated from the source tenant to the
    destination tenant without data loss
2.  It is possible to authorize all users in the new domain
