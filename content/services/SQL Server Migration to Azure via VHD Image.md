+++
title = "SQL Server Migration to Azure via VHD Image"
description = "Moving your SQL Server database to an Azure Virtual Machine via VHD image."
date = 2018-06-27

[taxonomies]
products = ["Microsoft Azure"]
types = ["Migration"]

[extra]
sku = "ITPWW300MIGOT"
price = "$450"
duration = "1 week"
manager = "Mike Mackey"
+++

An Azure Virtual Machine is a simple tool to host all supported editions
and versions of SQL Server, including SQL Server 2016,
on virtual machines. You can run your enterprise database applications
on high-end VMs in the cloud with the flexibility of either paying per
usage or reusing existing SQL Server licenses. Also, you may
use free-licensed SQL Developer and Express editions for
testing and lightweight workloads.

Please note that if you need a server upgrade, we can provide it as an
additional service.

Our **objective** is to migrate your SQL Server to an Azure VM.

This project will be considered **successful** when SQL
databases are available from an Azure VM without data loss.

### IT Partner responsibilities

-   Convert physical or virtual machines to Hyper-V VHDs by
    using Microsoft Virtual Machine Converter
-   Upload VHD files to Azure Storage by using the Add-AzureVHD
    cmdlet
-   Create a SQL VM with per-minute licensing or an existing
    license (please note, it is not possible to change the licensing
    model of a pay-per-minute SQL Server VM to using your own
    license. In this case, you must create a new BYOL VM and
    migrate your databases to the new VM.)
-   Deploy a new virtual machine by using the uploaded VHD
-   Configure high availability, if required

Also, if you have to transfer large amounts of data, we will help you
arrange to ship your hard drive(s) using the Azure Import/Export
Service, when uploading over the network is prohibitively expensive or
not feasible.

### Client responsibilities

-   Provide a dedicated point of contact responsible for working with IT
    Partner and coordinate any outside vendor resources and schedules
-   Configure all networking equipment, such as load balancers, routers,
    firewalls, and switches
-   Provide access to physical and virtual servers and/or systems and
    services, as needed. Provide remote and/or physical access to
    facility and systems required to complete work

### Outside the scope of this project (additional cost items)

-   Backup scheduling
-   Software version upgrade

Upon completion of the project, we will provide a *project closeout
report*. This document will indicate the final project status, including
evidence of meeting acceptance criteria, any outstanding issues, and the
final budget. If you require more extensive documentation, this can be
provided for an additional fee.

### Plan

The plan may vary depending on your needs.

1.  Kickoff meeting
2.  Review SQL Server and Windows Server
3.  Start deployment
4.  Finalize deployment
5.  Verify and fix issues, if any
