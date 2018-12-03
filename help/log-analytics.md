---
title: Log in to Adobe Analytics
seo-title: Log in to Adobe Analytics
description: null
seo-description: Learn how to log in to Adobe Analytics.
uuid: a2e5d1d0-92fd-4bfd-be9d-523951257b65
contentOwner: admin
cq-gepid: scene7/using/WSef8d5860223939e2-5fd4950512b2178e071-8000
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: aca2ddf6-1305-479d-b2de-b6ff7fa306bb
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 43.659-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/adobe_analytics_instrumentation_kit;/content/help/en/experience-manager/morehelp/adobe_analytics_instrumentation_kit
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Log in to Adobe Analytics{#log-in-to-adobe-analytics}

Before you log in to configure Adobe Analytics reports and match Adobe Analytics report variables to Scene7 events, verify that you are added as a member of the Web Service Access group in Adobe Analytics. Members in this group can access all reports in the specified report suites by way of the Marketing Cloud’s Web Services API regardless of the permissions set in the interface. To add a member to the group, in Adobe Analytics, click **Admin Tools** &gt; **User Management** &gt; **Edit Groups**.

When you log in you have the option of entering your Marketing Cloud Org ID to use the latest video analytics implementation. If you choose not to enter your ID, video reporting still works. However, it can cause the data to not integrate correctly with other data for that client from outside Scene7.

**To log in to Adobe Analytics**

1. Click **Setup** &gt; **Application Setup**.
1. In the left pane, under Application Setup, click **Adobe Analytics**.
1. In the Adobe Analytics Configuration screen, click **Adobe Analytics Login**.
1. In the Login dialog box, enter your company name, Marketing Cloud Org ID (optional), user name, and password. 
1. Click **Login**.
1. Choose a report suite, then click **OK**.

   >[!NOTE]
   >
   >The first time you log in to Adobe Analytics, the Report Suite drop-down list is blank. You do not choose a report suite the first time you log in. After you log in for the first time, log out, and then return to the Adobe Analytics screen. Log in again to be able to choose a report suite.

>[!MORE_LIKE_THIS]
>
>* [Configuring Adobe Analytics reports](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
