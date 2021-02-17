+++
title = "Everything you wanted to know about Windows Autopilot Deployment Program (Part 2)"
description = "What you need to do to set the stage for Windows deployment with Autopilot. "
date = 2019-03-20

[taxonomies]
tags = ["howto", "windows autopilot"]
+++

If you would like to read the other parts in this article series,
please go to:

-   [Part
    1](o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-1)
-   [Part
    3](o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-3)
-   [Part
    4](o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-4)

In the previous article, we discussed in detail the [modern way of
Windows deployment with
Autopilot](o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-1)
. In case you missed it, here is a short recap. Autopilot basic flow
always has three steps:

1.  **Register the device.** The hardware vendor adds the devices your
    company has purchased to the Autopilot deployment service,
    associating them to your organization.
2.  **Assign a profile.** The Autopilot profile is created by the IT
    admin via Intune and gets synced from Intune into the Autopilot
    deployment service. When the devices registered by the OEM
    connect to the Internet, they get synced with Intune (or other
    MDM) and AAD where you can assign a set of
    profiles to them using the techniques that we looked at in the
    previous article.
3.  **Deploy the machine.** When you unbox the machine off the shelf and
    boot it, the device deploys itself or guides you through a seamless
    user experience, and it is available for productive work in no time.

Autopilot is really framed from the beginning of a machine's lifecycle
all the way until its end. When you're done deploying, there's an
ongoing management of that device, performed largely by Microsoft
partners, and in case of breakdown, you have either a repair option
(Autopilot reset, where if the device stops working at some point throughout
its lifecycle, you can quickly and easily reset it in one click, bringing
it back to a business-ready state) or retirement of the device.

![](https://o365hq.com/images/270.png)

### Prerequisites

Autopilot uses numerous technologies so to prepare for it, you have to
make sure you meet the following requirements (otherwise the deployment
may fail):

![](https://o365hq.com/images/275.png)

Support for Autopilot was initially introduced in *Windows 10 version
1703*. For new features and capabilities, later versions may be required,
but at least 1703. You then need some specific capabilities of
AAD and an MDM service. On the AAD
side it:

-   is automatic MDM enrollment, so when a device is joined
    into AAD, it automatically enrolls in Intune or any other
    MDM you configured.
-   has the ability to do custom company branding to display the customized log
    on the page. Make sure you check on this, because many cases of failed
    Autopilot deployment were caused by the absence of this
    configuration.

These capabilities, for most enterprises, are provided through either
Azure AD Premium, EMS, or a Microsoft 365 Enterprise E3 or E5
subscription. Specific Azure capabilities that make the process of
Autopilot deployment work are included in Microsoft 365 for small and
medium businesses and Microsoft 365 F1 for first line workers as well.

### Initial one-time configurations you will need to do

To achieve these prerequisites, you then need to go through some
initial configuration tasks.

1\) *Automatic MDM enrollment* can be set up in Azure portal
under *Mobility (MDM and MAM)* and then *Intune*.

![](https://o365hq.com/images/274.png)

The first thing you are offered to select is that *Some* users will be able
to enroll automatically and choose *Groups* that include them. Then
you put in the URLs for the MDM service you are
using. In this example it is Intune, but if you are using a different
MDM service, you can ask the vendor for specific URLs
needed for that MDM. All that is lacking is to make your
choices concerning *MAM* (Mobile Application Management) -- in
our case it is *Some* for User Scope, and the same group as for
MDM.

![](https://o365hq.com/images/277.png)

2\) *Company branding*. In Azure portal find *Company branding* and
*Configure*.

![](https://o365hq.com/images/276.png)

Configurations will allow you to select sign-in page background image,
custom square logo and custom text. Keep in mind that there are size
limitations to all these items.

![](https://o365hq.com/images/271.png)

There are also some advanced settings that may be interesting.

![](https://o365hq.com/images/272.png)

The company name will also appear on the sign-in page, but it is set up
under *Properties* in the Azure AD tenant, where you enter a *Name*.

![](https://o365hq.com/images/279.png)

After these configurations, the sign-in page will look like this:

![](https://o365hq.com/images/278.png)

3\) *Enable Windows Subscription Activation*, if desired. You may need
this feature if you want to step up to Windows 10 Enterprise to take
advantage of the enterprise features. Thanks to Subscription Activation,
any time the user signs on to the Windows Pro machine, it magically
becomes Enterprise without reboot or time delay, as it sees the license
assigned to the user in AAD and steps up to Enterprise. After
this, your machine runs a new SKU (Stock Keeping Unit) of
Windows that has new capabilities, and Intune will push the new settings
corresponding to these capabilities.

4\) *Ensure users can join devices to AAD*, otherwise, the
process isn't going to go very far, as deployment is performed by the
user. This ability should be granted at least to those users that are
expected to deploy a machine via Autopilot. This feature is set up in
AAD portal under *Devices*, and there -- *Device settings*,
which will display the table with necessary configurations.

![](https://o365hq.com/images/273.png)

On the Intune side, you may take care of some settings as follows.

-   *enable the enrollment status page* -- it is displayed during
    machine deployment and shows its progress (we discussed how to
    set it up in the [previous
    article](https://o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-1)
    , so take a look).
-   If you prefer that only Autopilot-registered devices can enroll in
    MDM, you have an option to create a [device enrollment
    restriction](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set)
    . *When this rule is in place, any time user wants to join a
    personal device (not registered to Autopilot) to AAD, which
    triggers an MDM enrollment, the AAD join as well
    as the enrollment will fail, and their personal device will stay out
    of your corporate environment*.

Do your homework well, and Windows deployment will be a delightful
experience for end users and won't become a challenge for IT admins in
your company.

To be continued... A little spoiler on the next article -- we will
discuss a completely touch-free and click-free Windows deployment and
more scenarios, so stay tuned for more updates.

Download our PDF [Zero Touch
Deployment.pdf](/file_download/12/Zero_touch_deployment.pdf)
