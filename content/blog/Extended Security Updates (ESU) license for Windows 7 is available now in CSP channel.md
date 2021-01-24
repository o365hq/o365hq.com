+++
title = "Extended Security Updates (ESU) License for Windows 7 is available now in CSP channel"
description = "While many of you are well into your journey of deploying and/or servicing Windows 10, Microsoft understands that everyone is at a different point in the upgrade process. If your organization is unable to complete the transition from Windows 7 Pro, Microsoft wants to help you by ensuring that the devices running these select editions and versions continue to receive security updates while you complete your Windows and Windows Server upgrade projects."
date = 2019-12-05

[taxonomies]
tags = ["howto", "windows 10 update"]
+++

We are happy to announce that [Windows 7 Extended Security Updates
(ESU) 2020
SKU](https://buymssoft.com/license/CSP-DG7GMGF0FL73-0002 "p/n: CSP-DG7GMGF0FL73-0002")
is available on Buymssoft.com for purchase for
\$62^[1](#fn11224028605e1e1c1175529-1)^ per year. The price will
increase in 2021.

Extended Security Updates (ESU) for Windows 7 have been available for
some time through specific volume licensing programs, like EA
(Enterprise Agreement). It was a problem because not every organization
was eligible for one. But since December 2, 2019, you can purchase
Windows 7 ESU SKUs in CSP channel. There is
no minimum order.

### Purchasing Windows 7 ESUs through a Cloud Solution Provider (CSP)

The process is very simple:

1.  Contact your manager and ask about Windows 7 ESUs.
2.  Let them know the number of licenses that you would like to purchase
    (per device).
3.  Provide your Azure AD (Office 365) Tenant Name ([What is the Office
    365/Azure AD
    tenant](https://o365hq.com/faq/what-is-office-365-or-azure-ad-tenant)).
4.  Receive your invoice and make a payment.
5.  Receive your keys and install them.

Alternatively, just place an order via our website
[here](https://buymssoft.com/license/CSP-DG7GMGF0FL73-0002).

### Installation and activation

**First, install the ESU product key using the Windows Software
Licensing Management Tool (slmgr):**

1.  Open an elevated Command Prompt.
2.  Type slmgr /ipk and select Enter.
3.  If the product key installed successfully, you will see a message
    similar to the following\
    ![](https://gxcuf89792.i.lithium.com/t5/image/serverpage/image-id/138244i39443211C3ACAFCD/image-dimensions/535x168?v=1.0)

**Next, find the ESU Activation ID**

1.  In the elevated Command Prompt, type slmgr /dlv and select Enter.
2.  Note the Activation ID, as you will need it in the next step.\
    ![](https://gxcuf89792.i.lithium.com/t5/image/serverpage/image-id/138248i997F51A8C3D1BDC0/image-dimensions/574x260?v=1.0)

**Now, activate the ESU product key**

1.  Open an elevated Command Prompt.
2.  Type slmgr /ato and press Enter.\
    ![](https://gxcuf89792.i.lithium.com/t5/image/serverpage/image-id/138256i9E2F9617FA7E79E2/image-dimensions/500x214?v=1.0)

If your organization still has devices running Windows 7, Windows Server
2008, or Windows Server 2008 R2, we recommend that you take the steps
outlined above today to take advantage of Extended Security Updates and
help ensure that your devices continue to receive necessary security
updates after January 14, 2020.

**Footnotes**

^[1](#fnrev11224028605e1e1c1175529-1)^ The original price for Win 7
ESU was \$50. But on Dec 10, 2019, it was increased to \$62.
We got this communication from Microsoft:\
"UPDATE: Windows 7 ESU in CSP -- Pricing\
On December 2, Windows 7 Extended Security Updates (ESU) were
made available to businesses of all sizes through Cloud Solution
Provider (CSP).\
We have identified a price discrepancy with the Windows 7 Extended
Security Updates available through the CSP channel. As of
Tuesday, December 10, we have fixed the discrepancy to ensure that all
commercial customers have the same suggested retail price for the
Windows 7 ESU. Now, the ESU price that CSP
partners see will align to the pricing offered through our volume
licensing channel since April 2019."
