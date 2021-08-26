---
title: Deploy video to your websites and mobile sites
description: Learn how to deploy video to your websites and mobile sites from Adobe Dynamic Media Classic.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
---
# Deploy video to your websites and mobile sites{#deploying-video-to-your-websites-and-mobile-sites}

Websites, mobile sites, and desktop applications access Adobe Dynamic Media Classic server content, including video, by using URL strings or embedded code. Adobe Dynamic Media Classic activates these URL strings during the publishing process. To place the URL string or embed code for your video in your web pages, mobile pages, and desktop applications, copy it from Adobe Dynamic Media Classic.

>[!NOTE]
>
>The URL or embed code is not active until you publish the asset.

## Publish video {#publishing-video}

Publishing a video enables Adobe Dynamic Media Classic Servers to deliver video to your website, mobile site, or application.

There are two different methods you can use to publish video:

* **Publish videos automatically and instantly on upload** - As part of the video upload process, Adobe Dynamic Media Classic can automatically publish videos when they are uploaded and encoded. This ability to instantly publish means that there is no need to publish videos separately after the fact.

* **Publish video manually after upload** - If you do not want to publish videos immediately, you can manually publish videos at any time.

After you publish videos, Adobe Dynamic Media Classic activates the URL strings for your HTML page or application code.

**To publish video:**

1. Do one of the following:

    * To publish videos automatically and instantly on upload, in the Upload page, select **[!UICONTROL Publish after uploading]**. You have finished; there are no further steps to complete.
    * To publish videos manually after upload, in the Browse Panel, select the videos, and then on the Global Navigation bar, select **Publish**.

## Link a video URL to a mobile site or a website {#linking-a-video-url-to-a-mobile-site-or-a-website}

After you publish a video, you can obtain its URL for use in your website, mobile site, or desktop application. Use the video URL when you want to display video in a pop-up or modal window on top of the web page.

When a customer selects the link, their device, bandwidth, and screen size are automatically detected. The appropriate video is displayed for playback in a pre-defined viewer for desktop, or in the mobile device's native video player for smartphones and tablets.

