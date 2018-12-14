---
title: "Quick Start: Integrating Scene7 and Adobe Analytics "
seo-title: "Quick Start: Integrating Scene7 and Adobe Analytics "
description: null
seo-description: An introduction and Quick Start to integrating Dynamic Media Classic and Adobe Analytic to help you get up and running quickly.
uuid: 3f9e2c91-15d4-4b53-8220-9b1ca57c0b1d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: abec9a85-013c-4030-b129-bf27a89cb464
index: y
internal: n
snippet: y
---

# Quick Start: Integrating Scene7 and Adobe Analytics {#quick-start-integrating-scene-and-adobe-analytics}

Adobe Analytics is the industry-leading product that provides marketers with one place where they can measure, analyze, and optimize integrated data from all online initiatives across multiple marketing channels.

After integrating Adobe Analytics with the Scene7 Publishing System, you can get reports about the behavior of website visitors using Scene7 viewers on your website. For example, when a website visitor clicks a zoom target in a Scene7 Zoom Viewer, Adobe Analytics records this action. Adobe Analytics reports can gather cumulative information about user activity in Scene7 viewers.

Using Adobe Analytics reports, you can get a clear picture of the activity of customers on your website. You can determine which product presentations lead to conversion and which do not draw customer interest.

See also [Measuring Video in Adobe Analytics](https://marketing.adobe.com/resources/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>``A valid Adobe Analytics account is required to integrate Analytics with the Scene7 Publishing System and generate Analytics reports.

**Quick Start**

This Quick Start is designed to get you up and running quickly with Adobe Analytics Instrumentation Kit.

**1. Log in to Adobe Analytics by way of Scene7 and download Adobe Analytics report variables**

>[!NOTE]
>
>Before you can configure Adobe Analytics reports and match Adobe Analytics report variables to Scene7 events, verify that you are added as a member of the Web Service Access group in Adobe Analytics. Members in this group can access all reports in the specified report suites by way of the Marketing Cloud’s Web Services API regardless of the permissions set in the interface. To add a member to the group, in Adobe Analytics, click **Admin Tools** &gt; **User Management** &gt; **Edit Groups**.

After you have verified that you are a member of the Web Service Access group, in Scene7, click **Setup** &gt; **Application Setup** &gt; **Adobe Analytics**. On the Adobe Analytics Configuration page, click **Adobe Analytics Login**.

See [Log in to Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

In the Adobe Analytics Login dialog box, type your Marketing Cloud Org ID (optional), and your complete credentials, then click **Login**. On the Report Suite drop-down menu, select the name of the report suite that you want to use.

**2. Assign Adobe Analytics report variables to Scene7 viewer events and Scene7 variables**

On the Adobe Analytics Configuration page, specify the information you want in Adobe Analytics reports. For each Scene7 viewer event that you want information about, choose an Adobe Analytics variable (from your report suite) and a Scene7 variable.

* Viewer events describe the user activity that you want to measure in reports.
* Scene7 variables describe the data about user events that you want the reports to deliver.

The Adobe Analytics Configuration also offers tools for activating, editing, and deleting viewer events.

After you click Save in the Adobe Analytics Configuration screen, customized tracking code for measuring user activity is inserted in Scene7 viewers. This functionality lets you track user activity in Adobe Analytics reports.

See [Configuring Adobe Analytics reports](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

**3. Publish your Scene7 viewers**

Publish your Scene7 viewers so that the viewers (with code for tracking user activity in Adobe Analytics reports) are loaded on Scene7 servers. After you publish, this information is included in viewers and can be used for analyses by Adobe Analytics.

See [Publishing configuration information](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

**4. Place Scene7 viewers in your website**

Place the Scene7 viewers with Adobe Analytics tracking code on your website.

**5. Test the Adobe Analytics integration by viewing an Adobe Analytics report**

To view Adobe Analytics reports, go to the Adobe Analytics website. The Reporting page lets you view data and generate graphs and charts to measure user activity with different viewers.

See [Testing the Adobe Analytics integration by viewing an Adobe Analytics report](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
