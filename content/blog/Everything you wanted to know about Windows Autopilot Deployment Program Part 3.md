+++
title = "Everything you wanted to know about Windows Autopilot Deployment Program (Part 3)"
description = "Scenarios for Windows Autopilot – User-driven, Reset, Self-deploying modes"
date = 2019-03-28

[taxonomies]
tags = ["howto", "windows autopilot"]
+++

If you would like to read the other parts in this article series
please go to:

-   [Part
    1](o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-1)
-   [Part
    2](o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-2)
-   [Part
    4](o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-4)

Autopilot is a name for a modern way of Windows deployment that you will
surely enjoy. If you are new to this technology, please check out our
articles on the
[overview](o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-1)
and
[pre-requisites](o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-2)
for Autopilot. Windows deployment has many facets, and therefore there
exist many scenarios where Autopilot can play its role. Grab some
popcorn and make yourself comfortable, we're starting.

![](https://o365hq.com/images/285.png)

### User-driven mode

The first scenario that was in Autopilot from the start is the
user-driven deployment. Microsoft initially supported only joining the
device into Azure Active Directory and enrolling it into Intune, with
Intune then pushing the configurations down to the machine so the users
could set up the device themselves. We will go through the whole process
of deployment for you to see what it looks like in practice.\
Imagine a user opens up a new OEM device, like a Surface Book,
for example. There is a generic Windows installation directly from the
OEM loaded on the device. When it boots up it will ask a few
things, like the language of the OS, the region, and the keyboard layout.

![](https://o365hq.com/images/284.png)

![](https://o365hq.com/images/282.png)

After establishing a network connection, the machine gets its instructions -- it "talks"
to the Autopilot deployment service and downloads a profile of settings 
that states exactly what organization the machine belongs to and its
further "behavior." The next step will be to act on that -- the
downloaded settings are used to customize the rest of the user
experience. If those settings include a naming pattern (which is
available for Windows 10 1809), the device will rename itself and reboot
(so don't worry, it is part of the process). After rebooting, it will
have the naming convention that you specified, and the user can get back
on to the network and then type in an e-mail address and password on the
logon page.

![](https://o365hq.com/images/281.png)

The logon page can be customized for your organization, or even for the
user. If you preconfigure the user this device belongs to, you can give
him/her a nice out-of-the-box experience -- users won't even have to
type their e-mail address, only the password will be required and the
configuration will be finished in a short time.

During deployment, Autopilot will join the device into AAD. It
will trigger the MDM enrollment and once that is over, the
machine will start receiving policies. To track the progress of that, the
enrollment status page (ESP) is quite handy. If you want to set
up ESP, take a look at this
article: https://o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-1
.

It's preferable to keep the user at this point until the configurations
are completed. You don't want your user to end up on the desktop while
stuff is still happening, as the user is not going to really know what
is going on. On the other hand, if all installations are done while the
enrollment status page is being displayed, the user gets into a more
favorable situation when the device is configured and ready for
productive work.\
The amount of time enrollment takes can vary greatly, depending on how
much stuff you're pushing down to the device, its technical
capabilities, and network bandwidth. If you have a lot of software and
settings, enrollment could take anywhere from five minutes at the minimum up
through potentially a couple of hours. If you don't want a user to wait
that long, you can configure which apps installation will block the
desktop and which apps won't.

![](https://o365hq.com/images/286.png)

When you change from *All* to *Selected*, you can choose what apps will
be in the block list, so the user will have to stay on ESP
before these are installed.

![](https://o365hq.com/images/283.png)

There might be some issues when tracking Office ProPlus installment, so
to avoid these, check out this
[information](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Support-Tip-Office-C2R-installation-is-now-tracked-during-ESP/ba-p/295514)
.

In Intune, you can target policies to the machine and they get processed
during the *Device setup* phase of the process; also, you can target
them to users, and they get processed during the *Account setup* phase.
For example, if you have 1 app targeting *All devices* and 2 apps
targeting a *User group*, you will see the corresponding information on
ESP (0 of 1 in *Device setup* and 0 of 2 in *Account setup*).
More information
[here](https://docs.microsoft.com/en-us/intune/windows-enrollment-status#device-setup)
.

Setting up a profile for this mode was discussed
[here](https://o365hq.com/blog/everything-you-wanted-to-know-about-windows-autopilot-deployment-program-part-1)
.

р3ю Windows Autopilot reset

The basic concept behind an Autopilot reset is getting rid of any
"garbage" that might have piled up on the machine, like extra apps,
extra tweaks, etc. There are two options -- reset locally, or
remotely, but the end result is the same in both of those cases.

1.  All apps, settings, and personal files are wiped clean;
2.  AAD join and MDM enrollment are preserved so the
    device is still managed; you won't get orphaned objects in
    AAD or Intune. You will continue to use the same ones;
3.  Any provisioning packages that were preinstalled with the OS are
    preserved;
4.  The options picked during OOBE, like language and keyboard
    and some of the details around the network connections, are preserved
    (if you wish to keep them).

Reset will take 20-30 minutes and you will end up at a logon screen. 
The machine is then ready to be used by the next person.

In Windows 10 version 1709, you can initiate the reset *locally* via a
keystroke -- *Windows-Control-R* from a lock screen. After this, it
brings you to an authentication prompt and you should type in an admin
account to approve the reset of the device. Obviously, you don't want
that enabled for every device in your organization, so there exists a
policy that needs to be configured first to enable local reset. If you
try the reset keystroke and nothing happens, you probably haven't
enabled that policy.

The *remote* piece is new for Windows 1809 and it offers a remote action
inside of Intune, where you select the device in question, then click on
*Autopilot reset* and it sends the reset command down to the device.

![](https://o365hq.com/images/287.png)

Initially, the reset option was intended for schools -- the machines after
the end of semester might get to a point where they need to start over.
But there are certainly enterprise scenarios for doing this as well,
like when an employee is being promoted or leaves the company and his/her
computer is prepared for a different purpose.

### Self-deploying mode

This mode is not associated with the user. It could be just a shared
device used by people at a help desk, call center, or in a school or
some place where anyone can walk up, put in credentials, and use the
device. It can also be a locked-down kiosk or digital signage (like a
flight status board at an airport). The user-driven mode doesn't fit
quite right for either of those scenarios, as during the deployment
process almost all user interaction is eliminated. On the contrary, with
this mode preconfigured on the device, as soon as it is plugged in,
turned on, and connected to a network, hands off -- the deployment is
completely zero touch from that point. All you can do is watch the
progress of setup.

Setting up the self-deploying mode involves the same three steps as
user-driven: registering your device, assigning a self-deploying
profile via Intune, booting up the machine and connecting to a network.

As far as Internet connection is concerned, one thing needs to be
pointed out -- if the machine is connected to the Internet via Ethernet,
the machine will just boot itself. If you don't have Ethernet or network
at boot, you'll have to interact with this machine just a little bit
setting up the Wi-Fi connection.

![](https://o365hq.com/images/289.png)

When you hit next, the device, connected to the Internet (as any other
Autopilot machine, starting with 1703 with the July update) is going to
reach out to Autopilot service and send up its harbor hash. The
Autopilot will send down a self-deploying profile, and if in that
profile you have included a device rename, the machine will go down,
applying the device rename. When the machine comes back up, you'll see a
company -branded welcome page, and in about 5-10 seconds, you'll get
automatically transitioned over to the enrollment status page.

![](https://o365hq.com/images/288.png)

On this page, you'll see three different steps -- device preparation,
device setup, and account setup. The device preparation section, typically,
tracks the state of the device as its joining to Azure Active Directory;
but how will it happen without a user authentication? A new mechanism
was invented to do this, and it requires *[TPM]{.caps}* 2.0 chip for the
device to authenticate into AAD on your behalf. Not sure your
devices have the luxury of possessing that? Most modern devices have
[TPM]{.caps}, or a Trusted Platform Module, which is a dedicated
microcontroller designed to secure hardware through integrated
cryptographic keys. Make sure it is a physical [TPM]{.caps} 2.0 chip,
devices with virtual [TPM]{.caps}s (like Hyper-V VMs) or with earlier
versions of chips (like [TPM]{.caps} 1.2) won't work with this mode.

Next, all the Intune configurations will come down to the device and set
up this machine to be a kiosk, for example, launching directly into the
kiosk web browser, a new app released recently to allow you to enable
some of the kiosk type scenarios.

Licensing requirements are the same for this mode as for the previous
one. The only difference is that it requires a [TPM]{.caps} 2.0 chip
(because authentication on your behalf happens using that chip) and
Windows 10 1809 (or later). If you don't have it, you'll see an error in
the *Device preparation* section of the ESP, because it won't
be able to join AAD without user credentials.

### Setting up a profile for the self-deploying scenario

Under *Device enrollment* in Intune, select *Windows enrollment* and
*Deployment profiles*. Choose *+Create profile*, give it a *Name* and in the
*Deployment mode* dropdown select *Self-deploying*.

![](https://o365hq.com/images/291.png)

When it comes to configuring the OOBE, unlike in user-driven
mode, there is nobody who can configure language, region, keyboard,
internet connectivity, and then authenticate. All these settings should
be automated, so when you are creating the Autopilot profile, you'll see
that some new options show up, allowing you to preselect the
language/region and the keyboard on the user's behalf.

![](https://o365hq.com/images/290.png)

All other settings are the same as for the user-driven mode. Hit Save,
wait for the profile to assign, and boot your machine -- it will deploy
itself with zero touches. So, self-deploying mode is ideal for user-less
scenarios or shared devices.

### Conclusion

Autopilot can be used in many ways. Here we discussed how the users
can deploy the new devices on their own, how a machine can be reset
locally and remotely, and how it can deploy itself without any
interaction from the user. More is coming -- in the next article, we
will focus on how to use Autopilot deployment for existing devices, how
to migrate from Windows 7 to Windows 10 with Autopilot, and how to join
a device to your on-prem AD during OOBE (in other words, a
hybrid AAD join scenario).

Download our PDF [Zero Touch
Deployment.pdf](/file_download/12/Zero_touch_deployment.pdf)
