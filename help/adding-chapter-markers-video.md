---
title: Adding chapter markers to video
description: Learn how to add chapter markers to a video.
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic,Viewers,Video
role: Business Practitioner
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
---
# Adding chapter markers to video{#adding-chapter-markers-to-video}

You can make your long form videos easier to watch and navigate by adding chapter markers to single videos or to Adaptive Video Sets. When a user plays the video, they can click the chapter markers on the video timeline (also known as the video scrubber) to easily navigate to their point of interest, or immediately jump to new new content, demonstrations, tutorials, and so on.

>[!NOTE]
>
>The video player that is used must support the use of chapter markers.

See [Adding or editing a video viewer preset](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) to configure the chapter navigation cue points and chapter title pop-up text for the `Universal_HTML5_Video` viewer (HTML5).

See also [Adding and editing Viewer Presets](application-setup.md#adding_and_editing_viewer_presets).

You create a chapter list for your video in much the same way that you create captions. That is, you create a WebVTT file. Note, however, that this file must be separate from any WebVTT caption file that you may also be using; you cannot combine captions and chapters into one WebVTT file.

You can use the following sample as an example of the format you use to create a WebVTT file with chapter navigation:

```as3
WEBVTT 
Chapter 1 
00:00.000 --> 01:04.364 
The bicycle store behind it all. 
Chapter 2 
01:04.364 --> 02:00.944 
Creative Cloud. 
Chapter 3 
02:00.944 --> 03:02.937 
Ease of management for a working solution. 
Chapter 4 
03:02.937 --> 03:35.000 
Cost-efficient access to rapidly evolving technology.
```

In the example above, `Chapter 1` is the cue identifier and is optional. The cue time of `00:00:000 --> 01:04:364` specifies the start time and end time of the chapter, in 00:00:000 format. That last three digits are milliseconds and can be left as 000, if preferred. The chapter title of `The bicycle store behind it all` is the actual description of the chapter’s contents. The cue identifier, the starting cue time, and the chapter title all appear in a pop-up in the video player when a user hovers their mouse pointer over a visual cue point in the video’s timeline.

Because you are using an HTML5 video viewer, ensure that the chapter file you create follows the WebVTT (Web Video Text Tracks) standard. The chapter filename extension is .vtt. You can learn more information about the WebVTT captioning standard.

See [WebVTT: The Web Video Text Tracks format](https://dev.w3.org/html5/webvtt/).

**To add chapter markers to video**

1. Using a simple text editor outside Dynamic Media Classic, create your video chapter file.

   >[!NOTE]
   >
   >For global support of video chapters in languages other than English, be aware that the WebVTT standard requires that you create separate .vtt files and calls for each language you want to support.

1. Save the .vtt file in UTF8 encoding to avoid problems with character rendition in the chapter title text.

   Generally, you want to name the chapter VTT file the same name as the video file, and append it with `chapters`. By doing so, it can help you with automating the generation of the video URLs using your existing web content management system.

1. In Dynamic Media Classic, upload your WebVTT chapter file.

   See [Uploading files](uploading-files.md#uploading_files).

1. In the Asset Library panel on the left side, navigate to the asset folder that contains the video file that you want to associate with the chapter file that you uploaded.
1. In the Asset Browse panel, select a single video asset, and then below the thumbnail image of the asset, click **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. In the Viewer List table, find the HTML5 viewer named **Univeral_HTML5_Video**, and then do one of the following:

    * For a pop-up video viewer experience, click **[!UICONTROL Copy URL]** to the far right of the name.

      Append the copied URL of the video with the following syntax to associate it with the copied URL to your caption file:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`
    
    * For an embedded video viewer experience, click **[!UICONTROL Embed Code]** to the far right of the name.

      In the Embed Code dialog box, click **[!UICONTROL Copy to Clipboard]**.

      For the HTML5 `Universal_HTML5_Video` viewer, append the copied embed code with the following:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
