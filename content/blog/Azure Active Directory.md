+++
title = "Azure Active Directory"
description = "Microsoft offers a great choice of cloud-based identity and access management solutions on Azure Active Directory to help organizations monitor applications within their data centers and public cloud platforms. With the help of advanced features of AAD, one can easily control suspicious activity, reduce risk, and protect data. "
date = 2019-07-01

[taxonomies]
tags = ["azure", "azure ad", "security"]
+++

Azure AD Connect combines on-premises directories with Azure Active
Directory. Consolidated with Azure, Office 365, and SaaS app, it helps users 
be more efficient by providing them with opportunities to
use cloud and on-premises resources.\
Azure AD maintains SSO authentication and guarantees safe
access control to applications by letting the users sign in only once
with a single user account.

Azure AD offers three options for SSO authentication:

-   SAML-based Sign-on (sign in to a SaaS app automatically by
    processing the data in the user account from Azure AD)
-   Password SSO (sign in automatically to the third-party
    application by using a certain set of credentials)
-   Linked SSO (sign on to the app with the help of Active
    Directory Federation Services (ADFS) or a different
    third-party single sign-on provider)

![](https://o365hq.com/images/426.png)

![](https://o365hq.com/images/423.png)

### Azure AD SSO (federated) with Salesforce

For example, the Salesforce app can be added to Azure AD from the Azure
AD Application Gallery. Configuring Salesforce with federated
SSO makes it simple to access. After the app is configured
to perform service provider-initiated single sign-on, and the admin has
uploaded the certificate and configured the Salesforce authentication
provider, users can find their accounts in Salesforce automatically by
using account provisioning -- another feature supported by Azure AD.

![](https://o365hq.com/images/424.png)

The admin can set up SSO Integration by assigning the Sales and
Marketing security group access to Salesforce.

After that, the users will be able to access Salesforce via the
*Application Panel* as soon as they are granted access by the
administrator.

The *Applications Access Panel* is a cross-browser portal that
maintains iOS, Android, Mac, and Windows. When reaching the Access
Panel, the users can view or access any of the applications listed in
the MyApps portal. There is no need to re-authenticate if it was
configured for SSO by the administrator.

![](https://o365hq.com/images/427.png)

![](https://o365hq.com/images/425.png)

### Bring Your Own Apps

The Azure AD application gallery offers a wide range of applications
for companies. Even if a certain third-party app cannot be found
there, it can easily be added as a custom app. Once a new app has been
added, the admin can assign single sign-on. Now there is no need to
authenticate (e.g., type a password) a second time. With the help of this
function, the users are automatically signed in to the third-party SaaS
application. After the admin assigns the users and security group
access to the app, all members will be able to view and edit sign-in
field labels.

![](https://o365hq.com/images/428.png)

![](https://o365hq.com/images/429.png)

![](https://o365hq.com/images/430.png)

### Cross-Organization Collaboration

Azure Active Directory B2B collaboration enables partners to selectively
access corporate applications and data using self-managed identities.

Azure AD supports adding four types of users:

-   New user in an organization
-   User with an existing Microsoft account
-   User in another Microsoft Azure AD directory
-   Users in a partner company

Due to the Azure AD B2B capacities, partners may be invited right to the
company's directory, which allows them to have access only to the data
they need. If the new members are not yet part of such a directory, they
can simply join it via an automated email. After that, partners are
added to the security group and can use the same apps and resources as
other members of this group. Access by external users, as well as
corporate users, to corporate applications can be gated by the 
conditional access policies.

![](https://o365hq.com/images/431.png)

![](https://o365hq.com/images/432.png)

![](https://o365hq.com/images/433.png)

### Advanced User Lifecycle Management

Azure AD allows admins to easily add and manage users and groups and
enables dynamic group membership. The user account is created by
synchronizing with an on-premises AD in case the source is *local Active
Directory*. If the source is Azure Active Directory, Azure creates it in
the cloud. It is obligatory to have an account for everyone who will
use a Microsoft online service. The most basic role is *User*. An
administrator must first specify each user's location (by country) and
then product licenses can easily be granted based on subscriptions
already purchased by the organization.

Using groups to assign the app multiple users is essential in case a lot
of users access the same app. Groups may be used to configure access
management of other online services that monitor access to resources
(e.g., SharePoint Online).

The distribution groups and mail-enabled security groups are created and
managed within the Exchange Admin Center if the organization uses Office
365. Office 365 is the source for such groups and they must be managed
in Office 365. Dynamic groups can automatically add and remove users
from groups. Any user that meets the membership requirements will
automatically gain access to appropriate resources and privileges.

![](https://o365hq.com/images/434.png)

![](https://o365hq.com/images/435.png)

### Ease of Use for End Users

Azure AD offers an organization familiar applications that are well-integrated for
quick productivity. The Access Panel is used here as a one-stop shop to
share applications and data through Azure AD. If Multi-factor
Authentication is used as an added security measure to verify the user,
the user is required to verify their alternate contact info only first time. 
Once set up, their phone or authenticator app will
alert them to react to the [MFA]{.caps} challenge. If the user is
licensed to Office 365 apps, those will be displayed on their Access Panel.
Office 365 and Azure Active Directory integration allows a company to
place apps assigned to the user on the launcher in Office 365.

![](https://o365hq.com/images/436.png)

![](https://o365hq.com/images/438.png)

### Low IT Overhead

Azure AD Premium empowers IT productivity in a company by providing it
with self-service for password reset, group, and app management
capacities.

Self-service password reset has several benefits:

-   Reduced costs
-   Improved user experiences
-   Lower help desk volumes
-   Enabled mobility

Self-service is a very effective cost-cutting method that reduces help
desk calls because the user no longer depends on the IT help desk or an
administrator and can perform self-service on their Azure AD account on
their own.

![](https://o365hq.com/images/437.png)
