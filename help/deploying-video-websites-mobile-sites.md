---
title: Deploying video to your websites and mobile sites
seo-title: Deploying video to your websites and mobile sites
description: null
seo-description: Learn how to deploy video to your websites and mobile sites.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
index: y
internal: n
snippet: y
---

# Deploying video to your websites and mobile sites{#deploying-video-to-your-websites-and-mobile-sites}

Websites, mobile sites, and desktop applications access Scene7 server content, including video, by using URL strings or embedded code. Scene7 activates these URL strings during the publishing process. To place the URL string or embed code for your video in your web pages, mobile pages, and desktop applications, copy it from the Scene7 Publishing System.

>[!NOTE]
>
>The URL or embed code is not active until you publish the asset.

## Publishing video {#publishing-video}

Publishing a video enables Scene7 Servers to deliver video to your website, mobile site, or application.

There are two different methods you can use to publish video:

* **Publish videos automatically and instantly on upload**

  As part of the video upload process, Scene7 can automatically publish videos when they are uploaded and encoded. This ability to instantly publish means that there is no need to publish videos separately after the fact.

* **Publish video manually after upload**

  If you do not want to publish videos immediately, you can manually publish videos at any time.

After you publish videos, the Scene7 Publishing System activates the URL strings for your HTML page or application code.

**To publish video**

1. Do one of the following:

    * To publish videos automatically and instantly on upload, in the Upload screen, click **Publish after uploading**. You have finished; there are no further steps to complete.
    * To publish videos manually after upload, in the Browse Panel, select the videos, and then on the Global Navigation bar, click **Publish**.

## Linking a video URL to a mobile site or a website {#linking-a-video-url-to-a-mobile-site-or-a-website}

After you publish a video, you can obtain its URL for use in your website, mobile site, or desktop application. Use the video URL when you want to display video in a pop-up or modal window on top of the web page.

When a customer clicks the link, their device, bandwidth, and screen size are automatically detected. The appropriate video is displayed for playback in a pre-defined viewer for desktop, or in the mobile device's native video player for smartphones and tablets.

