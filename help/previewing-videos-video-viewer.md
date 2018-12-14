---
title: Previewing videos in a video viewer
seo-title: Previewing videos in a video viewer
description: null
seo-description: Learn how to preview videos in a Video viewer.
uuid: 7ab4e805-6e5d-461b-bd99-5e09b9ced950
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 6a2e6df1-9186-42e2-9b85-01f132936c72
index: y
internal: n
snippet: y
---

# Previewing videos in a video viewer{#previewing-videos-in-a-video-viewer}

You can preview what a video looks like and how it plays in the Video Viewer.

See [Adding and editing Viewer Presets](application-setup.md#adding_and_editing_viewer_presets).

**To preview videos in a video viewer**

1. In the Asset Library panel on the left side, in the Show drop-down list, select **Video** (single encoded videos) or **Adaptive Video Set** (when the Adaptive Video encoding preset is used, it results in a set of multi-bitrate encoded videos).
1. In the Asset Library panel on the left side, navigate the asset folders to select the video that you want to preview.
1. Do any one of the following

    * Above the Assets window, on the right side of the toolbar, click **List View**. In the Asset window, hover on an asset, and then click **Preview**.
    * Above the Assets window, on the right side of the toolbar, click **Grid View**. In the Asset window, in an asset thumbnail window, click **Preview**.
    * Above the Assets window, on the right side of the toolbar, click **Detail View**. On the same toolbar, click **Preview**.
    * In the Asset window, select an asset. In the toolbar, click **File** &gt; **Preview**.

1. (Optional) In the Preview window, in the drop-down list at the bottom, select the URL encoding that you want applied to the asset’s URL when it is copied.
1. Click the Preview link to preview the asset in the selected viewer.
1. Close the displayed viewer to return to the Preview screen.
1. Click **Close** to return to the Assets screen.

>[!NOTE]
>
>Scene7 provides a convenient method of previewing MP4 video on the desktop. Use this method to preview mobile content on the desktop without physically testing it on mobile devices. Be aware, however, that what you see in the desktop preview does not realistically show what playback looks like on the mobile device. To preview how video looks and plays on a mobile device, go to the Preview screen, select the Copy URL and enter that URL in the web browser of a mobile device. For more information, see [Deploying video to your websites and mobile sites](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

## Working with video viewer presets {#working-with-video-viewer-presets}

Users watch videos in the Video Viewer. How the Video Viewer behaves, what it looks like, and how its playback controls work depends on the Viewer Preset you choose for playing the video. You choose a Viewer Preset on the Preview screen. After you choose a preset, you can obtain the URL or the embed code for playing the video using the Viewer Preset you chose.

Scene7 comes with many predefined Viewer Presets for playing video, and if you are an administrator, you can create custom Viewer Presets. There are more than a dozen different settings for configuring the Video Viewer. You can configure its size, color, video and audio controls, progress bar, user-interface skin, and social features.

See also [Previewing videos in a video viewer](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

### Adding or editing a video viewer preset {#adding-or-editing-a-video-viewer-preset}

You can use Viewer Presets to see various viewer types and their pre-defined settings. You can also add and edit your own customized viewer presets or edit existing viewer presets that come with Scene7 Publishing System.

In Viewer Presets you can activate, filter, sort, and preview Viewer Presets.

See [Viewer Presets](application-setup.md#viewer_presets).

**To add or edit a video viewer preset**

1. Near the upper-right corner of Scene7 Publishing System, click **Setup** &gt; **Viewer Presets**.

   To see only presets for Video Viewers, select Video Viewer from the open the Viewers drop-down list in the toolbar directly above the table.

1. Add or edit a Viewer Preset for showing video:

   **Adding** Click Add in the toolbar. In the Add Viewer Preset dialog box, choose a platform and viewer from the respective drop-down lists, and then click Add.

   See also [Adding and editing Viewer Presets](application-setup.md#adding_and_editing_viewer_presets).

   **Adding by starting from an existing Viewer Preset** In the table, select a Video Viewer Preset, and then click Edit in the toolbar.

   After you reconfigure the Video Viewer, click **Save As** to save the preset using a different name in the Preset Name text field.

   **Editing** Select a Video Viewer Preset, and then click Edit.

1. In the Configure Viewer screen, in the Preset Name field, enter or edit the preset name.
1. Set the remaining options that you want.

   To see a description of an option, click its Info Tip icon.

1. Do one of the following:

    * Click **Save As** if you added a Viewer Preset by starting from an existing preset. 
    * Click **Save** if you added or edited a Viewer Preset.

>[!MORE_LIKE_THIS]
>
>* [Best practices for video encoding](uploading-encoding-videos.md#best_practices_for_video_encoding)
>* [Working with video encoding presets](uploading-encoding-videos.md#working_with_video_encoding_presets)
