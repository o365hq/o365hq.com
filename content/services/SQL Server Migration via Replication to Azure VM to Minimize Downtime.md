+++
title = "SQL Server Migration via Replication to Azure VM to Minimize Downtime"
description = "SQL Server migration through transactional replication to configure the Azure VM SQL Server as a subscriber and then disable replication, pointing users to the Azure database. "
date = 2018-06-27

[taxonomies]
products = ["Microsoft Azure"]
types = ["Migration"]

[extra]
sku = "ITPWW310MIGOT"
price = "$800"
duration = "1 week"
manager = "Mike Mackey"
+++

Transactional replication is typically used in server-to-server
environments. This service is relevant when you need to minimize
downtime and do not have an AlwaysOn on-premises deployment.

Our **objective** is to migrate a SQL Server to an Azure VM
with minimal downtime.

This project will be considered **successful** when SQL
databases are available from Azure without data loss.

### IT Partner responsibilities

-   Implement SQL Server Snapshot Agent, Log Reader Agent, and
    Distribution Agent
-   Prepare snapshot files containing schema and data of published
    tables and database objects
-   Synchronize jobs in the distribution database on the Distributor
-   Make incremental changes at the Publisher flow to Subscribers
    according to the schedule of the Distribution Agent, which can run
    continuously for minimal latency or at scheduled intervals

### Client responsibilities

-   Provide a dedicated point of contact responsible for working with IT
    Partner and coordinate any outside vendor resources and schedules
-   Configure all networking equipment, such as load balancers, routers,
    firewalls, and switches
-   Provide access to physical and virtual servers and/or systems and
    services, as needed. Provide remote and/or physical access to
    facility and systems required to complete work.

Upon completion of the project, we will provide a *project closeout
report*. This document will indicate the final project status including
evidence of meeting acceptance criteria, outstanding issues and the
final budget. If you require more extensive documentation, this can be
provided for an additional fee.

### Plan

The plan may vary depending on your needs.

1.  Kickoff meeting
2.  Review SQL Server and Windows Server
3.  Start deployment
4.  Finalize deployment
5.  Verify and fix issues, if any