See also [Embedding the video viewer on a web page](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**To link a video URL to a mobile site or a website**

1. In the Asset Browse panel, in the Show drop-down list, click **Video** or **Adaptive Video Set**.
1. in the Asset Library panel on the left side, navigate to the asset folder that contains the video or adaptive video set you want to link.
1. Above the Asset Browse panel, on the right side of the toolbar, do one of the following:

    * Click **Grid View** or **List View**. In the Asset Browse panel, double-click the video thumbnail of a single asset to open it in Detail View. In the URLs and Embed Code panel on the right, under HTTP Streaming, click **Copy URL** to the right of the viewer you want. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.
    * Click **Grid View**. In the Asset Browse panel, select a single asset, and then below the thumbnail image, click **Preview** &gt; **Viewer List**.

      In the Viewer List page, under the Actions column of the table, click **Copy URL**. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.
    
    * Click **List View**. In the Asset Browse panel, select a single asset, and then to the right of the thumbnail image, click **Preview** &gt; **Viewer List**.

      In the Viewer List page, under the Actions column of the table, click **Copy URL**. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.
    
    * Click **Grid View**, **List View**, or **Detail View**. On the same toolbar, click **Preview** &gt; **Viewer List**.

      In the Viewer List page, under the Actions column of the table, click **Copy URL**. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

1. Paste the HTML5 video URL link on your website and mobile site.

## Embedding the video viewer on a web page {#embedding-the-video-viewer-on-a-web-page}

Use the Embed Code feature when you want to play the video embedded on the web page. You copy the embed code to the clipboard so you can paste it in your web pages. Editing of the code is not permitted in the Embed Code dialog box.

See also [Linking a video URL to a mobile site or a website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**To embed the video viewer on a web page**

1. In the Asset Browse panel, in the Show drop-down list, click **Video** or **Adaptive Video Set**.
1. in the Asset Library panel on the left side, navigate to the asset folder that contains the video or adaptive video set whose embed code you want to copy.
1. Above the Asset Browse panel, on the right side of the toolbar, do one of the following:

    * Click **Grid View** or **List View**. In the Asset Browse panel, double-click the video thumbnail of a single asset to open it in Detail View. In the URLs and Embed Code panel on the right, under HTTP Streaming, click **Embed Code** to the right of the viewer you want. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.
    * Click **Grid View**. In the Asset Browse panel, select a single asset, and then below the video thumbnail image, click **Preview** &gt; **Viewer List**.

      In the Viewer List page, under the Actions column of the table, click **Embed Code**. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.
    
    * Click **List View**. In the Asset Browse panel, select a single asset, and then to the right of the thumbnail image, click **Preview** &gt; **Viewer List**.

      In the Viewer List page, under the Actions column of the table, click **Embed Code**. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.
    
    * Click **Grid View**, **List View**, or **Detail View**. On the same toolbar, click **Preview** &gt; **Viewer List**.

      In the Viewer List page, under the Actions column of the table, click **Embed Code**. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

1. In the Embed Code dialog box, click **Copy to Clipboard**.

   Editing the code is not permitted in the Embed Code dialog box.

1. Click **Close**.
1. Paste the embed code in your web pages.

### Implementing embed code for using HTML5 video with MP4 video assets {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

If you do not use the Scene7 HTML5 video player, but instead want to use the native HTML5 `<video>` tag with MP4 video assets, you can use the following embed code sample:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Replace `"S7 video thumbnail URL"` with the video’s thumbnail URL. This is the video’s thumbnail image that a user sees before they play the video.

  See [Obtaining video thumbnail URLs](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Replace `"S7 OGG video asset URL (no player)"` with the video’s progressive URL for OGG video.

  See [Linking a video URL to a mobile site or a website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Replace `"S7 MP4 mobile progressive video asset URL (no player)"` with the video’s mobile progressive URL.

  See [Linking a video URL to a mobile site or a website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Deploying video using a third-party video player {#deploying-video-using-a-third-party-video-player}

If you use a third-party video player or a custom built video player instead of a Scene7 video viewer, you can obtain the direct video URL that works for HLS multi-bitrate video streaming or progressive download.

**To deploy video using a third-party video player**

1. In Scene7 Publishing System, on the Global Navigation bar, click **Setup** &gt; **Application Setup** &gt; **General Settings**.
1. Depending on the type of URL you want to use, do one of the following tasks:

<table cellpadding="4" cellspacing="0"> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" valign="top" width="NaN%"><p>To generate a direct HLS streaming video URL (multi-bitrate)</p></td> 
   <td class="cellrowborder" valign="top" width="NaN%"> 
    <ol> 
     <li><p>On the <strong>Application General Settings</strong> page, in the <strong>Servers</strong> group, in the <strong>Published Server Name</strong> text field, construct the direct URL using the following syntax:</p><p><span class="code">server/is/content/company/folder/filename.m3u8</span></p><p>For example, suppose the Published server name is <span class="code">https://s7d9.scene7.com/</span>. Using the syntax in step 2, the direct URL might look like the following:</p></li> 
     <li><p><span class="code">https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8</span></p></li> 
    </ol></td> 
  </tr> 
 </tbody> 
</table>

<table cellpadding="4" cellspacing="0"> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" valign="top" width="NaN%"><p>To generate a direct HLS streaming video URL (single bit rate)</p></td> 
   <td class="cellrowborder" valign="top" width="NaN%"> 
    <ol> 
     <li><p>On the <strong>Application General Settings</strong> page, in the <strong>Servers</strong> group, in the <strong>HLS Streaming Server Name</strong> text field, construct the direct URL using the following syntax:</p><p><span class="code">server/company/folder/filename.ext.m3u8</span></p><p>For example, suppose the HLS streaming server name is <span class="code">https://s7mbrstream.scene7.com/hls-vod/</span>. Using the syntax in step 2, the direct URL might look like the following:</p><p><span class="code">https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3_Teaser1_High_iPad_768x432_1296K.mp4.m3u8</span></p></li> 
    </ol></td> 
  </tr> 
 </tbody> 
</table>

<table cellpadding="4" cellspacing="0"> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" valign="top" width="NaN%"><p>To generate a direct progressive video URL</p></td> 
   <td class="cellrowborder" valign="top" width="NaN%"> 
    <ol> 
     <li><p>On the <strong>Application General Settings</strong> page, in the <strong>Servers</strong> group, in the <strong>Progressive Video Server Name</strong> text field, construct the direct eVideo URL using the following syntax:</p><p><span class="code">server/company/folder/filename</span></p><p>For example, suppose the progressive video server name is <span class="code">https://s7d9.scene7.com/is/content/</span>. Using the syntax in step 2, the direct URL might look like the following:</p><p><span class="code">https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4</span></p></li> 
    </ol></td> 
  </tr> 
 </tbody> 
</table>

## Working with video thumbnails {#working-with-video-thumbnails}

Scene7 generates thumbnails for encoded videos, and pre-encoded videos. You can use video thumbnails like any image asset. Moreover, you can obtain URLs for the video thumbnails that Scene7 generates and deploy these URLs outside SPS. For example, you can deploy the thumbnails in search results, related video listings, and video play lists on a website.

Thumbnails are generated based on the first heterogeneous frame (not an all black frame, or an all white frame, and so forth) of the video.

### Obtaining video thumbnail URLs {#obtaining-video-thumbnail-urls}

Scene7 generates video thumbnails automatically during the upload process. The thumbnails appear in the Browse panel in List view and Grid view.

To generate URLs for video thumbnails, perform a publish operation.

See [Publishing video](deploying-video-websites-mobile-sites.md#publishing_video).

After publishing, you can obtain video thumbnail URLs in Detail View in the URLs and Embed Code panel. Click **Copy URL** to the right of the video thumbnail to copy its URL

### Modifying poster frames in video viewers {#modifying-poster-frames-in-video-viewers}

The *poster frame* is the initial frame that appears in Video viewers before the video begins playing. Scene7 uses video thumbnails as poster frames.

You can apply image modifiers to the poster frame. For example, you can crop the poster frame or make it transparent. To modify the poster frame, open the video viewer configuration screen and enter modifiers in the Poster Image Modifiers section.

See [Adding or editing a video viewer preset](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

See [www.adobe.com/go/learn_s7_image_server_guide_en](https://www.adobe.com/go/learn_s7_image_server_guide_en).

You can also modify video thumbnails by appending modifiers to video thumbnail URLs.

>[!MORE_LIKE_THIS]
>
>* [Publishing files](publishing-files.md#publishing_files)
