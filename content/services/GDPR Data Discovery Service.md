+++
title = "GDPR Data Discovery Service"
description = "The General Data Protection Regulation (GDPR) is the law of the European Union on the protection of natural persons with regard to the processing of personal data and on the free movement of such data. Our offer is a multi-step process that can be used to discover and scan data sources within the organization for personal data. The outcome of the discovery process will be a detailed inventory of data sources, together with the data they contain. Additionally, it will provide insights into how much of the data contains personally identifiable information (PII), or sensitive personal information that might be subject to the GDPR. "
date = 2019-04-23

[taxonomies]
products = ["Office 365"]
types = ["Training"]

[extra]
sku = "ITPWW190TRNOT"
price = "$15,000"
duration = "2 - 6 weeks"
manager = "Mike Mackey"
+++

Please note, GDPR Discovery Toolkit is NOT a tool to
certify compliance. It is the distributed responsibility of the customer
and their legal and compliance teams to certify their own GDPR
compliance.

Our **objective** is to identify and create an inventory of personal
data relevant to the GDPR. Also, we want to guide customers to
appropriate solutions that will help them elevate their GDPR
maturity and work toward GDPR compliance.

The project will be considered **successful** when you have answers
to questions like:

-   How much data do I have?
-   Where is my data?
-   Which data is impacted by the GDPR? (For example, if it
    contains PII - Personal Identifiable Information)

### IT Partner responsibilities

-   Identify what personal data you have and where it resides
-   Report how personal data is used and accessed
-   Recommend how to establish security controls to prevent, detect, and
    respond to vulnerabilities and data breaches
-   Advise how to keep required documentation and manage data requests and
    breach notifications

### Client responsibilities

-   Provide access to data locations (non-supported locations in
    OneDrive Personal), Databases (SQL Server, SQL
    online, Access, other), Local storage (workstation, laptop, tablet,
    mobile phone), Removable devices (USB drives, mobile hard
    disks), Backup media/3rd-party applications 
    (Non-Microsoft cloud solutions)
-   Resource and activity planning
-   Establish and confirm timelines
-   Readiness to implement Microsoft Information Protection

### Plan

![](https://o365hq.com/images/320.png)

#### Kick-off meeting

During this meeting, the team members will be introduced and the team
will be briefed on the upcoming activities, proposed timelines, and
expected outcome. We will explain the technical details of the scanning
process, how it works, and what it scans for. Important topics to discuss
include, but are not limited to, the scope of the discovery process, the
required prerequisites, and the expected outcome.

#### Step 1 -- Identify and assess

The first activity is to identify all possible data sources across the
organization. The data sources that are discovered will be documented in
a catalog that will be used as input for the next steps. For every data
source, the exact location and access type will be recorded, together
with information about the type of data and its owner.

#### Step 2 -- Plan for automated classification and labeling

Now that we have identified all possible data sources, the next step
towards GDPR compliance will be to assess whether the
GDPR will apply to the organization, and if so, to what
extent. Microsoft offers two solutions for automated data discovery and
classification: Microsoft Information Protection (MIP) and
Microsoft Advanced Data Governance (ADG). For both solutions,
the automated classification of documents will rely on the configuration
of policies, labels, and conditions.

As a result, we will:

-   Translate legal and business requirements into a finalized
    classification scheme that defines policies, labels, and conditions.
-   Document the classification scheme for further processing in
    consecutive steps.

#### Step 3 -- Select the right solution

Microsoft currently offers two solutions for data
governance: Microsoft Information Protection and Microsoft Advanced Data
Governance. Although both support data classification, (automated)
labeling based on sensitive data types, and a wealth of other data
protection and security features, each solution has its own specific
deployment scenarios and at the time of this writing, the two solutions are not
(fully) integrated yet.

#### Step 4 (on-premises) -- Implement Microsoft Information Protection

The MIP scanner service will be installed on an on-premises
domain joined member server and relies on the cloud-based Microsoft
Information Protection service for policy and labeling information. This
type of operation requires an integrated deployment in which both the
on-premises Active Directory and the Azure Active Directory are
synchronized.

#### Step 5 (on-premises) -- Scan existing data sources

Microsoft Information Protection (MIP) Scanner lets you
discover, classify, and protect files on the following data stores:

-   Local folders on the Windows Server computer that runs the scanner
-   Network shares (through UNC paths) that use the Common
    Internet File System (CIFS) protocol
-   Sites and libraries for SharePoint Server 2016 and SharePoint
    Server 2013

#### Step 4 (online) -- Prepare for Search and Discovery

Recognition of Personal Identifiable Information (PII) in
Office 365 data sources relies on automated data classification through
recognition of sensitive data types. The data classification process can
be automated in a way that existing data is scanned and labeled
automatically, and new data is classified upon creation.

Office 365 Labels and Advanced Data Governance (ADG) will be
used for data classification and labeling. Classification can be done
automatically or by enabling the user to apply a label to content
manually. Once labeled and classified, the data can then be protected by
additional means or searched for the presence of specific words or data
types.

#### Step 5 (online) -- Search and Discovery in Office 365

We will use the Content Search feature in the Office 365 Security &
Compliance Center to create the inventory. Content Search allows you to
search all content locations in your Office 365 organization. This
includes all mailboxes (including inactive mailboxes, and the mailboxes
for all Office 365 Groups and Microsoft Teams), all SharePoint and
OneDrive for Business sites (which includes the sites for all Office 365
groups and Microsoft Teams), and all public folders.

### Results

-   Data source inventory. You'll be able to identify and document
    the data sources within the organization online and on-premises
-   Classification and Labeling. This helps in facilitating the discussion with the
    legal, business, and IT teams
-   Defining a data classification taxonomy and label schema based on
    legal and business requirements
-   Reporting on data discovery
