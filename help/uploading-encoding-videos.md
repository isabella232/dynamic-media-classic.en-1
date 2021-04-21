---
title: Uploading and encoding videos
seo-title: Uploading and encoding videos
description: Learn how to upload and encode videos.
seo-description: Learn how to upload and encode videos.
uuid: 9a7d6513-b10c-40b0-aebb-18a795c2b8d1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: a0941823-850c-4373-9e37-f32032de3805
feature: Dynamic Media Classic,Viewers,Video
role: Business Practitioner
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
---
# Uploading and encoding videos{#uploading-and-encoding-videos}

To create single video or adaptive video sets for delivery to the web or mobile devices, you first upload your master video files to Dynamic Media Classic. Dynamic Media Classic encodes videos to MP4 format and it publishes video in the following file formats:

**MP4** Dynamic Media Classic recommends MP4 as the preferred video file format. Use MP4 files for the following:

* HTTP Dynamic Streaming on desktops.
* HTTP Live Streaming (Apple’s streaming protocol).
* Progressive video delivery to Android, Blackberry, and Windows mobile devices

Dynamic Media Classic offers two workflows for uploading video files:

**Pre-encoded Videos** You upload MP4 files directly to Dynamic Media Classic. With this workflow, files are not encoded at the time you upload them. The files are pre-encoded in preparation for delivery to the desktop and to mobile devices.

**Master source videos** Upload master source video files and, at upload, encode these files to MP4 files. Encoded videos are labeled “Video” in the Browse panel. Dynamic Media Classic supports the encoding of video files in many formats.

