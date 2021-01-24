+++
title = "What is Microsoft 365?"
description = "Customers are wrestling with the idea of providing a productive environment using the latest technology, while at the same time figuring out how to maintain this new technology and keep their data secure. The result is a patchwork of different solutions, complex integration, lost productivity, and systems with security flaws due to not having the most up-to-date software patches and releases. This is where Microsoft 365 Business comes into play. By providing productivity tools, built-in security, and simplified management in one package, Microsoft 365 Business addresses the business challenges customers face in the modern workplace."
date = 2018-07-27

[taxonomies]
tags = ["microsoft 365"]
+++

Cloud-based IDPs, like Azure Active Directory B2C (AAD
B2C), claim that they enable developers to add SSO,
MFA, secure storage for user data, and even integrate with
other IDPs without the need to write any code. Let's take a
closer look at AAD B2C and try to figure out how much effort
you will need to use it and whether it is the right solution for your
apps.

### What is Azure Active Directory B2C (AAD B2C)?

AAD B2C is a cloud identity provider service based on Azure
Active Directory and available in Microsoft Azure Cloud. AAD
B2C can be used to:

-   Enable customers to create user accounts, securely log into
    applications, reset passwords, and manage profiles
-   Enable customers to authenticate with social and/or corporate
    credentials (Facebook, Google, Twitter, ADFS, Active
    Directory, Salesforce, etc.)
-   Enable customers to seamlessly navigate between applications using a
    single identity (SSO)
-   Enable multi-factor authentication (MFA), implement a secure password
    policy
-   Grant authorized access to web APIs for applications and
    users

### What application types does AAD B2C support?

AAD B2C is not restricted to any particular language or
platform, and works with most modern application architectures -- web,
mobile, desktop, SPA, and web APIs. AAD B2C
employs industry standard protocols, such as OAuth 2.0 or OpenID Connect
to authenticate users.

### How does AAD B2C authenticate users?

AAD B2C works as a cloud-based extension for apps.
Unauthenticated users are redirected to MS Azure, where they can log in
and/or sign up for a new account. After a successful login, AAD
B2C issues a token and returns the user back to the original
application. If SSO is enabled, users can continue to other
applications in the "pool" with the same token. AAD B2C gives
developers full flexibility to customize all authentication steps, as
well as the look and feel of the login/signup experience.

### How secure is AAD B2C?

If your apps are using AAD B2C, Microsoft is responsible for
the entire authentication process, from accepting and validating user
input to safely storing user data in Azure Active Directory. The
registered applications are only responsible for accepting and
validating access tokens.

AAD B2C authentication is based on JSON Web Tokens
(JWTs) -- an open standard ([RFC
7519](https://tools.ietf.org/html/rfc7519)) for securely sending
information between parties inside compact, digitally signed tokens.

### Do I need to rewrite my applications to use AAD B2C?

Applications using AAD B2C must be able to do two things:
redirect users to AAD B2C and accept/validate the JWT
tokens that it generates. These are the only changes that must be
implemented, and there are dozens of libraries (for .NET, Java,
PHP, Python, JavaScript, etc.) to help you with that. All the
complex logic related to accepting and sanitizing user input, querying
user DBs, managing SSO sessions, etc. is handled by
AAD B2C.

All features, including SSO, MFA, and integrations
with social/corporate IDPs, can be configured in the UI.
AAD B2C also provides advanced tools to build highly customized
authentication experiences and integrate with arbitrary IDPs
and even APIs.

### What does a typical implementation process look like?

The implementation typically involves three steps:

-   Architecture planning. In the planning stage, an Azure professional
    reviews existing apps and designs an appropriate architecture for
    the AAD B2C service. They may also provide guidance on what
    changes will be required to the code.
-   Implementation. During the implementation stage, an AAD B2C
    service is created and configured in MS Azure Cloud. In case the
    apps are not directory-aware, the logic for accepting and validating
    JWT tokens is implemented too.
-   User migration. During the migration stage, if that is required by
    the project, users are moved from existing data storage into the
    AAD B2C directory. AAD B2C does not have to store
    users in the cloud and can do federated authentication (e.g., via
    existing ADFS).

Still not sure if AAD B2C is suitable for your specific requirements?
Contact one of our representatives.
