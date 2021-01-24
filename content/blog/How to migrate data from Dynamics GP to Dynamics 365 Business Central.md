+++
title = "How to migrate data from Dynamics GP to Dynamics 365 Business Central"
description = "Business Central is an Enterprise Resource Planning solution from Microsoft that appeared last year but has already gained popularity – it is a user friendly, all-in-one business management product for a very reasonable price. "
date = 2019-02-25

[taxonomies]
tags = ["dynamics365", "howto"]
+++

Business Central (BC) comes with Essentials and Premium editions -- the latter intended for
producers and service providers, as it contains feature-packed modules
for manufacturing (with inventory planning and MRP) and service
management. Apart from these modules, the Essentials package contains
nearly everything you could think of and is totally sufficient for the majority
of companies.

BC comprises financials, sales, services and operations, project
accounting, and HR; it streamlines processes and provides AI insights for
smarter decision-making. On top of this -- it is integrated with Office
365. Now your data from BC can travel to Office apps and back with no
boundaries -- this is a fantastic experience.

Business Central is a real treasure chest for every business, with
immense options for customization and personalization. But if you have
Dynamics GP deployed and haven't decided on Business Central yet, you
can still give BC a whirl by synchronizing your on-prem Dynamics GP with
Dynamics 365 Business Central. This will allow you to stay on-prem, but
at the same time enjoy insights from cloud AI for better planning and
decision-making.

If you have found that the cloud is your perfect match and you are ready to
make the move -- both literally and figuratively -- keep reading. We will 
discuss how to migrate your data from on-prem Dynamics GP
to Business Central in a few easy-to-follow steps and make this SaaS
your primary solution.

### Which GP versions can be migrated?

