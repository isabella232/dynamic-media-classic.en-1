---
title: Setting up Zoom Viewer Presets
seo-title: Setting up Zoom Viewer Presets
description: null
seo-description: Learn how to set up Zoom Viewer Presets.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b

---

# Setting up Zoom Viewer Presets{#setting-up-zoom-viewer-presets}

Zoom Viewer Presets determine the style, behavior, and look of your Zoom viewers. Scene7 offers many options for customizing and skinning Viewers. Scene7 comes with default basic (fast), fly-out, and custom Zoom Viewer Presets. If you are an administrator, you can create new company Zoom Viewer Presets or edit a default preset and save it with a new name.

All Zoom Viewers have buttons for zooming in, zooming out, panning, and resetting the image to its original state after zooming. What these buttons look like and what the window itself looks like depends on your choice of Zoom Viewer Presets. You can configure a Zoom Viewer Preset with different colors, borders, fonts, and image settings. When configuring a Guided Zoom Viewer, you can also choose where to place the zoom targets. Zoom targets are the thumbnails that users click to zoom to areas you specify.

## About Zoom Viewer Presets {#about-zoom-viewer-presets}

Scene7 offers these Zoom Viewer Presets:

**Zoom Viewer: Basic** Provides a basic zoom on original image.

**Zoom Viewer: Fly-out** Displays a second image of the zoomed area next to the original image. There are no controls to use, users simply move the selection over the area they want to view.

When determining the complete bandwidth usage for this viewer, consider that both the main image and the flyout image are served in the viewer. The flyout image size is determined by the main image size (Stage Width and Height) and the Zoom Factor. To keep the flyout file size from becoming too large, balance these two values: if you have a large main image size, lower the Zoom Factor value. (The Flyout Width and Flyout Height determine the size of the flyout window, but not the size of the flyout image that is served into the viewer.)

For example, if your main image size is 350 by 350 pixels, with a Zoom Factor of 3, the resulting flyout image is 1050 by 1050 pixels. If your main image size is 300 by 300 pixels, with a Zoom Factor of 4, the flyout image is 1200 by 1200 pixels. Depending on the JPEG quality setting (recommended settings are between 80-90), you can decrease the file size significantly. Recommended zoom factors are 2.5 to 4, depending on the size of your main image.

Scene7 recommends these parameters for fly-out Zoom Viewer Presets:

**Enlarged image size** Approximately 1500 by 1500 pixels, not to exceed 2000 by 2000 pixels.

**Image size** 100KB or under, not to exceed 150KB (compress the file to keep it under 150KB).

**Zoom Viewer: Custom** Provides guided or unguided zoom with images, Image Sets with multiple views, or Color Swatch Sets.

## Creating and editing Zoom Viewer Presets {#creating-and-editing-zoom-viewer-presets}

Follow these steps to create or edit a Zoom Viewer Preset:

1. Click **Setup** &gt; **Viewer Presets**.
1. Do one of the following:

   **Creating a preset** Click Add. In the Add Viewer Preset dialog box, choose a platform, choose a Zoom Viewer, and then click Add. Enter a name for the preset in the Preset Name box.

   **Editing a preset** Select a Zoom Viewer Preset, then click **Edit**.

1. Specify settings as desired.

   To see a description of an option, click the Info Tip icon adjacent to the option.

   The preview screen displays the viewer as you update and change settings.

1. Click **Save** or **Save As**.
1. On the Viewer Presets screen, examine the Zoom Viewer Preset or Guided Zoom Viewer Preset you created. If it needs adjusting, click **Edit**, change settings on the Configure Viewer screen, and click **Save**.

For information about managing Viewer Presets on the Viewer Presets screen, see [Viewer Presets](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Creating and editing Viewer Presets](application-setup.md#adding_and_editing_viewer_presets)
