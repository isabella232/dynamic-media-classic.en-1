---
title: Configuring Adobe Analytics reports
seo-title: Configuring Adobe Analytics reports
description: null
seo-description: Learn how to configure Adobe Analytics reports.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
index: y
internal: n
snippet: y
---

# Configuring Adobe Analytics reports{#configuring-adobe-analytics-reports}

To tell Adobe Analytics what information you want in Adobe Analytics reports, go to the Adobe Analytics Configuration screen. After you configure reports, this screen lists, for each viewer event you want information about, a corresponding Adobe Analytics variable and Scene7 variable. These viewer events-Adobe Analytics variable-Scene7 variable combinations determine what information is reported.

As well as associating viewer events with variables, the Adobe Analytics Configuration screen offers tools for activating, editing, and deleting viewer events.

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Added Important note below plus xrefs, 10/3/2012.</p>

 -->

>[!NOTE]
>
>Whenever you change Adobe Analytics Report settings within Adobe Analytics, be sure you log back on to Adobe Analytics from within Adobe Scene7 Publishing System, re-save your Adobe Analytics configuration settings, and then re-publish.

See [Log in to Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

See [Publishing configuration information](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Assigning Adobe Analytics variables to Scene7 viewer events and variables {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Use the Adobe Analytics Configuration screen to associate viewer events with Adobe Analytics variables and Scene7 variables. For each viewer event, choose one Adobe Analytics variable and one Scene7 variable. For instructions about opening the Adobe Analytics Configuration screen, see [Log in to Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**To assign Adobe Analytics variables to Scene7 viewer events and variables**

1. After you log in to Adobe Analytics from within Scene7 and select a report suite, on the Adobe Analytics Configuration page, in the far right column of the table, activate a viewer event by clicking **Enable**.
1. Under the Variables column, display the variable pair chooser by clicking the arrow button for the desired Viewer Event.

   See [Viewer events](configuring-analytics-reports.md#viewer_events).

1. Add a Scene7 variable.

   See [Scene7 variables](configuring-analytics-reports.md#scene7_variables).

1. Add an Adobe Analytics variable.
1. (Optional) To add another variable pair, click **Add**.
1. Click **Save**.

   After you click Save, the viewer event, its Adobe Analytics variable, and its Scene7 variable, are listed in the Adobe Analytics Configuration screen. 

1. In the lower right corner, click **Close**.
1. Click **Publish** &gt; **Submit Publish** to run an Image Serving publish.

   Publishing is necessary so that the information contained in the viewers is available on Scene7 servers.

### Viewer events {#viewer-events}

Viewer events describe actions that users perform with Scene7 viewers. When a user initiates a certain action, such as clicking on a thumbnail or starting or stopping a video, the viewer “broadcasts” an event to the web page, along with data associated with that event.

The following table describes viewer events you can add to the Adobe Analytics Configuration screen.

<table> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e26526" valign="top" width="NaN%"><p>Viewer event</p></th> 
   <th class="cellrowborder" id="d19e26529" valign="top" width="NaN%"><p>HTML5 Viewer Platform support and viewers</p></th> 
   <th class="cellrowborder" id="d19e26532" valign="top" width="NaN%"><p>Description</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>LOAD</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p><strong>X</strong> (eCatalog, Flyout, SpinSet, Video, Zoom)</p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>When a user starts the viewer.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>PAGE</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p><strong>X</strong> (eCatalog)</p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>In eCatalogs, when a user turns a page; in targeted zoom viewers, when a user clicks a different target or a color swatch.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>SWAP</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p><strong>X</strong> (eCatalog, Flyout, SpinSet, Video, Zoom)</p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>When a user clicks a different thumbnail to view a different image.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>ITEM</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p><strong>X</strong> (eCatalog)</p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>In viewers that support Image Maps in which rollovers are defined, when a user hovers the pointer over an Image Map to read the rollover text. </p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>HREF</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p><strong>X</strong> (eCatalog)</p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>In viewers that support Image Maps, when a user clicks a URL in an Image Map.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>TARGET</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p></p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>In targeted zoom viewers, when a user clicks a zoom target to zoom to part of an image.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>SEARCH</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p></p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>In eCatalogs, when a user conducts a word search.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>PLAY</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p><strong>X</strong> (Video)</p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>In Video viewers, when a user clicks Play to start playing a video.</p><p><i><strong>note</strong>: If you are using Adobe Analytics heartbeat-based video reporting, you do not need to map any variables to this viewer event when you configure Adobe Analytics in Scene7. Video Heartbeat works with out-of-the-box Scene7 HTML5 Video and MixedMedia viewers. The video player generates tracking data for viewing within Adobe Analytics Video Reports. See <a href="enabling-analytics-video-reports.md#enabling_adobe_analytics_video_reports">Enabling Adobe Analytics Video Reports</a>.</i></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>PAUSE</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p><strong>X</strong> (Video)</p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>In Video viewers, when a user clicks Pause to pause a video.</p><p><i><strong>note</strong>: If you are using Adobe Analytics heartbeat-based video reporting, you do not need to map any variables to this viewer event when you configure Adobe Analytics in Scene7. Video Heartbeat works with out-of-the-box Scene7 HTML5 Video and MixedMedia viewers. The video player generates tracking data for viewing within Adobe Analytics Video Reports. See <a href="enabling-analytics-video-reports.md#enabling_adobe_analytics_video_reports">Enabling Adobe Analytics Video Reports</a>.</i></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>STOP</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p><strong>X</strong> (Video)</p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>In Video viewers, when a user clicks Stop to stop playing a video.</p><p><i><strong>note</strong>: For the HTML5 viewer platform, this viewer event is only available for custom HTML5 Viewers that you have created using the Adobe Scene7 HTML5 Viewer SDK.</i></p><p><i><strong>note</strong>: If you are using Adobe Analytics heartbeat-based video reporting, you do not need to map any variables to this viewer event when you configure Adobe Analytics in Scene7. Video Heartbeat works with out-of-the-box Scene7 HTML5 Video and MixedMedia viewers. The video player generates tracking data for viewing within Adobe Analytics Video Reports. See <a href="enabling-analytics-video-reports.md#enabling_adobe_analytics_video_reports">Enabling Adobe Analytics Video Reports</a>.</i></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>MILESTONE</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p><strong>X</strong> (Video)</p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>In Video viewers, milestone events are generated when the user watches 0, 25, 50, 75, or 100 percent of the video.</p><p><i><strong>note</strong>: If you are using Adobe Analytics heartbeat-based video reporting, you do not need to map any variables to this viewer event when you configure Adobe Analytics in Scene7. Video Heartbeat works with out-of-the-box Scene7 HTML5 Video and MixedMedia viewers. The video player generates tracking data for viewing within Adobe Analytics Video Reports. See <a href="enabling-analytics-video-reports.md#enabling_adobe_analytics_video_reports">Enabling Adobe Analytics Video Reports</a>.</i></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>SWATCH</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p><strong>X</strong> (Flyout, Zoom) </p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>This viewer event is mapped to the PAGE viewer event in Scene7 Publishing System.</p><p><i><strong>note</strong>: This HTML5 platform viewer event is only available for custom HTML5 Viewers that you have created using the Adobe Scene7 HTML5 Viewer SDK.</i></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>ZOOM</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p><strong>X</strong> (eCatalog, SpinSet, Zoom)</p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>Not tracked by Adobe Analytics.</p><p><i><strong>note</strong>: This HTML5 platform viewer event is only available for custom HTML5 Viewers that you have created using the Adobe Scene7 HTML5 Viewer SDK.</i></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>PAN</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p><strong>X</strong> (eCatalog, SpinSet, Zoom)</p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>Not tracked by Adobe Analytics.</p><p><i><strong>note</strong>: This HTML5 platform viewer event is only available for custom HTML5 Viewers that you have created using the Adobe Scene7 HTML5 Viewer SDK.</i></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e26526 " valign="top" width="NaN%"><p>SPIN</p></td> 
   <td class="cellrowborder" headers="d19e26529 " valign="top" width="NaN%"><p><strong>X</strong> (SpinSet)</p></td> 
   <td class="cellrowborder" headers="d19e26532 " valign="top" width="NaN%"><p>Not tracked by Adobe Analytics.</p><p><i><strong>note</strong>: This HTML5 platform viewer event is only available for custom HTML5 Viewers that you have created using the Adobe Scene7 HTML5 Viewer SDK.</i></p></td> 
  </tr> 
 </tbody> 
</table>

### Scene7 variables {#scene-variables}

For each viewer event on Adobe Analytics Configuration screen, choose a Adobe Analytics variable and a *Scene7 variable*. Scene7 variables represent data you can obtain for a report. For example, the `searchTerm` variable lists keywords used in eCatalog searches.

The following table describes Scene7 variables.

|Scene7 variable|Description|
|--- |:--- |
|asset|Scene7 Publishing System asset ID or video path file.|
|viewerId|An arbitrary number that is assigned to each different viewer type.|
|pageLabel|In eCatalogs, the page that a viewer displays.|
|label|The label value (a string).|
|frame|The page or page reference in an Image Set.|
|rollover_keyRaw|The entire HREF value, not just any processed part of it.|
|rollover_keyProc|The ID of an item that is referenced in an Image Map (valid for href and item events).|
|searchTerm|A term that is used in eCatalog search.|
|timeStamp|Play, Stop, and Pause chosen in video viewers.|
|progress|The percentage of a milestone event that is complete.|
|targetId|The id value (a number).|

## Activating, editing, and deleting viewer events {#activating-editing-and-deleting-viewer-events}

On the Adobe Analytics Configuration screen, you can activate, edit, and delete viewer events:

**Activating** Click Enable to activate or Disable to deactivate a selected viewer event.

**Editing** Select a viewer event and click View/Edit Variables grey button. In the Scene7 Variable and Adobe Analytics Variable drop-down lists, choose a different variable from each respective list. For more information, see Assigning Adobe Analytics variables to Scene7 viewer events and variables.

**Deleting** Select a viewer event, and click View/Edit Variables grey button. Click Delete.
