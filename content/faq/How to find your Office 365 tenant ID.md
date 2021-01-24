+++
title = "How to find your Office 365 tenant ID"
description = ""
date = 2018-07-04

[taxonomies]
tags = ["office 365 tenant"]
+++

Your Office 365 tenant ID is a globally unique identifier
(GUID) that is different than your tenant name or domain. On
rare occasions, you might need this identifier, such as when configuring
Windows group policy for OneDrive for Business.

If you do need to find your Office 365 tenant ID, it's pretty easy.
Choose one of the following procedures.

Use the Azure AD portal
-----------------------

Office 365 uses Azure AD to manage user accounts. You can find your
tenant ID in the Azure AD portal. You'll need to be an Azure AD
administrator.

### To find your Office 365 tenant ID in the Azure AD portal

1.  Log in to Microsoft Azure as an administrator.
2.  In the Microsoft Azure portal, click **Azure Active Directory**.
3.  Under **Manage**, click **Properties**. The tenant ID is shown in
    the **Directory ID** box.

Use Windows PowerShell
----------------------

You can use Windows PowerShell to find the tenant ID. You'll need the
[Microsoft Azure PowerShell
module](https://go.microsoft.com/fwlink/p/?LinkId=717444).

Open a Microsoft Azure PowerShell command window and run the following
script, entering your Office 365 credentials when prompted.

`Login-AzureRmAccount`

Your tenant ID is listed in the output.

### For more information about Office 365 tenants, check these articles:

-   [Office 365 tenant -- what is
    it?](https://o365hq.com/faq/what-is-office-365-or-azure-ad-tenant)
-   [How to find your Office 365 tenant
    name](https://o365hq.com/faq/how-to-find-your-office-365-tenant-name)

### Let us help you with your Office 365 migration project

Complete this [Pre-migration
Questionnaire](https://office365.typeform.com/to/TMQniV) and we will
reply with a quote. Or join hundreds of organizations that switched
their Office 365 subscriptions from Microsoft to us to enjoy 24/7
professional support, better terms, and free consulting and
implementation hours. Contact sales\@o365hq.com.
