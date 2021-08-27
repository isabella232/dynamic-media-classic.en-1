---
title: Configure Adobe Analytics reports
description: Learn how to configure Adobe Analytics reports in Adobe Dynamic Media Classic.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
---
# Configure Adobe Analytics reports{#configuring-adobe-analytics-reports}

To tell Adobe Analytics what information you want in Adobe Analytics reports, go to the Adobe Analytics Configuration screen. After you configure reports, this screen lists, for each viewer event you want information about, a corresponding Adobe Analytics variable and Adobe Dynamic Media Classic variable. These viewer events-Adobe Analytics variable-Adobe Dynamic Media Classic variable combinations determine what information is reported.

Besides associating viewer events with variables, the Adobe Analytics Configuration screen offers tools for activating, editing, and deleting viewer events.

>[!NOTE]
>
>Whenever you change Adobe Analytics Report settings within Adobe Analytics, be sure you log back on to Adobe Analytics from within Adobe Dynamic Media Classic, resave your Adobe Analytics configuration settings, and then republish.

See [Log in to Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

See [Publish configuration information](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Assign Adobe Analytics variables to Adobe Dynamic Media Classic viewer events and variables {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Use the Adobe Analytics Configuration screen to associate viewer events with Adobe Analytics variables and Adobe Dynamic Media Classic variables. For each viewer event, choose one Adobe Analytics variable and one Adobe Dynamic Media Classic variable. For instructions about opening the Adobe Analytics Configuration screen, see [Log in to Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**To assign Adobe Analytics variables to Adobe Dynamic Media Classic viewer events and variables:**

1. After you log in to Adobe Analytics from within Adobe Dynamic Media Classic and select a report suite, on the Adobe Analytics Configuration page, in the right table column, activate a viewer event by selecting **[!UICONTROL Enable]**.
1. Under the Variables column, display the variable pair chooser by selecting the arrow button for the desired Viewer Event.

   See [Viewer events](configuring-analytics-reports.md#viewer_events).

1. Add an Adobe Dynamic Media Classic variable.

   See [Adobe Dynamic Media Classic variables](configuring-analytics-reports.md#scene7_variables).

1. Add an Adobe Analytics variable.
1. (Optional) To add another variable pair, select **[!UICONTROL Add]**.
1. Select **[!UICONTROL Save]**.

   After you select **[!UICONTROL Save]**, the viewer event, its Adobe Analytics variable, and its Adobe Dynamic Media Classic variable, are listed in the Adobe Analytics Configuration screen.

1. In the lower right corner, select **[!UICONTROL Close]**.
1. Go to **[!UICONTROL Publish]** > **[!UICONTROL Submit Publish]** to run an Image Serving publish.

   Publishing is necessary so that the information contained in the viewers is available on Adobe Dynamic Media Classic servers.

### Viewer events {#viewer-events}

Viewer events describe actions that users perform with Adobe Dynamic Media Classic viewers. When a user initiates a certain action, such as selecting a thumbnail or starting or stopping a video, the viewer “broadcasts” an event to the web page, along with data associated with that event.

The following table describes viewer events you can add to the Adobe Analytics Configuration screen.

|Viewer event|HTML5 Viewer Platform support and viewers|Description|
| --- | --- | --- |
| LOAD | **X** (eCatalog, Flyout, SpinSet, Video, Zoom) | When a user starts a viewer |
| PAGE | **X**  (eCatalog) | In eCatalogs, when a user turns a page; in targeted zoom viewers, when a user selects a different target or a color swatch. |
|SWAP| **X**  (eCatalog, Flyout, SpinSet, Video, Zoom) | When a user selects a different thumbnail to view a different image. |
| ITEM | **X**  (eCatalog) | In viewers that support Image Maps in which rollovers are defined, when a user hovers the pointer over an Image Map to read the rollover text. |
| HREF | **X**  (eCatalog) | In viewers that support Image Maps, when a user selects a URL in an Image Map. |
|TARGET | | In targeted zoom viewers, when a user selects a zoom target to zoom to part of an image. |
| SEARCH | | In eCatalogs, when a user conducts a word search. |
| PLAY | **X**  (Video) | In Video viewers, when a user selects Play to start playing a video.<br><br>**Note:** If you are using Adobe Analytics heartbeat-based video reporting, you do not need to map any variables to this viewer event when you configure Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat works with out-of-the-box Adobe Dynamic Media Classic HTML5 Video and MixedMedia viewers. The video player generates tracking data for viewing within Adobe Analytics Video Reports. See [Enable Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| PAUSE | **X** (Video) | In Video viewers, when a user selects **[!UICONTROL Pause]** to freeze a video.<br><br>**Note:** If you are using Adobe Analytics heartbeat-based video reporting, you do not need to map any variables to this viewer event when you configure Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat works with out-of-the-box Adobe Dynamic Media Classic HTML5 Video and MixedMedia viewers. The video player generates tracking data for viewing within Adobe Analytics Video Reports. See [Enable Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| STOP | **X** (Video) | In Video viewers, when a user selects **[!UICONTROL Stop]** to stop playing a video.<br><br>**Note:** If you are using Adobe Analytics heartbeat-based video reporting, you do not need to map any variables to this viewer event when you configure Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat works with out-of-the-box Adobe Dynamic Media Classic HTML5 Video and MixedMedia viewers. The video player generates tracking data for viewing within Adobe Analytics Video Reports. See [Enable Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| MILESTONE | **X**  (Video) | In Video viewers, milestone events are generated when the user watches 0, 25, 50, 75, or 100 percent of the video.<br><br>**Note:** If you are using Adobe Analytics heartbeat-based video reporting, you do not need to map any variables to this viewer event when you configure Adobe Analytics in Adobe Dynamic Media Classic. Video Heartbeat works with out-of-the-box Adobe Dynamic Media Classic HTML5 Video and MixedMedia viewers. The video player generates tracking data for viewing within Adobe Analytics Video Reports. See [Enable Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| SWATCH | **X** (Flyout, Zoom) | This viewer event is mapped to the PAGE viewer event in Adobe Dynamic Media Classic. |
| ZOOM | **X** (eCatalog, SpinSet, Zoom) | Not tracked by Adobe Analytics. |
| PAN | **X** (eCatalog, SpinSet, Zoom) | Not tracked by Adobe Analytics. |
| SPIN | **X** (SpinSet) | Not tracked by Adobe Analytics. |

### Adobe Dynamic Media Classic variables {#scene-variables}

For each viewer event on Adobe Analytics Configuration screen, choose an Adobe Analytics variable and a *Adobe Dynamic Media Classic variable*. Adobe Dynamic Media Classic variables represent data you can obtain for a report. For example, the `searchTerm` variable lists keywords used in eCatalog searches.

The following table describes Adobe Dynamic Media Classic variables:

|Adobe Dynamic Media Classic variable|Description|
| --- | --- |
|asset | Adobe Dynamic Media Classic asset ID or video path file. |
|viewerId | An arbitrary number that is assigned to each different viewer type. |
|pageLabel | In eCatalogs, the page that a viewer displays. |
|label | The label value (a string). |
|frame | The page or page reference in an Image Set. |
|rollover_keyRaw | The entire HREF value, not just any processed part of it. |
|rollover_keyProc | The ID of an item that is referenced in an Image Map (valid for href and item events). |
|searchTerm | A term that is used in eCatalog search. |
|timeStamp | Play, Stop, and Pause chosen in video viewers. |
|progress | The percentage of a milestone event that is complete. |
|targetId | The id value (a number). |

## Activate, edit, and delete viewer events {#activating-editing-and-deleting-viewer-events}

On the Adobe Analytics Configuration screen, you can activate, edit, and delete viewer events:

* **Activate** - Select **[!UICONTROL Enable]** to activate or **[!UICONTROL Disable]** to deactivate a selected viewer event.

* **Edit** - Select a viewer event and select **[!UICONTROL View/Edit]** Variables gray button. In the Adobe Dynamic Media Classic Variable and Adobe Analytics Variable drop-down lists, choose a different variable from each respective list. For more information, see [Assigning Adobe Analytics variables to Adobe Dynamic Media Classic viewer events and variables](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **Delete** - Select a viewer event, and select **[!UICONTROL View/Edit]** Variables gray button. Select **[!UICONTROL Delete]**.
