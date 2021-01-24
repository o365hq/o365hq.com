+++
title = "Windows 7 Extended Security Updates 2020: An ultimate, step-by-step guide on purchasing and activation"
description = "As you may have heard, Windows 7 is at the end of its life cycle. This makes users more susceptible to malware attacks and turns Window 7 into a minefield of security threats. The Extended Security Update program is an alternative for consumers to manage certain legacy Microsoft products after the support is ended. And this is an ultimate step-by-step guide on how to purchase and activate  Windows 7 Extended Security Updates for your computers."
date = 2020-01-10

[taxonomies]
tags = ["howto", "windows 10 update"]
+++

We will help you get those elusive and hard-to-find Windows 7 Extended
Security Updates for your computers.

Please follow the steps listed below to make sure you purchase the right
product for your device(s).

***NOTE***:

The original price for Win 7 ESU was \$50. But on Dec 10, 2019,
it was increased to \$62. We got this communication from Microsoft:

> UPDATE: Windows 7 ESU in CSP -- Pricing On
> December 2, Windows 7 Extended Security Updates (ESU) were
> made available to businesses of all sizes through Cloud Solution
> Provider (CSP). We have identified a price discrepancy with
> the Windows 7 Extended Security Updates available through the
> CSP channel. As of Tuesday, December 10, we have fixed the
> discrepancy to ensure that all commercial customers have the same
> suggested retail price for the Windows 7 ESU. Now, the
> ESU price that CSP partners see will align to the
> pricing offered through our volume licensing channel since April
> 2019."

### Verify if your edition of Windows 7 is eligible for ESU