![](https://o365hq.com/images/224.png)

Pic. 1

Only a supported version of Dynamics GP (released in 2015, 2016, 2018)
with the latest build deployed can be migrated (Pic. 1). The reason for
this is that only the above-mentioned versions have additional code
units that allow data to be exported from GP into a separate zip file
compatible with the migration tool. To create this file, go under the File menu
in your GP, choose *Maintenance* and then *Export data* (Pic. 2).

![](https://o365hq.com/images/226.png)

Pic. 2

Once you save your zip folder containing .txt files with data and
settings (Pic. 3), you can start the migration -- it's as simple as that.

![](https://o365hq.com/images/223.png)

Pic. 3

### What data can be migrated?

Migration is a one-time data move. Once you migrate, BC SaaS will
become your primary solution and your existing Dynamics GP system will
only be used to search across your historical GP data or for reporting
purposes (if you use a connector to a reporting tool). As moving from
on-prem finance solutions becomes more commonplace, Microsoft is
developing extensions that make the migration process a walk in
the park. Dynamics GP Data Migration Extension is available for free at
[Appsource](https://appsource.microsoft.com/en-us/product/dynamics-365-business-central/PUBID.microsoftdynsmb%7CAID.5a417920-451b-4a16-8f08-2b25862fef8e%7CPAPPID.936d57e3-05fe-4aff-8459-35aa9367abec?tab=Overview)
. Thanks to this extension, you can migrate the following modules:

![](https://o365hq.com/images/222.png)

Now you may ask an obvious question -- why can't we migrate all our GP
data? The reason is that Dynamics 365 BC is a totally different product,
and some modules in it, like *Fixed Assets* or *No. series* work
differently (compared to on-prem GP) or don't exist at all, like, for example,
*Payroll.*

At the moment, only the above-mentioned data can be migrated with the
help of the GP extension, but Microsoft is planning to add the ability to
migrate historical data for Sales, Purchasing, and Inventory too. There
is also a *Rapid Start Services* toolkit to migrate more data, and we
will come back to that a little bit later.

### Follow the Wizard to move to the cloud

When everything is ready for migration, you can start the process.
Under *Setup and Extensions* you will see *Assisted setup*. Click on
*Migrate business data*. On the "Data Migrators" page, you can select
from a number of options: to import from GP, QuickBooks, QuickBooks
Online, and Excel. At this point, you will be asked to choose the export
(zip) file, and the extension will group the information it contains in a
table for you to check to make sure everything was exported correctly before
the migration process starts (Pic. 4). As you continue, the migration tool
picks up your data, pushes it up into BC tenant, and maps it to the
tables within the BC application.

![](https://o365hq.com/images/225.png)

Pic. 4

During migration, you can see an overview of the progress (Pic.5).

![](https://o365hq.com/images/227.png)

Pic. 5

If an error occurs, there may be two scenarios -- if a not-required field
contains an error (like an absent @ symbol in an email address), the record
will still be migrated, and you will be able to correct the error after
migration. If the error is in a required field, the record won't migrate.
The overview of migration will help you to keep track of that (Pic. 5).

### What will happen to your data after migration?

**Accounts**

When GP extension was first released, it only offered the option of
bringing over your existing Chart of Accounts and the Balance Sheet at
the time of migration, so only a Summary value was brought across to BC.
The reason is that the *GL chart of accounts* in Dynamics GP and
Business Central are distinguished by their structure. There is only one
Account number in BC tenant; therefore, the GP account main segment will
become the account number in BC once you migrate. The other segments
will come as dimensions. Transaction amounts are not distributed across
those dimensions, but all the amounts are summed in the main segment of
that particular account (Pic. 6).

![](https://o365hq.com/images/231.png)

Pic. 6

Since the 2018 fall release, you have a new option of bringing a brand-new
Chart of Accounts with new account numbers. To do this, choose the "Create a
New Chart of Accounts" option during the setup process (Pic. 7).

![](https://o365hq.com/images/228.png)

Pic. 7

Then you will be given the option to download an Excel file (Pic. 8) where you should
map each of your current accounts with a new unique account number. If
you leave some lines in the "New Account Number" column (Pic. 9) blank or
enter duplicates, the migration will fail.

![](https://o365hq.com/images/230.png)

Pic. 8

![](https://o365hq.com/images/235.png)

Pic. 9

After your Excel table is ready, you can import it back to Wizard
(Pic. 8) and all your accounts will change their numbers according to the
Excel table lines. Not only the numbers, but also new account summary
information will change -- it will be available for a fiscal period of the
current year and the year before (Pic. 10) (fiscal periods are determined
according to GP settings).

![](https://o365hq.com/images/232.png)

Pic. 10

When you click on the *Net change*, you will see the summary info for
the last two years (Pic. 11).

![](https://o365hq.com/images/229.png)

It will be the same summary as in GP for the corresponding fiscal years
(Pic. 12).

![](https://o365hq.com/images/234.png)

Pic. 12

Another new option available since fall 2018 is the ability to post
transactions automatically or leave them unposted, meaning you can post
them manually once the migration process is over. You can automatically
update the General Journal or, if you want to make sure everything
migrated correctly, you can leave it unposted, which would give you the
ability to look at all the transactions and their batches and then post
them manually, in case you want to make any changes before that process
completes.

**Customers/Vendors**

Previously, only summary transactions for Customer/Vendor balance could be
migrated.

Now, detailed open transactions are brought across too. For example, if
you have 10 invoices, 1 credit memo, and 3 open payments, all of those
documents will come across as individual transactions. Instead of
bringing the original transaction amount, the amount remaining on the
transactions is brought across. For example, if Adam Park Resort has
invoices for \$40,000, with an amount remaining \$20,800.09, the balance in
the customer ledger entry will be for \$20,800.09 (Pic. 13). The same
applies to Vendors -- only the outstanding amount on the transactions will
migrate.

![](https://o365hq.com/images/233.png)

Pic.13

You can drill into that total amount and see what transactions it
consists of (Pic.14).

![](https://o365hq.com/images/236.png)

Pic. 14

**Items**

Your inventory items will be imported according to the cost valuation
chosen when you set up a company in BC. The first in/first out evaluation
method is automatically applied to service items. For now, the
quantities on hand are migrated into the blank site; after migration, you
can transfer those to the corresponding locations manually (Pic. 15). It
is also one of the enhancements around the migration tool that Microsoft
is planning to make in future releases.

![](https://o365hq.com/images/237.png)

Pic. 15

Apart from this data, certain setup information is migrated. *Posting
groups* are brought across based on *Posting Setup* in GP, as well as
*Payment method ID*, *Shipping Method ID*, and *Salesperson ID* (the
details in regard to those particular entities are not brought across;
only the IDs are transferred).

**Other migration tools**

Similar to Integration Manager and Rapid Start within the Dynamics GP
product, there is a Rapid Start Services toolkit within BC. If you need
to migrate more data to BC, contact your service provider and you will
be given configuration packages to export necessary data from your
former financial system and import it to BC.

**Excel Integration**

BC integration with Excel is a valuable tool, as most of
the tables within BC can be edited in Excel. It means you can export
your financial data from a list page to Excel, where it can be analyzed
using the extensive data analysis tools Excel provides. For example, let's
say you want to create a report from your customer ledger entries that
shows quarterly sales by customer. You start by searching Customer Ledger
Entries and then click the *Edit in Excel* button on the *Home* tab of the
ribbon to open this data in Excel. When the Workbook opens, the Microsoft
Dynamics Office Add-in opens, creating a connection to the data and
providing controls for working with the data connection, including the
ability to refresh the data to ensure that reports and charts you create
are always up to date. Using the application's powerful reporting and
charting functionality, you will create your report in a few minutes
(Pic. 16).

![](https://o365hq.com/images/238.png)

Pic.16

BC enables you to easily update records by modifying your data in Excel and
publishing the changes back to your database in BC. Let's assume you
want to update the "document sending profile" for all your customers.
This could take a while if you have to update the field one by one on
each customer card. However, you can speed this up by making the updates
to the list of data in Excel and publish it. Once the changes have been
published successfully, you can check the customer card to see if the
field has been updated correctly.

### Conclusion

As you can see, data migration from GP to BC is really easy thanks to the 
data migration tool, but its functions and the amounts of data you can
transfer are limited due to the core differences in the structure of
these products. However, Microsoft has announced that many enhancements are expected
soon, and if some of the business data is critical, you can use Rapid
Start tools to right the ship no matter what.\
Once you are done with migration, the coast is clear -- your data is in
the cloud, and the only thing remaining is to simply enjoy working in 
Business Central, reaching new heights in your business.
