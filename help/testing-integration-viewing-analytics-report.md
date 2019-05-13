---
title: Testing the integration by viewing an Adobe Analytics report
seo-title: Testing the integration by viewing an Adobe Analytics report
description: null
seo-description: Learning how to test the integration by viewing an Adobe Analytics report.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991

---

# Testing the integration by viewing an Adobe Analytics report{#testing-the-integration-by-viewing-an-adobe-analytics-report}

After you have created the necessary variables in Adobe Analytics, linked them to Dynamic Media Classic events and completed the necessary implementation steps, then you should test the setup. You can test and verify that the data is being captured, inside Adobe Analytics itself. If the setup works here, then no further steps are needed. Assuming you followed the steps above and linked your Dynamic Media Classic event data to one or more custom traffic variables, then follow this workflow to test your data inside Adobe Analytics.

**To test the integration by viewing a Adobe Analytics report**

1. Launch a Dynamic Media Classic viewer from your account, particularly one that broadcasts the metric that you want to capture, and interact with it to create some event data.

   For example, if you want to measure the most popular alternative views in an Image Set, then preview an Image Set and click on the different thumbnails images.

1. Inside Adobe Analytics, go to Custom Traffic &gt; Custom Traffic 1-10 &gt; [Name of prop], selecting your traffic prop name from the menu choices.

   For example, to access the LoadAsset prop in our sample account, the proper menu choice would be Custom Traffic &gt; Custom Traffic 1-10 &gt; LoadAsset. If you have more than ten custom props, then you may see additional menu choices as well.

1. View the chart produced by Adobe Analytics. Note that this is typically just the data for a single metric. If you also want to know with which asset this data is associated (for example, which video is being watched to only 50%, or which image in a set is most popular), be sure to capture the asset data of this event as well.

>[!NOTE]
>
>All Dynamic Media Classic viewer data is displayed and reported in Custom Traffic reports or Custom Conversion reports of Adobe Analytics.

For more information, see [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
