---
title: Add captions to video 
description: Learn how to add captions to video in Adobe Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
---
# Add captions to video {#adding-captions-to-video}

You can extend the reach of your videos to global markets by adding captioning to single videos or to Adaptive Video Sets. By adding captioning you avoid the need to dub the audio, or the need to use native speakers to rerecord the audio for each different language. The video is played in the language that it was recorded. Foreign language subtitles appear so that people of different languages can still understand the audio portion.

Captioning also allows for greater accessibility by using closed captioning for people who are deaf or hard of hearing.

>[!NOTE]
>
>The video player that is used must support the display of captions.

To configure the Caption Effect and to edit the Caption Menu itself, including the menu’s text for any of the following viewers:

* `Universal_HTML5_Video` viewer
* `Universal_HTML5_MixedMedia_dark` viewer
* `Universal_HTML5_MixedMedia_light` viewer

See [Add or edit a video viewer preset](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

See also [Add and edit Viewer Presets](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic can convert caption files to JSON (JavaScript Object Notation) format. This conversion means you can embed the JSON text into a web page as a hidden but complete transcript of the video. Search engines can then crawl and index the content to make the videos more easily discoverable and give customers more details about the video content.

See [Serve static (non-image) contents](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) in the *Adobe Image Serving API Help* for more information about using the JSON function in a URL.

**To add captions to video:**

1. Using a third-party application outside Adobe Dynamic Media Classic, create your video caption file based on the viewer type that you are using.

   |Viewer type|Captioning file|
   |--- |--- |
   |HTML5|If you are using an HTML5 video viewer, ensure that the caption file you create follows the WebVTT (Web Video Text Tracks) standard. The captioning filename extension is .vtt. You can learn more information about the WebVTT captioning standard.<br><br>[See WebVTT](https://w3c.github.io/webvtt/): The Web Video Text Tracks format. <br><br>There are both free and paid for tools and services that you can use to author caption files outside Adobe Dynamic Media Classic. For example, to create a simple video caption file with no styling, you can use the following free online caption authoring and editing tool: <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>For best results, use the tool in Internet Explorer 9 or above, Google Chrome, or Safari. <br><br>In the tool, in the <b>Enter URL of video file</b> field, paste the URL of your video file and then select <b>Load</b>. <br><br>For example, if you are using an Adobe Dynamic Media Classic URL for your video file, double-click an individual video asset (not an Adaptive Video Set or a Master Video) to open it in Detail View. In the right panel of the Detail View, expand URLs and Embed Code. Then under the Mobile group, to the right of Mobile (Progressive), select <b>Copy URL</b>. This process gives you the URL to the video file itself which you can then paste into the <b>Enter URL of video file</b> field. Internet Explorer, Chrome, or Safari can then natively play back the video. Now follow the onscreen instructions from the site to author and save your WebVTT file. When you have finished, copy the caption file contents and paste it into a plain text editor and save it with a VTT filename extension. <br><br><b>Note:</b> For global support of video captions in languages other than English, the WebVTT standard requires that you create separate .vtt files and calls for each language you want to support. <br><br>Generally, you want to name the caption VTT file the same name as the video file, and append it with captions. By doing so, it can help you with automating the generation of the video URLs using your existing web content management system.|

1. In Adobe Dynamic Media Classic, upload your WebVTT, DFXP, or SMPTE XML caption file.

   See [Upload files](uploading-files.md#uploading_files).

1. In the Asset Library panel on the left side, navigate to the asset folder that contains the video file that you want to associate with the caption file that you uploaded.
1. In the Asset Browse panel, select a single video asset, and then below the thumbnail image of the asset, select **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
1. In the Viewer List table, find the HTML5 viewer named **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark**, or **Universal_HTML5_MixedMedia_light**, then do one of the following:

    * For a pop-up video viewer experience, select **[!UICONTROL Copy URL]** to the far right of the name.

      Append the copied URL of the video with the following syntax so you can associate it with the copied URL to your caption file:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Note the `,1` at the end of the caption URL path. Immediately following the VTT filename extension in the path, you can optionally enable or disable the closed caption button on the video player bar by setting to `1` or `0`, respectively.
    
    * For an embedded video viewer experience, select **[!UICONTROL Embed Code]** to the far right of the name.

      In the Embed Code dialog box, select **[!UICONTROL Copy to Clipboard]**.

      For the HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`, or `Universal_HTML5_MixedMedia_light` viewers, append the copied embed code with the following:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Note the `,1` at the end of the URL path. Immediately following the VTT filename extension in the URL path, you can optionally enable or disable the caption button on the video player bar by setting to `1` or `0`, respectively.
