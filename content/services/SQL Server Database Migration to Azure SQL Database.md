+++
title = "SQL Server Database Migration to Azure SQL Database"
description = "Moving your SQL Server database to Azure SQL Database"
date = 2018-06-27

[taxonomies]
products = ["Microsoft Azure"]
types = ["Migration"]

[extra]
sku = "ITPWW320MIGOT"
price = "$150 per hour"
duration = "1 week"
manager = "Mike Mackey"
+++

Please note that this service is relevant for migration to Azure
SQL Database. If you want to migrate a SQL Server
database to a SQL Server in an Azure VM, see our other service.

Our **objective** is to migrate SQL databases to the Azure
cloud.

This project will be considered **successful** when SQL
databases are available from Azure without data loss.

### IT Partner responsibilities

We have two possible scenarios for SQL migration. The first
method is simpler, but requires some possibly substantial downtime
during the migration. The second method is more complex, but
substantially eliminates downtime during the migration.

*Method 1: Migration with downtime during the migration*

-   Assess the database for compatibility using the latest version of
    Data Migration Assistant (DMA).
-   Prepare any necessary fixes as Transact-SQL scripts.
-   Make a transactionally consistent copy of the source database being
    migrated and ensure no further changes are being made to the source
    database (or you can manually apply any such changes after the
    migration is complete). There are many methods to quiesce a
    database, from disabling client connectivity to creating a database
    snapshot.
-   Deploy the Transact-SQL scripts to apply the fixes to the
    database copy.
-   Export the database copy to a .BACPAC file on a local drive.
-   Import the .BACPAC file as a new Azure SQL database using
    any of several BACPAC import tools, with
    SQLPackage.exe being the recommended tool for best
    performance.

*Method 2: Use transactional replication*

-   Remove your SQL Server database from production
-   SQL Server transactional replication as a migration solution
-   Configure Azure SQL Database as a subscriber to the
    SQL Server that you wish to migrate
-   Transactional replication; all changes to your data or schema show
    up in your Azure SQL Database
-   Migrate and change the connection string of your applications to
    point them to your Azure SQL Database

### Client responsibilities

-   Provide a dedicated point of contact responsible for working with IT
    Partner and coordinate any outside vendor resources and schedules
-   Configure all networking equipment, such as load balancers, routers,
    firewalls, and switches
-   Provide access to physical and virtual servers and/or systems and
    services, as needed. Provide remote and/or physical access to
    facility and systems required to complete work
-   Perform changes to internal and external DNS, as required

### Outside the scope of this project (additional cost items)

Upon completion of the project, we will provide a *project closeout
report*. This document will indicate the final project status, including
evidence of meeting acceptance criteria, any outstanding issues, and the
final budget. If you require more extensive documentation, this can be
provided for an additional fee.

### Prerequisites

You must have an Azure subscription.

### Plan

The plan may vary depending on your needs.

1.  Kickoff meeting
2.  Define backup points and policy
3.  Start deployment
4.  Finalize deployment
5.  Verify and fix issues, if any
