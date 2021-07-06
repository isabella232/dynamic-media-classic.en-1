---
title: Log in to Adobe Analytics
description: Learn how to log in to Adobe Analytics.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
---
# Log in to Adobe Analytics{#log-in-to-adobe-analytics}

Before you log in to configure Adobe Analytics reports and match Adobe Analytics report variables to Dynamic Media Classic events, verify that you are a member of the Web Service Access group in Adobe Analytics. Members in this group can access all reports in the specified report suites by way of the Experience Cloud’s Web Services API regardless of the permissions set in the interface. To add a member to the group, in Adobe Analytics, click **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Edit Groups]**.

When you log in, you have the option of entering your Experience Cloud Org ID to use the latest video analytics implementation. If you choose not to enter your ID, video reporting still works. However, it can cause the data to not integrate correctly with other data for that client from outside Dynamic Media Classic.

>[!NOTE]
>
>If your Adobe Analytics account has been migrated to Adobe IMS-based authentication (Identity Management System) for login, entering direct credentials does not work.

**To log in to Adobe Analytics:**

1. Near the upper-right corner of the Dynamic Media Classic page, tap **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**.
1. In the left pane, under **[!UICONTROL Application Setup]**, tap **[!UICONTROL Adobe Analytics]**.
1. In the Adobe Analytics Configuration page, tap **[!UICONTROL Adobe Analytics Login]**.
1. In the **[!UICONTROL Adobe Analytics Login]** dialog box, enter your company name, Experience Cloud Org ID (optional), username, and the *shared secret* key in the **[!UICONTROL Password]** text field.

   You can retrieve the *shared secret* key from the Analytics Admin Console. See [How to get API credentials for user accounts](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md).

1. Click **[!UICONTROL Login]**.
1. In the **[!UICONTROL Report Suite]** drop-down menu, choose a report suite, then click **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >The first time you log in to Adobe Analytics, the Report Suite drop-down list is blank. You do not choose a report suite the first time you log in. After you log in for the first time, log out, and then return to the Adobe Analytics screen. Log in again to be able to choose a report suite.

>[!MORELIKETHIS]
>
>* [Configuring Adobe Analytics reports](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
