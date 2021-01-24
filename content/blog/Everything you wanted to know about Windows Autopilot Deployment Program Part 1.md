+++
title = "Everything you wanted to know about Windows Autopilot Deployment Program (Part 1)"
description = "How can the end user can deploy a new device? Do you have a soft spot for new, shiny devices? Who doesn’t? But you have to take the rough with the smooth and spend a lot of time to make all the necessary configurations and settings before you can actually enjoy your new device. Well, not anymore – forget about the old way of deploying machines. It was costly and time-consuming. You had to build a custom image, gather drivers, etc., to deploy an operating system to a machine that was shipped with an operating system already installed by the hardware vendor."
date = 2019-03-15

[taxonomies]
tags = ["howto", "windows autopilot"]
+++

If you would like to read the other parts in this article series,
please go to:

-   [Part
    2](https://o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-2)
-   [Part
    3](https://o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-3)
-   [Part
    4](https://o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-4)

![](https://o365hq.com/images/257.png)

Microsoft introduced a new way of doing things. You take the device out
of the box and do not reimage it at all, only transform it into something
that is ready for business. You can layer all the necessary
configuration on top of that core operating system that comes from the
OEM (Original Equipment Manufacturer), preoptimized for their
hardware. It is much cheaper and it opens up new scenarios, like the
user can deploy the device without an IT specialist even touching it. Or the
device can deploy itself after being plugged in and connected to a
network, and more.

![](https://o365hq.com/images/260.png)

Changing this process is beneficial for both users and IT specialists:

1.  End users can do the deployment themselves. All the policies and
    user's data will come to the device from the cloud. The user won't
    have to waste the rest of the day before getting productive again.
    The device can be shipped directly to the end user with a simple set
    of instructions, pretty much like -- take the device, plug it in,
    turn it on, connect it to a Wi-Fi network, type in your ID and
    password, and off you go. Sit back and watch the machine set itself
    up. You can start working in no time.
2.  The IT specialist doesn't need to touch the device to configure it,
    because the preinstalled OS (that is typically Windows 10 Pro) may be
    transformed into anything you need as you layer on top of that OS
    all of your software, which could include security suites,
    productivity applications, Office, etc.

![](https://o365hq.com/images/261.png)

#### Administration

As far as administration is concerned, there are four portals to upload
the devices to Autopilot.

![](https://o365hq.com/images/258.png)

Most of the customers use the *Intune portal*. Three other portals are
more targeted -- *Microsoft 365 Business* is primarily for SMBs
using a corresponding subscription. The *Partner Center* portal is primarily
used by distributors and resellers, those who add devices to your
organization on your behalf. *Microsoft Store for Business* was an
initial portal for maintaining Autopilot devices, but it is now the
place to do the administrative actions for those customers who are
working with third-party MDM services.

Here we will focus primarily on Intune, going through three basic steps
for Autopilot deployment (the experience on the other portals will be
very similar).

#### Step 1. Register devices

The easiest way to register devices is to have someone else do it. There
are now six OEMs that are completely ready to go.

![](https://o365hq.com/images/259.png)

These OEMs have support for placing an order and are able to
register new machines for your organization.

Let's see what the OEM, distributor, or reseller can do for you.

-   Add new devices to Azure tenant (to be specific -- to the Autopilot
    deployment service) at the time your order is processed;
-   Associate devices to customer's purchase order for easy device
    grouping. OEM will actually tag the device with a purchase
    order ID, so all of the devices, when they show up in Intune, will
    have an attribute on them that says which purchase order that went
    to. You can now use that attribute to group them, which is
    convenient.
-   Tag devices with a customized label. For example, you may ask the
    OEM to mark all laptops you ordered with a laptop tag and
    all desktops with a desktop tag, so that you can group them by that
    attribute.
-   Preinstall OS that is ready to be transformed. Some OEMs
    provide a clean Windows free from unsanctioned software; some have
    a different opinion on what should be preloaded on their devices. To
    get a clean OS, you might have to ask nicely in some cases, or pay a
    little bit in some other cases.

If your OEM, reseller, or distributor doesn't do this, or you
want to register existing devices, you have this option on the back end
(follow subsequent articles to learn more).

#### Step 2. Assign profile

Imagine having bought a certain number of machines and they have now
been added to your Autopilot list by the OEM. Well, the
OEM doesn't assign a profile; that is still a responsibility of
the customer. You obviously don't want to do that for each of your
machines, especially if there are quite a few of them. It's really
tedious! Intune can help you with that. Create a profile with
necessary settings, give it a name, save it, and Intune will apply it to
the individual machines.

**How to create this profile**

In the Intune console, click *Device enrollment* and then *Windows
enrollment*. In this article we are focusing on the user-driven
deployment mode, so choose this option from the drop-down menu. This
mode presumes that the end user will deploy the machine. Settings will
show you many options to configure, like hide user license agreement and
don't show any privacy pages.

You can suppress the change account option so your end user can't
escape out of customized OOBE. This is important because the
machine doesn't get the Autopilot profile until it is connected to a
network, so if the user never connects to a network, the device never
gets the settings configured by the organization. You should try your
best not to allow them to skip out of the process; otherwise, this would
not do any good. By the way, the S mode devices (with secured OS) always
require an internet connection, so you are perfectly safe in this case.

You have an option to specify if the user should end up as an admin or
not. You will still be able to sign in to this machine with other tenant
admin accounts, but the users setting up the machine themselves wouldn't
have those rights.

![](https://o365hq.com/images/265.png)

The newest option that works with Windows 10 1809 is the naming
template. As of now, there are two types of naming patterns: an x-digit
random number or a serial number. To customize a device name, you may
enter a prefix (CMN, in our example) and then choose a serial
or a random number that will be added to that prefix.

![](https://o365hq.com/images/263.png)

When the deployment profile is ready, you need a user or a group of
users to assign it to. The group can be created manually, or, making a
step further to automation, you can create dynamic groups. With the
latter, you don't manually put the machines into a group -- you build a
dynamic query that specifies what computers should be in that group. As
soon as the OEM registers another batch of computers into the
Autopilot, Azure AD objects are automatically created for each one of
those with the specific attributes. Then the dynamic group picks them
up based on this attribute, and Intune provides the profile of
settings.

Remember when we were talking about OEM registering new
devices for your company, we mentioned that an order ID tag or custom
device tag can be added to simplify grouping? This is your time to use
this functionality. The easiest way is to apply the exact same profile
to every single registered machine. You create a
group, name it, and put in a query that selects all the computers based
on the attribute that only exists on Autopilot registered devices (in our
example, the query says the created group should contain all of the
machines that have ZTDId tag, which is present on every
Autopilot registered device). Over time, AAD evaluates the
query and selects all the machines that meet these rules.

![](https://o365hq.com/images/264.png)

The same applies to any attribute of your choice, whether it be the purchase
order ID or custom tag.

When the profile is created, the group is formed. Just let Intune
tie these together, assigning a profile to a group. On the profile page
in Intune, under Assignments, specify one or more groups. In this example,
we will select "Non-Kiosk Devices" and as a result, Intune will constantly
examine that group to see if there are any new machines and will assign
the profile to them.

![](https://o365hq.com/images/266.png)

That could be all the administration you ever need to do -- create the
profiles, assign them to groups, and put the right computers in the right
groups (or create groups with the right queries). Just make sure that
the OEM puts the devices into your tenant with the right
attributes during the ordering process, and the rest will happen automatically.

#### Step 3. Deployment

After being shipped to the employee, the device boots up for the first
time and instantly checks with the Autopilot deployment service to see
if it belongs to any organization. It may be hard to imagine, but every
Windows 10 device checks in with the Autopilot deployment service when
it gets a network connection. If it is not registered to Autopilot, it
goes through the normal flow of OOBE (probably, it is a
consumer device). If it turns out to be registered to an organization
and it has a profile associated with it, then it goes through the
customized deployment your organization preconfigured through the
profile.

To make sure that apps and settings are completed prior to the employee
gaining access to the desktop, you can configure *the enrollment status
page* to remain on the screen until the deployment is done (requires
version 1803 with May cumulative update or later). This page displays
progress of deployment, which goes through the three phases: device
preparation, device setup, and account setup.

![](https://o365hq.com/images/268.png)

This page will show up during deployment if you specify the desired
settings in the Intune console under *Windows enrollment*, customizing
the user experience. Right now, there is just one global setting used for
all users, but improvements to target specific groups are expected in the future.

![](https://o365hq.com/images/262.png)

In these settings, you may configure the enrollment page to show
progress, block the device before all the apps and data are pushed
down, put in a custom message in case of errors, specify a timeout (if
it takes longer than, say, 60 minutes, go ahead and let the user onto
the desktop), etc. Once that is configured, all the Autopilot deployments
will show this automatically as part of the process.

Instead of a conclusion, here is a little mind-twisting picture that visualizes
all that was discussed above.

![](https://o365hq.com/images/267.png)

This article is just the beginning; Autopilot has much more to offer to
turn deploying and resetting your machines into a breathtaking
experience, so follow us to learn more.

Download our PDF [Zero Touch
Deployment.pdf](/file_download/12/Zero_touch_deployment.pdf)
