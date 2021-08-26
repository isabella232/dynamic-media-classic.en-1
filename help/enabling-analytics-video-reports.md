---
title: Enable Adobe Analytics Video Reports
description: Learn how to enable Adobe Analytics video reports in Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
---
# Enable Adobe Analytics Video Reports{#enabling-adobe-analytics-video-reports}

Using Adobe Analytics heartbeat-based video reporting, you no longer must enable the four video viewer events (Play, Pause, Stop, Milestone) when you configure Adobe Analytics in Dynamic Media Classic. Video Heartbeat works with out-of-the-box Dynamic Media Classic HTML5 Video and Mixed Media viewers. The video player generates tracking data for viewing within Adobe Analytics Video Reports.

* For an introduction to streaming media and ‘heartbeat measurement’, see [About Adobe Analytics for Streaming Media](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* The integration of Adobe Analytics video reports with Dynamic Media Classic supports solution variables, but not custom variables.

  See [Audio and Video parameters](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) for more information about solution variables and custom variables.

* Out-of-the-box segments of one-minute increments are supported. However, custom segment reporting, such as customer-defined milestones based on time increments, % milestone, or offset milestones, is not supported.

  For more information about streaming media requirements and setup, see [Measure Steaming Media in Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* For information about custom and solution variables see [Media reports enablement](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>If your licensed solution of Adobe Analytics does not include Video Heartbeat, you must continue using the steps described in this chapter to assign Adobe Analytics variables to Dynamic Media Classic viewer events and variables.
