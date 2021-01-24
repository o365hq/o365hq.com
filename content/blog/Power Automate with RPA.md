+++
title = "Power Automate with RPA"
description = "All enterprises are embracing the importance of using data to drive business outcomes. The Microsoft Power Platform empowers them to control data from a multitude of sources. Making data work more efficiently requires that all employees can deploy it to drive business impact. "
date = 2020-04-14

[taxonomies]
tags = ["office 365 business apps", "powerapps"]
+++

Microsoft is integrating AI, Machine Learning, and Robotic Process
Automation (RPA) into the Power Platform to automate tasks that
are typically performed electronically via optical character recognition
systems (OCR), or manually by human workers.

Power Automate will be adding new RPA capabilities with UI
flows that will build on its already extensive automation capabilities.
RPA systems use software robots (bots), or AI workers, to
generate the action list by "watching" users accomplish their tasks in
the application's graphical user interface (GUI). These
RPA systems then perform the automation by repeating those
tasks directly in the GUI. This can reduce the development cost
and accomplish those tasks in situations where APIs may not
exist, like legacy software applications.

![](https://o365hq.com/images/721.png)

The Power Platform allows the tackling of common process automation scenarios,
like invoice processing. Eliminating manual steps performed by human
beings and replacing them with automated processes will reduce the
amount of time needed to accomplish these common tasks and will
improve data entry accuracy through a reduction in transcription errors,
and will free skilled information workers to be more productive in other
areas of their roles. Automating invoice processing also has the
potential to dramatically reduce turnaround time, as electronic systems
process significantly higher volumes of invoices per hour when compared
to traditional OCR or manual methods.

Power Automate's out-of-the-box low to no-code solutions help you
quickly configure your workflow to trigger when an email arrives in an
Outlook 365 inbox. You can narrow the scope of the action by adding your
email alias. This will be replaced later with the email of the person
who is responsible for approvals after testing. The action will also
check for an email that has an attachment and the word "invoice" in the
subject line. This creates a focused and narrow trigger that only fires
under these specific conditions.

The *Get attachment* action in your flow is used to pass that document
through the subsequent invoice process automation actions. It is simple
to train the *Invoice Processing* model by uploading a small quantity of
invoice samples. *AI Builder* can easily recognize and remove key-value
pairs and table data from form documents. Once trained, the model is
used to automatically extract similar information from additional
documents that use a similar format -- without OCR or manual
human processes. During the training process, you can easily select the
fields from the invoice that are important, like *Due Date*, *Bill to*,
*Balance due*, *Primary contact*, and *Contact email address*, among
others.

![](https://o365hq.com/images/722.png)

In cases where the balance due is greater than or equal to two thousand
dollars, you can set up a Microsoft Teams connector to automatically
notify the approving party to review the high-value invoice. The action
has two options: \_Approve\_ and *Reject*. The Headline will appear in
the approver's Teams chat channel from the Flow bot. It is also possible
to set the *IsAlert* option to *Yes*. This will draw the attention of
the approving party with visual and audible cues, a notification on the
Teams icon, and an audible ding, ensuring the invoice is reviewed
promptly.

You can use the power of AI and Machine Learning to automate invoice
data entry into your company legacy invoicing solution. Power Automate's
intuitive user experience allows you to quickly add the last action in
the chain, *UI flows*. *UI flows* prompts you for information required
to bridge the gap between data in the cloud and actions performed on
your local machine by *UI flows*.

*UI flows* helps detect the user interface elements users interact with
when they perform data entry in the organization's Invoicing app. The
first field users interact with is the Date field, used to capture the
*Due date* information from the invoice.

*UI flow's* modular design creates efficiency by allowing you to repeat
configuration steps quickly in sequence: \_Account\_, *Amount*, and
*Status*. *The Power Platform's* focus on user-centric design and
democratization of solution development is on full display here. UI
flows simplifies configuration steps by presenting them to the user in
intuitive, logical, and easily understood concepts.

![](https://o365hq.com/images/723.png)

With the recording started, UI flows captures the sequence of events
your company data entry users execute when performing their daily tasks.
UI flows does not impede users or require them to perform unfamiliar
actions -- quite the opposite. UI flows captures the natural human actions
required to perform a specific task.

Expanding the *Run Invoicing script* action, you can see the
interactions captured by UI flows during task execution as a linear
sequence of flow actions. UI flows has accelerated and simplified
development of the flow for you by eliminating manual configuration
steps and removing coding requirements.

The Power Platform, AI Builder, and UI flows have empowered one employee
to accomplish the work of what would traditionally require a lengthy and
costly development cycle performed by a highly specialized and compensated
team of developers and management staff -- technological democratization
in action!

![](https://o365hq.com/images/724.png)

After navigating to *Outlook*, you can submit an invoice processing
request via email, just like the multitude of invoices processed by
companies every day. What used to take a team of humans and OCR
technology now happens seamlessly behind the scenes in a fraction of the
time, at a fraction of the cost.

Microsoft's bold bet and expertise in the areas of AI, machine learning,
and RPA empowers your team to develop solutions to unique
problems and inefficiencies your organization is experiencing. Help your
employees accomplish more and solve real-world business problems, like
invoicing inefficiency, by automating repetitive tasks with *AI
Builder*, *UI Flows*, and the *Power Platform*.

![](https://o365hq.com/images/725.png)