* Make sure the master source video files you want to encode are supported.

  See [Supported video file types for encoding](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

* Choose a video encoding preset.

  See [Video presets for encoding video files](application-setup.md#video-presets-for-encoding-video-files).  
  
  See [Best practices for video encoding](uploading-encoding-videos.md#best-practices-for-video-encoding).

Dynamic Media Classic also generates video thumbnails. You can learn more about video thumbnails, how to obtain their URLs, and modifying poster frames.

See [Working with video thumbnails](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**To upload and encode videos**

Do one of the following:

*If your videos are already encoded*

1. On the Global Navigation bar, click **Upload**.
1. In the Upload screen, click **From Desktop** tab.
1. On the Upload page, in the Select Files for Upload panel, click **Browse**, navigate to an MP4 video file, and then click **Open**.
1. In the Choose Folder Destination panel, select a folder for the uploaded file.
1. On the Upload page, make sure **Publish After Uploading** is checked.
1. Click **Submit Upload**.
  
*If you want to encode your videos using Dynamic Media Classic*

1. On the Global Navigation bar, click **Upload**. 
1. In the Upload screen, click **From Desktop** tab.
1. In the Select Files to Upload panel, click **Browse**, navigate to a master source video file, and then click **Open**.
1. In the Choose Folder Destination panel, select a folder for the uploaded file.
1. In the lower-right corner of the page, click **Job Options**,
1. In the Upload Job Options dialog box, expand EVideo Options.
   * Do one of the following:
     * Best practice is to use the following method.
       Select **Adaptive Video Encoding**.
       See [Adaptive Video (default)](application-setup.md#adaptive-video-default).
   *   Optional, if you want to use individual encoding settings, do the following.
       Expand **Single Encoding Presets**, and then select the encoding options you want for Desktop, Mobile, and Tablet.
       See [Desktop video encoding presets](application-setup.md#desktop-video-encoding-presets), [Mobile video encoding presets](application-setup.md#mobile-video-encoding-presets), [Tablet video encoding presets](application-setup.md#tablet-video-encoding-presets).
1. In the Upload Job Options dialog box, click **Save**.
1. On the Upload page, make sure **Publish After Uploading** is checked.
1. On the Upload page, in the lower-right corner, click **Submit Upload**.
    
If you want to re-encode a video file that you previously uploaded

1.  In Dynamic Media Classic, in the Browse panel, navigate to the video and select it.
1. Click **File** > **Reprocess**.
1. In the Reprocess Assets dialog box, expand EVideo Options.
1. Do one of the following:
   * Best practice is to use the following method.
     Select **Adaptive Video**.
     See [Adaptive Video (default)](application-setup.md#adaptive-video-default).
   * Optional, if you want to use individual encoding settings, do the following.
     Expand **Single Encoding Presets**, and then select the encoding options you want for Desktop, Mobile, and Tablet.
     See [Desktop video encoding presets](application-setup.md#desktop-video-encoding-presets), [Mobile video encoding presets](application-setup.md#mobile-video-encoding-presets), [Tablet video encoding presets](application-setup.md#tablet-video-encoding-presets).
1. In the Reprocess Assets dialog box, click **Submit**.

When you use Adaptive Video encoding preset or you use multiple single encoding presets, the result is an Adaptive Video Set that is automatically created with multiple video encodings. You can also manually create an Adaptive Video Set by selecting individual videos.

Only MP4 and M4V file types are created when you generate an Adaptive Video Set either automatically or manually.

## Supported video file types for encoding {#supported-video-file-types-for-encoding}

The following table lists video file types (with permitted video codecs) that you can encode to MP4 or OGV format when you upload files. The table lists file formats and codecs:

**Video file formats** Similar to a ZIP file, a video file format determines how files are contained in the video file. A video file usually contains multiple tracks — a video track (without audio) and one or more audio tracks (without video) — that are interrelated and synchronized. The video file format determines how these different data tracks and metadata are organized.

**Video codecs** A video codec describes the algorithm by which a video is encoded. A video player decodes the video according to its codec and then displays a series of images, or frames, on the screen. Codecs minimize the amount of information that video files are required to store to play video. Rather than information about each individual frame, only information about the differences between one frame and the next are stored. Because most videos change little from one frame to the next, codecs allow for high compression rates, which results in smaller file sizes.

|Video file format|Video codecs|
|:--- |:--- |
|3GP|H.263, H.264|
|AVI|DivX, DV|
|M2P|MPEG-2 PS|
|M2T|MPEG-2 TS|
|M2TS|MPEG-2 TS|
|M2V|MPEG-2 ES|
|M4V|H.264|
|MOV|DV, DVCPro 50, H.261, H.263, H.264, Sorenson Video 1|
|MP4|H.264/MPEG-4 AVC|
|MPEG|MPEG-2 SS|
|MPG|MPEG-2 SS|
|MTS|MPEG-2|
|ProRes|APCN , APCS, APCO, APCH, AP4H|
|TS|DVCPro 50|
|VOB|MPEG-2|
|WMV/ASF|VC-1, Windows Media Video 7, Windows Media Video 8|

>[!NOTE]
>
>The Jobs screen alerts you if you upload and attempt to encode a video file but the file is rejected because it contains an incompatible codec or file container. For more information, see [Checking job files](checking-job-files.md).

## Best practices for video encoding {#best-practices-for-video-encoding}

The following are best-practice tips for encoding source video files in Dynamic Media Classic.

For advice about video encoding, see the following:

* Article: *Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution: * [www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en).
* Video: *Video Encoding Basics: * [www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en).

### Source video files {#source-video-files}

When you encode a video file, use a source video file of the highest possible quality. Avoid using previously encoded video files because these files are already compressed, and further encoding creates a subpar quality video.

The following table describes the recommended size, aspect ratio, and minimum bit rate that your source video files should have when you encode them:

|Size|Aspect ratio|Minimum bit rate|
|--- |--- |--- |
|1024 X 768|4:3|4500 kbps for most videos.|
|1280 X 720|16:9|3000 - 6000 kbps, depending on the amount of motion in the video.|
|1920 X 1080|16:9|6000 - 8000 kbps, depending on the amount of motion in the video.|

### Obtaining a file’s metadata {#obtaining-a-file-s-metadata}

You can obtain a file’s metadata by viewing its metadata in Dynamic Media Classic, using a video editing tool, or using an application designed for obtaining metadata. Following are instructions for using MediaInfo, a third-party application, to obtain a video file’s metadata:

1. Go to this web page: [https://mediainfo.sourceforge.net/en/Download](https://mediainfo.sourceforge.net/en/Download).
1. Select and download the installer for the GUI version, and follow the installation instructions.
1. After installation, either right-click the video file (Windows only) and select MediaInfo, or open MediaInfo and drag your video file into the application. You see all metadata associated with your video file, including its width, height, and fps.

### Aspect ratio {#aspect-ratio}

When you choose or create a video encoding preset for your master video file, make sure that the preset has the same aspect ratio as the master video file. The *aspect ratio* is the ratio of the width to the height of the video.

To determine the aspect ratio of a video file, obtain the file’s metadata and note the file’s width and height (see [Obtaining a file’s metadata](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Then use this formula to determine the aspect ratio:

width/height = aspect ratio

The following table describes how formula results translate to common aspect ratio choices:

|Formula result|Aspect ratio|
|--- |--- |
|1.33|4:3|
|0.75|3:4|
|1.78|16:9|
|0.56|9:16|

For example, a video that is 1440 width x 1080 height has an aspect ratio of 1440/1080, or 1.33. In this case you choose a video encoding preset with a 4:3 aspect ratio to encode the video file.

### Data rate {#data-rate}

The *data rate* (also called the* bit rate*) is the amount of data that is encoded to make up a single second of video playback. The data rate is measured in kilobits per second (Kbps).

>[!NOTE]
>
>Because all codecs use lossy compression, data rate is the most important factor in video quality. With lossy compression, the more you compress a video file, the more the quality is degraded. For this reason, all other characteristics being equal (the resolution, frame rate, and codec), the lower the data rate, the lower the quality of the compressed file.

When you choose a video encoding preset, take into account the target end user’s connection speed. Choose a preset with a data rate that is 80 percent of that speed. For example, if the target end user’s connection speed is 1000 Kbps, the best preset is one with a video data rate of 800 Kbps.

This table describes the data rate of typical connection speeds.

|Speed (Kbps)|Connection type|
|--- |--- |
|256|Dial-up connection.|
|800|Typical mobile connection. For this connection, target a data rate in the range of 400 to a maximum of 800 for 3G experiences.|
|2000|Typical broadband desktop connection. For this connection, target a data rate in the 800-2000 Kbps range, with most targets averaging 1200-1500 Kbps.|
|5000|Typical high-broadband connection. Encoding in this upper range is not recommended because video delivery at this speed is not available to most consumers.|

### Resolution {#resolution}

*Resolution* describes a video file’s height and width in pixels. Most source video is stored at a high resolution (for example, 1920 x 1080). For streaming purposes, source video is compressed to a smaller resolution (640 x 480 or smaller).

Resolution and data rate are two integrally linked factors that determine video quality. To maintain the same video quality, the higher the number of pixels in a video file (the higher the resolution), the higher the data rate must be. For example, consider the number of pixels per frame in a 320 x 240 resolution and a 640 x 480 resolution video file:

|Resolution|Pixels per frame|
|--- |--- |
|320 x 240|76,800|
|640 x 480|307,200|

The 640 x 480 file has four times more pixels per frame. To achieve the same data rate for these two example resolutions, you apply four times the compression to the 640 x 480 file, which can reduce the quality of the video. Therefore, a video data rate of 250 Kbps produces high-quality viewing at a 320 x 240 resolution, but not at a 640 x 480 resolution.

>[!NOTE]
>
>In general, the higher data rate you use, the better your video looks, and the higher resolution you use, the higher data rate you need to maintain viewing quality (compared to lower resolutions).

Because resolution and data rate are linked, you have two options when encoding video:

* Choose a data rate and then encode at the highest resolution that looks good at the data rate you chose. 
* Choose a resolution and then encode at the data rate necessary to achieve high-quality video at the resolution you chose.

When you choose (or create) a video encoding preset for your master video file, use this table to target the correct resolution:

|Resolution|Height (pixels)|Screen size|
|--- |--- |--- |
|240p|240|Tiny screen|
|300p|300|Small screen typically for mobile devices|
|360p|360|Small screen|
|480p|480|Medium screen|
|720p|720|Large screen|
|1080p|1080|High-definition large screen|

### Fps (frames per second) {#fps-frames-per-second}

In the United States and Japan, most video is shot at 29.97 frames per second (fps); in Europe, most video is shot at 25 fps. Film is shot at 24 fps.

Choose a video encoding preset that matches the fps rate of your master video file. For example, if your master video is 25 fps, choose an encoding preset with 25 fps. By default, all custom encoding uses the master video file’s fps. For this reason, you do not need to explicitly specify the fps setting when you create a video encoding preset.

### Video encoding dimensions {#video-encoding-dimensions}

For optimal results, select encoding dimensions such that the source video is a whole multiple of all your encoded videos.

To calculate this ratio, you divide source width by encoded width to get the width ratio. Then, you divide source height by encoded height to get the height ratio.

If the resulting ratio is a whole integer, it means that the video is optimally scaled. If the resulting ratio is not a whole integer, it impacts video quality by leaving leftover pixel artifacts on the display. This effect is most noticeable when the video has text.

As an example, suppose that your source video is 1920 x 1080. In the following table, the three encoded videos provide the optimal encoding settings to use.

|Video Type|Width x Height|Width Ratio|Height Ratio|
|--- |--- |--- |--- |
|Source|1920 x 1080|1|1|
|Encoded|960 x 540|2|2|
|Encoded|640 x 360|3|3|
|Encoded|480 x 270|4|4|

### Encoded video file format {#encoded-video-file-format}

Adobe Dynamic Media Classic recommends using MP4 H.264 video encoding presets. Because MP4 files use the H.264 video codec, it provides high-quality video but in a compressed file size.

## Working with video encoding presets {#working-with-video-encoding-presets}

Master video files created with video production equipment and video-editing software are often too large and not in the proper format for delivery to online destinations. To convert digital video to the proper format and specifications for playback on different screens, you can *transcode* video files (a process also known as *encoding*). During the encoding process, the video is compressed to a smaller, efficient file size for optimal delivery to the web and to mobile devices.

See [Uploading and encoding videos](uploading-encoding-videos.md#uploading-and-encoding-videos).

Dynamic Media Classic gives you a library of predefined video encoding presets that reflect the most common encoding settings used today. These encoding presets are optimized for playback on target screens. In addition, administrators can create their own video encoding presets to customize the size and playback quality of videos to end users. All video encoding presets, whether out-of-the-box from Dynamic Media Classic, or custom-made, output video in the MP4 file format.

On the Video Presets screen, administrators can set up and manage video encoding. They can do the following:

* Activate and deactivate video encoding presets.
* Create a video encoding preset.
* Edit video encoding presets.
* Delete video presets.

Any video that you upload to Dynamic Media Classic or that you encode in Dynamic Media Classic is treated as “video”. In other words, this asset classification means that you can deliver the video for playback on desktops, mobile devices, or both. For example, you can preview these types of videos in Dynamic Media Classic. You can also generate URLs (using the Copy URL feature) and code that you can embed (using the Embed Code feature) for use with video players, on websites, and so on.

See [Previewing videos in a video viewer](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

See [Linking a video URL to a mobile site or a website](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

See [Embedding the video viewer on a web page](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

For video assets that you upload and encode in Dynamic Media Classic, video is delivered in the following file format:

**MP4 H.264** Use MP4 files for the following:

* HTTP Dynamic Streaming on desktops.
* HLS (HTTP Live Streaming, Apple’s streaming protocol).
* Progressive video delivery to Android, Blackberry, and Windows mobile devices.

Any other video format and codec is treated as a “Master Video”. This asset classification means that the video is a source video file and cannot be used for delivery playback on desktops or mobile devices. For example, you cannot preview these types of videos in Dynamic Media Classic. You also cannot generate Copy URLs or Embed Code for use in video players, on websites, and so on.

### Filtering the list of video encoding presets {#filtering-the-list-of-video-encoding-presets}

The Video Presets page and the Adaptive Video Presets page consist of a table that lists the active status, preset name, intended playback device, video dimension, and target data rate of each video preset.

You can refine the list by choosing to filter on Both, Active, or Inactive, to see all Video Presets or narrow the list to presets that are active or inactive.

You can also filter based on a playback device option to narrow the list to Video Presets designed for playing videos on all devices, desktop, mobile, or tablets.

**To filter the list of video encoding presets**

1. In Dynamic Media Classic, click **Setup** > **Application Setup** > **Video Presets** > **Adaptive Video Presets** or **Single Encoding Presets**.

   The pages for Adaptive Video Presets and Single Encoding Presets include a table that lists the Active status, Preset name, intended Playback Device, video dimensions, and Target data rate of each video preset. 

1. On the Single Encoding Presets page called Video Presets, on the Video Presets toolbar, use the two drop-down lists to refine the list of presets in the table based on Active status, and playback device.

    * On the first, narrower drop-down list, choose **Both** to see all Video Presets, or choose **Active** or **Inactive** or narrow the list to presets that are active or inactive.
    * On the second, wider drop-down list, choose a playback device option to narrow the list to Video Presets designed for playing videos on desktops. or for playing videos on mobile or tablet devices.

### Activating or deactivating video encoding presets {#activating-or-deactivating-video-encoding-presets}

Activated Video Presets show up in the Upload Job Options dialog box. This is the dialog box that appears when a user uploads video files during the upload process. They can choose from a list of all activated encoding presets.

**To activate or deactivate video encoding presets:**

1. In Dynamic Media Classic, click **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video Presets]**.
1. Do one of the following:

    * Click **[!UICONTROL Adaptive Video Presets]**.
    * Click **[!UICONTROL Single Encoding Presets]**.

1. Do one of the following:

    * To activate a video preset, on the presets page, under the Active column, select the box next to a preset name.
    * To deactivate a video preset, deselect the box next to the video presets that you want to make inactive.

      >[!NOTE]
      >
      >Inactive Video Presets do not appear in the Upload Job Options dialog box.

1. In the lower right corner of the page, click **[!UICONTROL Close]**.

### Adding or editing a video encoding preset {#adding-or-editing-a-video-encoding-preset}

You can create your own custom single encoding video presets and add them to the Video Presets table. You can also make changes to any pre-defined single encoding Video Presets that came with Dynamic Media Classic, provided you save the edited preset with a new name.

Dynamic Media Classic has set maximum limits on the target data rate, resolution height, and resolution width to ensure a proper playback experience. Warning messages appear if you exceed these limits which are the following:

* For computer playback, the limits are: (Width/16) &#42; (Height/16) &lt; 8192.
* For mobile playback, the limits are: (Width/16) &#42; (Height/16) &lt; 660; target data rate &lt; 4000.
* For tablet playback, the limits are: (Width/16) &#42; (Height/16) &lt; 3600.

**To add or edit a video encoding preset**

1. In Dynamic Media Classic, click **Setup** > **Application Setup** > **Video Presets**.
1. Click **Single Encoding Presets** to open the Video Presets page.
1. In the Video Presets page, do any one of the following:

    * On the Video Presets toolbar click **Add** to add a new Video Preset.
    * Select a Video Preset. In the toolbar, click **Edit**.

      You cannot edit Dynamic Media Classic predefined presets; you can only create a preset from an existing one by choosing **Save As**.

1. On the Add Video Preset page or the Edit Video Preset page, set the Video Preset options you want.

   See [Best practices for video encoding](uploading-encoding-videos.md#best-practices-for-video-encoding) for recommended settings.

    |Video Preset option|Description|
    |--- |--- |
    |Preset Name|Enter a descriptive name for the Video Preset. The name you enter appears in the Upload Job Options dialog box, in which users choose transcoding options.|
    |Description|Describe the Video Preset. What you enter appears as a tool tip when you move the pointer over the name of the preset in the Upload Job Options dialog box in which users choose transcoding options.|
    |Playback Device|Choose the device that the video is intended to play back on. The options are Computer (desktops), Mobile (iPhone, iPad, Android); or Tablet (iPad only). This setting automatically determines the appropriate video and audio codec that is used during encoding.|
    |Target Data Rate|Enter the average Internet connection speed (in kilobits per second) of the target end user. You can enter the rate or drag the slider to enter it. The User Connection Speed spectrum lists typical speeds for broadband, DSL, mobile, and dial-up connections. This setting automatically determines the combined video and audio data rate. In other words, the amount of data that is encoded to make up a single second of video playback. The higher the data rate, the better the quality of the resulting video. However, data rates that are too high result in large file sizes that create subpar viewing experiences for users with a low bandwidth. As a best practice, strike a balance between high and low data rates. Aim to create an adequate quality playback experience without alienating users who have narrow bandwidths.|
    |Aspect Ratio|Aspect ratio is the ratio of the width to the height of the video. The first two aspect ratios listed below are commonly used to display video horizontally:<ul><li> 4:3 - Used for almost all standard definition TV broadcast content.</li><li>16:9 - Used for almost all wide-screen, high-definition TV content (HDTV) and movies.</li><li>Auto-scale - (Default) A single encoding preset that works with any aspect ratio to create videos for delivery to mobile, tablet, and desktop. Uploaded source videos that are encoded with this preset are set with a fixed height. However, the width automatically scales to preserve the video’s aspect ratio (width to height ratio).</li><li>Custom - Used when you want to define a non-standard video size.</li><li>The aspect ratio you choose determines the width and height settings for the Resolution Size; the width and height value automatically scale to the proper aspect ratio.</li></ul>|
    |Resolution Size|Resolution size, expressed by the number of pixels wide by the number of pixels high, determines the dimension. Enter a width and height value in pixels or drag the slider to enter these values. The Resolution spectrum lists typical resolution sizes. The width and height values automatically adhere to the aspect ratio you selected. For example, if you select 4:3 as the aspect ratio and enter 400 for width, 300 is entered automatically for height.If you selected Auto-scale for the Aspect Ratio setting, then the Width value for the Resolution Size is automatically set to Auto.Click Preview to open a browser window and see your resolution choices there.|
    |Encode File Suffix|Enter a suffix. This suffix is appended to the resulting encoded video file. You can enter a hyphen and underscore in the name; blank spaces and special characters are not allowed.|
    |Other Settings|Dynamic Media Classic determines all other encoding settings automatically according to best-practice encoding guidelines.|

1. Do one of the following:

    * Click **Save** if you added or edited a Video Preset. 
    * Click **Save As** if you added a Video Preset by starting from an existing preset.

### Deleting a video encoding preset {#deleting-a-video-encoding-preset}

Administrators can delete custom Video Presets. Video presets that come with Dynamic Media Classic cannot be deleted.

**To delete a video encoding preset**

1. In Dynamic Media Classic, click **Setup** > **Application Setup** > **Video Presets**.
1. Click **Single Encoding Presets** to open the Video Presets page.
1. In the Video Presets page, select a Video Preset in the table that you no longer want or need.
1. On the Video Presets toolbar, click **Delete**.
1. In the Delete Preset dialog box, click **Delete**.

>[!MORELIKETHIS]
>
>* [Quick Start: Video](quick-start-video.md#quick-start-video)
>* [Uploading and encoding videos](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Working with video viewer presets](previewing-videos-video-viewer.md#working-with-video-viewer-presets)
