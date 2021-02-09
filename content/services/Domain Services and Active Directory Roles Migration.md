+++
title = "Domain Services and Active Directory Roles Migration"
description = "This service allows you to transfer the typical functions of a domain controller, including DNS and DHCP, to a new server."
date = 2019-06-03

[taxonomies]
products = ["SCCM"]
types = ["Migration"]

[extra]
sku = "ITPWW390MIGOT"
price = "$900"
duration = "3 days"
manager = "Roman Sotnik"
+++

Domain services and active directory roles migration may be necessary if 
you are migrating from an SBS server to a new server, or from On-Premises 
solution to Office 365 and you want tokeep the Domain Controller in your 
network, but a new operating system or hardware is required.

### IT Partner responsibilities

1.  Domain Controller preparation and promotion
2.  Transfer of Domain Controller roles
3.  Transfer of group policy, groups, and users
4.  DNS server transfer
5.  DHCP server transfer

### Client responsibilities

1.  Coordinate Client resources and staff schedules
2.  Provide a dedicated point of contact responsible for working with IT
    Partner
3.  Coordinate any outside vendor resources and schedules
4.  Provide administrative access to the Active Directory domain and
    servers
5.  Configure all network equipment, such as load balancers, routers,
    firewalls, and switches
6.  Review and approve engagement deliverables in a timely manner

### Additional cost items not provided by the project

1.  Migration to Azure AD
2.  Email and/or documents transfer to Office 365
3.  Support of the devices with static network settings
4.  Remote installation of the Microsoft Windows OS on the server, if
    necessary, for example, when using a virtual machine or remote server
    management technologies -- iLO and others

### Prerequisites

1.  The operating system for the new DC is installed
2.  All devices are configured to use a DHCP server

### Plan

The plan may vary depending on your needs.

1.  Kickoff meeting
2.  The new server preparation
3.  Staged transfer of roles and data
4.  Verification of work
5.  Demotion of the old DC
6.  Verification and fixing issues, if any

### Success Criteria

1.  The new Domain Controller is available to users and can perform all
    necessary functions
2.  Users can log in to their PCs
3.  All GPO settings are saved
4.  The DHCP server is working and all its settings are saved
5.  The old DC is demoted and can be turned off
