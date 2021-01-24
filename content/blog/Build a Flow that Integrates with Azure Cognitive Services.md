+++
title = "Build a Flow that Integrates with Azure Cognitive Services"
description = "Microsoft Flow helps companies arrange no-code workflows between apps and services to synchronize files, receive messages and alerts, gather all the necessary information, and more."
date = 2019-11-14

[taxonomies]
tags = ["microsoft flow", "office 365 business apps"]
+++

![](https://o365hq.com/images/609.jpg)

*Microsoft Flow and Azure Cognitive Services* allow users to extract
rich data from images automatically. With Flow and Custom Vision Service
(part of Azure Cognitive Services), the team can build a simple workflow
that automates the task, saving time and effort. The flow can be applied
to automatically crawl, analyze, and retrieve a large collection of
images -- from external image sources, social media feeds (such as Twitter
and LinkedIn), or a corporate image library. In addition to that, the
service could be trained to find more detailed information, such as the
number of objects, color, design layout, accessories, and more. Applied
in such a way, Flow and Custom Vision Service together can save time,
provide more accurate and reliable results, and free up team members for
more value-adding tasks.

You can now easily build a workflow in Microsoft Flow that submits an
image to Custom Vision Service and receives an analysis, all without
code. Every flow needs a trigger to start it. It is possible to trigger
the flow from a mobile device or add a manual trigger to start the flow.
The flow needs an input file to run. In this case, the user will add a
file from a mobile phone.

![](https://o365hq.com/images/605.png)

You can enter the globally unique identifier (GUID) for the
Custom Vision Service project you want to use for the analysis of the
image and choose a content type you want to analyze. You can use data
from previous steps in the workflow, such as the *MyPicture* file
content specifier. This is the attribute defined to specify that the input
will be a picture. An attribute called *Predictions tag* is listed in
the dynamic content and generates a yes/no result (i.e., content that can
be used now and later in the flow).

Microsoft Flow makes automating the image upload possible in just a few
clicks, with its intuitive and easy-to-use interface. It makes it easy
to modify the flow to automatically send users a notification for visual
screening when the *Predictions Probability* is less than the preset 85%
threshold.

![](https://o365hq.com/images/606.png)

You can quickly extend the flow to align to your company's business
processes, such as uploading lower probability drone images to a
SharePoint document library and notifying any number of visual screeners
or approvers via email in just a few clicks by adding additional actions
in the series.

![](https://o365hq.com/images/607.png)

Whether your business needs require simple serial flows, as in our
example, or multistep parallel scenarios across your entire
organization, Microsoft Flow's intuitive interface makes designing,
testing, and deploying it quick and easy.

It is very simple to build a workflow that uploads an image to Custom
Vision Service, analyzes it for specific content, returns a notification
specifying whether and with what probability that content exists in the
image, and then uploads high-probability images to a SharePoint asset
library.

This simple flow can easily be scaled up to more complex scenarios. For
example, it can run when someone tweets or puts an image on Instagram
with certain hashtags, or refined further by training Custom Vision
Service to recognize the model or type of drone. Microsoft Flow and
Azure Cognitive Services allow you to intuitively build intelligent
algorithms into your image classification app, reducing human visual
review processes and speeding up distribution of product collateral for
the Marketing team.

![](https://o365hq.com/images/608.png)
