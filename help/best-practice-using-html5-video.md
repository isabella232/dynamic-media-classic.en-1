---
title: "Best practice: Using the HTML5 Video viewer"
seo-title: "Best practice: Using the HTML5 Video viewer"
description: null
seo-description: Learn about best practices for using the HTML5 video viewer.
uuid: 43ba93a4-a88b-43c8-9f44-5246ddb1093a
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WSeb9554d1a38d8f24-72833989143d5718892-8000,scene7/using/WSeb9554d1a38d8f24-72833989143d5718892-7fff
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: c70f0a27-e2a8-46a2-a97d-f91bd89b097f
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 42.342-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/video;/content/help/en/experience-manager/morehelp/video
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Best practice: Using the HTML5 Video viewer{#best-practice-using-the-html-video-viewer}

The Scene7 HTML5 Video viewer presets are robust video players. On the design side of the player, you can create all of the video player’s functionality using standard web development tools. For example, you can design the buttons, controls, and custom poster image background using HTML5 and CSS to help you reach your customers with a customized appearance.

On the playback side of the viewer, it automatically detects the browser’s video capability. It then serves the video using HLS (adaptive video streaming). Or, if that delivery method is not present then HTML5 progressive is used instead.

By combining into a single player the ability to design the playback components using HTML5 and CSS, have embedded playback, and use adaptive and progressive streaming depending on the browser’s capability, you extend the reach of your rich media content to both desktop and mobile users and ensure a streamlined video experience.

See also [About HTML5 Viewers](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) in the Adobe Scene7 Viewers Reference Guide.

## Playback of video on desktop computers and mobile devices using the Scene7 Video Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

For desktop and mobile adaptive video streaming, the videos used for bit rate switching are based on all MP4 videos in the Adaptive Video Set.

Video playback occurs using either HLS or progressive video. HLS (HTTP Live Streaming) is an Apple standard for adaptive video streaming that automatically adjusts playback based on network bandwidth capacity. It also lets the customer “seek” to any point in the video without the need to wait for the rest of the video to download (see also [HTTP Live Streaming](#UnresolvedLink-https://developer.apple.com/streaming/)). Progressive video is delivered by downloading and storing the video locally to a user’s desktop screen or mobile device.

The following table describes the device, browser, and playback method of videos on desktop computers and mobile devices using the Scene7 Video Viewer.

<table border="1" cellpadding="4" cellspacing="0" frame="border" rules="all" summary="">
 <thead align="left">
  <tr>
   <th class="cellrowborder" id="d19e22507" valign="top" width="NaN%"><p>Device</p></th> 
   <th class="cellrowborder" id="d19e22510" valign="top" width="NaN%"><p>Browser</p></th> 
   <th class="cellrowborder" id="d19e22513" valign="top" width="NaN%"><p>Video playback mode</p></th> 
  </tr> 
 </thead> 
 <tbody>
  <tr>
   <td class="cellrowborder" headers="d19e22507 " valign="top" width="NaN%"><p>Deskop</p></td> 
   <td class="cellrowborder" headers="d19e22510 " valign="top" width="NaN%"><p>Internet Explorer 9 and 10</p></td> 
   <td class="cellrowborder" headers="d19e22513 " valign="top" width="NaN%"><p>Progressive download.</p></td> 
  </tr> 
  <tr>
   <td class="cellrowborder" headers="d19e22507 " valign="top" width="NaN%"><p>Desktop</p></td> 
   <td class="cellrowborder" headers="d19e22510 " valign="top" width="NaN%"><p>Internet Explorer 11+</p></td> 
   <td class="cellrowborder" headers="d19e22513 " valign="top" width="NaN%"><p>HLS video streaming.</p></td> 
  </tr> 
  <tr>
   <td class="cellrowborder" headers="d19e22507 " valign="top" width="NaN%"><p>Desktop</p></td> 
   <td class="cellrowborder" headers="d19e22510 " valign="top" width="NaN%"><p>Firefox 23-44</p></td> 
   <td class="cellrowborder" headers="d19e22513 " valign="top" width="NaN%"><p>Progressive download.</p></td> 
  </tr> 
  <tr>
   <td class="cellrowborder" headers="d19e22507 " valign="top" width="NaN%"><p>Desktop</p></td> 
   <td class="cellrowborder" headers="d19e22510 " valign="top" width="NaN%"><p>Firefox 45 or later</p></td> 
   <td class="cellrowborder" headers="d19e22513 " valign="top" width="NaN%"><p>HLS video streaming.</p></td> 
  </tr> 
  <tr>
   <td class="cellrowborder" headers="d19e22507 " valign="top" width="NaN%"><p>Desktop</p></td> 
   <td class="cellrowborder" headers="d19e22510 " valign="top" width="NaN%"><p>Chrome</p></td> 
   <td class="cellrowborder" headers="d19e22513 " valign="top" width="NaN%"><p>HLS video streaming.</p></td> 
  </tr> 
  <tr>
   <td class="cellrowborder" headers="d19e22507 " valign="top" width="NaN%"><p>Desktop</p></td> 
   <td class="cellrowborder" headers="d19e22510 " valign="top" width="NaN%"><p>Safari (Mac)</p></td> 
   <td class="cellrowborder" headers="d19e22513 " valign="top" width="NaN%"><p>HLS video streaming.</p></td> 
  </tr> 
  <tr>
   <td class="cellrowborder" headers="d19e22507 " valign="top" width="NaN%"><p>Mobile</p></td> 
   <td class="cellrowborder" headers="d19e22510 " valign="top" width="NaN%"><p>Chrome (Android 6 or earlier)</p></td> 
   <td class="cellrowborder" headers="d19e22513 " valign="top" width="NaN%"><p>Progressive download.</p></td> 
  </tr> 
  <tr>
   <td class="cellrowborder" headers="d19e22507 " valign="top" width="NaN%"><p>Mobile</p></td> 
   <td class="cellrowborder" headers="d19e22510 " valign="top" width="NaN%"><p>Chrome (Android 7 or later)</p></td> 
   <td class="cellrowborder" headers="d19e22513 " valign="top" width="NaN%"><p>HLS video streaming.</p></td> 
  </tr> 
  <tr>
   <td class="cellrowborder" headers="d19e22507 " valign="top" width="NaN%"><p>Mobile</p></td> 
   <td class="cellrowborder" headers="d19e22510 " valign="top" width="NaN%"><p>Android (Default browser)</p></td> 
   <td class="cellrowborder" headers="d19e22513 " valign="top" width="NaN%"><p>Progressive download.</p></td> 
  </tr> 
  <tr>
   <td class="cellrowborder" headers="d19e22507 " valign="top" width="NaN%"><p>Mobile</p></td> 
   <td class="cellrowborder" headers="d19e22510 " valign="top" width="NaN%"><p>Safari (iOS)</p></td> 
   <td class="cellrowborder" headers="d19e22513 " valign="top" width="NaN%"><p>HLS video streaming.</p></td> 
  </tr> 
  <tr>
   <td class="cellrowborder" headers="d19e22507 " valign="top" width="NaN%"><p>Mobile</p></td> 
   <td class="cellrowborder" headers="d19e22510 " valign="top" width="NaN%"><p>Chrome (iOS)</p></td> 
   <td class="cellrowborder" headers="d19e22513 " valign="top" width="NaN%"><p>HLS video streaming.</p></td> 
  </tr> 
  <tr>
   <td class="cellrowborder" headers="d19e22507 " valign="top" width="NaN%"><p>Mobile</p></td> 
   <td class="cellrowborder" headers="d19e22510 " valign="top" width="NaN%"><p>Blackberry</p></td> 
   <td class="cellrowborder" headers="d19e22513 " valign="top" width="NaN%"><p>HLS video streaming.</p></td> 
  </tr> 
 </tbody> 
</table>

