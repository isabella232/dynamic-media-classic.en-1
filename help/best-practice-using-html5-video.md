---
title: "Best practice: Using the HTML5 Video viewer"
seo-title: "Best practice: Using the HTML5 Video viewer"
description: null
seo-description: Learn about best practices for using the HTML5 video viewer.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
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

|Device|Browser|Video playback mode|
|--- |--- |--- |
|Deskop|Internet Explorer 9 and 10|Progressive download.|
|Desktop|Internet Explorer 11+|HLS video streaming.|
|Desktop|Firefox 23-44|Progressive download.|
|Desktop|Firefox 45 or later|HLS video streaming.|
|Desktop|Chrome|HLS video streaming.|
|Desktop|Safari (Mac)|HLS video streaming.|
|Mobile|Chrome (Android 6 or earlier)|Progressive download.|
|Mobile|Chrome (Android 7 or later)|HLS video streaming.|
|Mobile|Android (Default browser)|Progressive download.|
|Mobile|Safari (iOS)|HLS video streaming.|
|Mobile|Chrome (iOS)|HLS video streaming.|
|Mobile|Blackberry|HLS video streaming.|