1.  Select *the Start button*, type *Computer* in the search box,
    right-click on *Computer*, and then select *Properties*.\
    ![](https://msegceporticoprodassets.blob.core.windows.net/asset-blobs/4502677_en_1)
2.  Under Windows edition, you'll see the version and edition of Windows
    that your device is running. ESU are available for
    **Windows 7 Professional**, **Windows 7 Enterprise** and **Windows 7
    Ultimate**.

### Verify that you have all the Windows 7 Updates installed

1.  Open the Windows Control Panel, and then click System and Security.\
    ![](https://www.dummies.com/wp-content/uploads/283118.image0.jpg)
2.  Click Windows Update.\
    ![](https://www.dummies.com/wp-content/uploads/283120.image2.jpg)
3.  In the left pane, click Check for Updates.\
    ![](https://www.dummies.com/wp-content/uploads/283122.image4.jpg)
4.  Allow for updates to download and install, and then check for new
    updates again to make sure there are no new updates.

### Make sure all your Windows 7 computers that need to be ESU-enabled are connected to the Internet.

ESU MAK Phone activation was recently added as an
option for non-Internet-connected devices. This article doesn't describe
that activation process.

### Check the instructions below and decide if you will be able to install and activate the Win7ESU keys yourself.

-   If yes -- please skip this step.
-   If no -- reserve about \$49 per PC for [Windows 7 ESU
    Remote Installation
    Service](https://buymssoft.com/directlink?q=_ITPWW240CONOT.1).
    Internet connectivity is required.

### Purchase the required number of licenses using [this link](https://buymssoft.com/license/CSP-DG7GMGF0FL73-0002).

An Office 365 / Azure AD tenant name will be required to place an order for
ESU licenses. It's ok if you don't have one. We will register a
tenant for you. It's free, and there are no strings attached. If you have a
tenant and want to use it -- make sure you complete the questionnaire
after you place your order.

Usually, it takes about a day to process an ESU order. When an
order is processed, you will receive an email with a MAK (Multiple
Activation Key).

### Check your mailbox and Junk Mail folder for an email from us with the activation key.

Depending on what office process the order, the email with the key may
come from one of the following domain names:
o365hq.com OR itpartner365.com.

When you have the key, you are ready for the next step.

### Install and activate ESU on your Windows 7 computers

1.  Install the ESU product key using the Windows Software
    Licensing Management Tool (slmgr):
    1.  Open an elevated Command Prompt.
        1.  Click Start
        2.  In the search box, type **cmd**.
        3.  Right-click on **cmd.exe** and choose Run as Administrator.
            If done properly, the below User Account Control window
            opens.
        4.  Click Yes to run the **Windows Command Prompt** as
            Administrator.
    2.  Type **slmgr /ipk** and enter your ESU MAK key
        and press Enter. Make sure you have spaces between slmgr and
        /ipk and your MAK key. Your slmg command should look
        like this: **slmgr /ipk A7B6D-N3D1F-J34ND-LP3NA-32BNA**
    3.  If the product key installed successfully, after a short delay,
        you will see a message similar to the following:\
        ![](https://gxcuf89792.i.lithium.com/t5/image/serverpage/image-id/138244i39443211C3ACAFCD/image-dimensions/535x168?v=1.0)
2.  Next, find the ESU Activation ID
    (77db037b-95c3-48d7-a3ab-a9c6d41093e0):
    1.  In the elevated Command Prompt, type **slmgr /dlv** and select
        Enter.
    2.  Note the Activation ID, as you will need it in the next step.\
        ![](https://gxcuf89792.i.lithium.com/t5/image/serverpage/image-id/138248i997F51A8C3D1BDC0/image-dimensions/574x260?v=1.0)
    3.  It should be 77db037b-95c3-48d7-a3ab-a9c6d41093e0. It's the
        Activation ID for the year 2020.
3.  Now, you'll activate the ESU product key:
    1.  Open an elevated Command Prompt.
    2.  Type **slmgr /ato 77db037b-95c3-48d7-a3ab-a9c6d41093e0** and
        press Enter.\
        ![](https://gxcuf89792.i.lithium.com/t5/image/serverpage/image-id/138256i9E2F9617FA7E79E2/image-dimensions/500x214?v=1.0)
    3.  Once you have activated the ESU product key, you can
        verify the status at any time by following these steps:
        1.  Open an elevated Command Prompt.
        2.  Type **slmgr /dlv** and select Enter.
        3.  Verify Licensed Status shows as Licensed for the
            corresponding ESU program, as shown below:
            ![](https://o365hq.com/images/653.png){width="535"
            height="295"}
    4.  Once activated, continue to use your current update and
        servicing strategy to deploy Microsoft Windows Security Updates
        through Windows Update, Windows Server Update Services
        ([WSUS]{.caps}), Microsoft Update Catalog, or whichever patch
        management solution you prefer. You will receive updates until
        the end of 2020.

### Check the [Microsoft Windows 7 ESU [FAQ]{.caps} page] (https://support.microsoft.com/en-us/help/4527878/faq-about-extended-security-updates-for-windows-7) for additional information.

### Troubleshooting Windows 7 ESU installation and activation errors

**Error:** 0xC004F050 The Software Licensing Service reported that the
product key is invalid.

**Solution:** Install all the Windows Updates. Restart the computer.
Check for Windows Updates one more time to ensure your computer is up to
date. Disable any third-party antivirus and/or firewall software. Try
installation and activation one more time. If you have problems with
your Windows Updates subsystem -- please try this [Microsoft
Article](https://support.microsoft.com/en-us/help/10164/fix-windows-update-errors).

**Question** How many activations are left on your ESU
MAK key?

**Solution** [Source: Microsoft Windows 7 ESU
FAQ](https://support.microsoft.com/en-us/help/4527878/faq-about-extended-security-updates-for-windows-7)
-- Customers can determine the remaining activations on a MAK
key using VAMT}:

1.  Launch the VAMT}.
2.  In the left-side pane, select the Product Keys node.
3.  In the center pane, find the ESU Add-on MAK key.
    The remaining activation count is displayed in the Remaining
    Activation Count column.
