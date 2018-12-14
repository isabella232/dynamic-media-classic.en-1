---
title: Enabling Adobe Analytics Video Reports
seo-title: Enabling Adobe Analytics Video Reports
description: null
seo-description: Learn how to enable Adobe Analytics video reports.
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
index: y
internal: n
snippet: y
---

# Enabling Adobe Analytics Video Reports{#enabling-adobe-analytics-video-reports}

Using Adobe Analytics heartbeat-based video reporting, you no longer need to enable the four video viewer events (Play, Pause, Stop, Milestone) when you configure Adobe Analytics in Scene7. Video Heartbeat works with out-of-the-box Scene7 HTML5 Video and MixedMedia viewers. The video player generates tracking data for viewing within Adobe Analytics Video Reports.

* The integration of Adobe Analytics video reports with Scene7 supports solution variables, but not custom variables.

  See [Configure Analytics Video Reporting](http://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) for more information about solution variables and custom variables.

* Out-of-the-box segments of one minute increments is supported. However, custom segment reporting, such as customer-defined milestones based on time increments, % milestone, or offset milestones, is not supported.

For more information about Video Heartbeat requirements and setup, see [Measuring Video in Adobe Analytics using Video Heartbeat](http://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

If you are customizing your own viewer and want to use Video Heartbeat, see *Enabling Adobe Analytics Video Reports* in the Adobe Scene7 HTML5 Viewer SDK available for download through Adobe Developer Connection at [www.adobe.com/go/learn/learn_s7_devresources_en](http://www.adobe.com/go/learn/learn_s7_devresources_en).

>[!NOTE]
>
>If your licensed solution of Adobe Analytics does not include Video Heartbeat, you will need to continue using the steps described in this chapter to assign Adobe Analytics variables to Scene7 viewer events and variables.

