---
title: Testing the integration by viewing an Adobe Analytics report
description: Learning how to test the integration by viewing an Adobe Analytics report.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
---
# Testing the integration by viewing an Adobe Analytics report{#testing-the-integration-by-viewing-an-adobe-analytics-report}

After you have created the necessary variables in Adobe Analytics, linked them to Adobe Dynamic Media Classic events, and completed the necessary implementation steps, you can test the setup. You can test and verify that the data is being captured, inside Adobe Analytics itself. If the setup works here, then no further steps are needed. Assuming you followed the steps above and linked your Adobe Dynamic Media Classic event data to one or more custom traffic variables, then follow this workflow to test your data inside Adobe Analytics.

**To test the integration by viewing an Adobe Analytics report:**

1. Start an Adobe Dynamic Media Classic viewer from your account, particularly one that broadcasts the metric that you want to obtain, and interact with it to create some event data.

   For example, if you want to measure popular alternative views in an Image Set, then preview an Image Set and click the different thumbnails images.

1. Inside Adobe Analytics, go to **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > [Name of prop], selecting your traffic prop name from the menu choices.

   For example, to access the **[!UICONTROL LoadAsset]** prop in the sample account, the proper menu choice would be **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > **[!UICONTROL LoadAsset]**. If you have more than ten custom props, you see other menu choices as well.

1. View the chart produced by Adobe Analytics. This chart is typically just the data for a single metric. If you also want to know with which asset this data is associated, obtain the asset data of this event. For example, it is often useful to know which video is watched to only 50%, or which image in a set is popular.

>[!NOTE]
>
>All Adobe Dynamic Media Classic viewer data is displayed and reported in Custom Traffic reports or Custom Conversion reports of Adobe Analytics.

For more information, see [Analytics Tutorials](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html).