See also [Embed the video viewer on a web page](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**To link a video URL to a mobile site or a website:**

1. In the Asset Browse panel, in the **[!UICONTROL Show]** drop-down list, select **[!UICONTROL Video]** or **[!UICONTROL Adaptive Video Set]**.
1. in the Asset Library panel on the left side, navigate to the asset folder that contains the video or adaptive video set you want to link.
1. Above the Asset Browse panel, on the right side of the toolbar, do one of the following:

    * Select **[!UICONTROL Grid View]** or **[!UICONTROL List View]**. In the Asset Browse panel, double-click the video thumbnail of a single asset to open it in Detail View. In the URLs and Embed Code panel on the right, under HTTP Streaming, select **[!UICONTROL Copy URL]** to the right of the viewer you want. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.
    * Select **[!UICONTROL Grid View]**. In the Asset Browse panel, select a single asset, and then below the thumbnail image, go to **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      In the Viewer List page, under the Actions column of the table, select **[!UICONTROL Copy URL]**. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

    * Select **[!UICONTROL List View]**. In the Asset Browse panel, select a single asset, and then to the right of the thumbnail image, go to **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      In the Viewer List page, under the Actions column of the table, select **[!UICONTROL Copy URL]**. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

    * Select **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, or **[!UICONTROL Detail View]**. On the same toolbar, go to **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      In the Viewer List page, under the Actions column of the table, select **[!UICONTROL Copy URL]**. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

1. Paste the HTML5 video URL link on your website and mobile site.

## Embed the video viewer on a web page {#embedding-the-video-viewer-on-a-web-page}

Use the Embed Code feature when you want to play the video embedded on the web page. You copy the embed code to the clipboard so you can paste it in your web pages. Editing of the code is not permitted in the Embed Code dialog box.

See also [Link a video URL to a mobile site or a website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**To embed the video viewer on a web page:**

1. In the Asset Browse panel, in the Show drop-down list, select **[!UICONTROL Video]** or **[!UICONTROL Adaptive Video Set]**.
1. in the Asset Library panel on the left side, navigate to the asset folder that contains the video or adaptive video set whose embed code you want to copy.
1. Above the Asset Browse panel, on the right side of the toolbar, do one of the following:

    * Select **[!UICONTROL Grid View]** or **[!UICONTROL List View]**. In the Asset Browse panel, double-click the video thumbnail of a single asset to open it in Detail View. In the URLs and Embed Code panel on the right, under HTTP Streaming, select **[!UICONTROL Embed Code]** to the right of the viewer you want. As a best practice, select **[!UICONTROL Embed Code]** that is associated with the `Universal_HTML5_Video` viewer.
    * Select **[!UICONTROL Grid View]**. In the Asset Browse panel, select a single asset, and then below the video thumbnail image, select **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      In the Viewer List page, under the Actions column of the table, select **[!UICONTROL Embed Code]**. As a best practice, select **[!UICONTROL Embed Code]** that is associated with the `Universal_HTML5_Video` viewer.

    * Select **[!UICONTROL List View]**. In the Asset Browse panel, select a single asset, and then to the right of the thumbnail image, go to **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      In the Viewer List page, under the Actions column of the table, select **[!UICONTROL Embed Code]**. As a best practice, select **[!UICONTROL Embed Code]** that is associated with the `Universal_HTML5_Video` viewer.

    * Select **[!UICONTROL Grid View]**, **[!UICONTROL List View]**, or **[!UICONTROL Detail View]**. On the same toolbar, go to **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

      In the Viewer List page, under the Actions column of the table, select **[!UICONTROL Embed Code]**. As a best practice, select **[!UICONTROL Embed Code]** that is associated with the `Universal_HTML5_Video` viewer.

1. In the Embed Code dialog box, select **[!UICONTROL Copy to Clipboard]**.

   Editing the code is not permitted in the Embed Code dialog box.

1. select **[!UICONTROL Close]**.
1. Paste the embed code in your web pages.

### Implement embed code for using HTML5 video with MP4 video assets {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

If you do not use the Adobe Dynamic Media Classic HTML5 video player, but instead want to use the native HTML5 `<video>` tag with MP4 video assets, you can use the following embed code sample:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Replace `"S7 video thumbnail URL"` with the video’s thumbnail URL which is the video’s thumbnail image that a user sees before they play the video.

  See [Obtain video thumbnail URLs](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Replace `"S7 OGG video asset URL (no player)"` with the video’s progressive URL for OGG video.

  See [Link a video URL to a mobile site or a website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Replace `"S7 MP4 mobile progressive video asset URL (no player)"` with the video’s mobile progressive URL.

  See [Link a video URL to a mobile site or a website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Deploy video using a third-party video player {#deploying-video-using-a-third-party-video-player}

If you use a third-party video player or a custom-built video player instead of a Adobe Dynamic Media Classic video viewer, you obtain the direct video URL that works for HLS multi-bitrate video streaming or progressive download.

**To deploy video using a third-party video player:**

1. In Adobe Dynamic Media Classic, on the Global Navigation bar, go to **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]**.
1. Depending on the type of URL you want to use, do one of the following tasks:

* To generate a direct HLS streaming video URL (multi-bitrate)

  On the **[!UICONTROL Application General Settings]** page, in the **[!UICONTROL Servers]** group, in the **[!UICONTROL Published Server Name]** text field, construct the direct URL. Use the following syntax: `server/is/content/company/folder/filename.m3u8`
  
  For example, suppose that the Published server name is `https://s7d9.scene7.com/.` Using the syntax in step 2, the direct URL could look like the following:
  `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* To generate a direct HLS streaming video URL (single bit rate)

  On the **[!UICONTROL Application General Settings]** page, in the **[!UICONTROL Servers]** group, in the **[!UICONTROL HLS Streaming Server Name]** text field, construct the direct URL using the following syntax:

  `server/company/folder/filename.ext.m3u8`
  
  For example, suppose that the HLS streaming server name is `https://s7mbrstream.scene7.com/hls-vod/`. Using the syntax in step 2, the direct URL could look like the following:
  `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* To generate a direct progressive video URL

  On the **[!UICONTROL Application General Settings]** page, in the **[!UICONTROL Servers]** group, in the **[!UICONTROL Progressive Video Server Name]** text field, construct the direct eVideo URL using the following syntax:
  
  `server/company/folder/filename`
  
  For example, suppose that the progressive video server name is `https://s7d9.scene7.com/is/content/`. Using the syntax in step 2, the direct URL could look like the following:
  `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Work with video thumbnails {#working-with-video-thumbnails}

Adobe Dynamic Media Classic generates thumbnails for encoded videos, and pre-encoded videos. You can use video thumbnails like any image asset. Moreover, you can obtain URLs for the video thumbnails that Adobe Dynamic Media Classic generates and deploy these URLs outside Adobe Dynamic Media Classic. For example, you can deploy the thumbnails in search results, related video listings, and video play lists on a website.

Thumbnails are generated based on the first heterogeneous frame (not an all black frame, or an all white frame, and so forth) of the video.

### Obtain video thumbnail URLs {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic generates video thumbnails automatically during the upload process. The thumbnails appear in the Browse panel in List View and Grid View.

To generate URLs for video thumbnails, perform a publish operation.

See [Publish video](deploying-video-websites-mobile-sites.md#publishing_video).

After publishing, you can obtain video thumbnail URLs in Detail View in the URLs and Embed Code panel. Select **[!UICONTROL Copy URL]** to the right of the video thumbnail so you can copy its URL.

### Modify poster frames in video viewers {#modifying-poster-frames-in-video-viewers}

The *poster frame* is the initial frame that appears in Video viewers before the video begins playing. Adobe Dynamic Media Classic uses video thumbnails as poster frames.

You can apply image modifiers to the poster frame. For example, you can crop the poster frame or make it transparent. To modify the poster frame, open the video viewer configuration screen and enter modifiers in the Poster Image Modifiers section.

See [Add or edit a video viewer preset](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

See [Image Serving Guide](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api).

You can also modify video thumbnails by appending modifiers to video thumbnail URLs.

>[!MORELIKETHIS]
>
>* [Publish files](publishing-files.md#publishing_files)