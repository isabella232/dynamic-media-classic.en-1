---
title: Setting up eCatalog Viewer Presets
seo-title: Setting up eCatalog Viewer Presets
description: null
seo-description: Learn how to set up eCatalog Viewer Presets.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
index: y
internal: n
snippet: y
---

# Setting up eCatalog Viewer Presets{#setting-up-ecatalog-viewer-presets}

eCatalog Viewer Presets determine the style, behavior, and look of eCatalog Viewers. Scene7 provides eCatalog Viewer Presets, and you can create your own eCatalog Viewer Presets as well if you are an administrator.

To create a new preset, you can start from scratch or start with a Scene7-provided eCatalog Viewer Preset and save it under a new name. You can create your own eCatalog Viewer Presets to present printed material in your company colors and set the tone.

eCatalog Viewer Presets offer many settings for going from page to page, zooming, searching, and choosing “skins.” What these controls look like and what the Viewer itself looks like depends on your choice of eCatalog Viewer Presets.

Follow these steps to create a eCatalog Viewer Preset (you must be an administrator):

1. Click **Setup** &gt; **Viewer Presets**.
1. In the Viewer Presets screen, create an eCatalog Viewer Preset by starting anew or by starting from an existing eCatalog Viewer Preset:

   **Creating an eCatalog Viewer Preset** Click Add. In the Add Viewer Preset dialog box, choose a platform, choose eCatalog Viewer, then click Add.

   **Editing an eCatalog Viewer Preset** Select an eCatalog Viewer Preset, then click Edit. Click Save As after you finish creating the preset.

1. On the Configure Viewer screen, enter a name for your eCatalog Viewer Preset.
1. In the Configure Viewer screen, set the options you want.

   Click the Info Tip icon  ![](assets/Infotip.png)

   adjacent to the option to see its description.

   The preview screen displays the viewer as you update and change settings.

1. (Optional) In the Info Panel Settings, the Information Server URL option can include the following special tokens, which the viewer substitutes:

    |Token|Substituted with|Notes|
    |--- |--- |--- |
    |`$1$`|rollover_key value|The item identifier from the `<area>` element of the map.|
    |`$2$`|frame|The sequence number of the currently shown frame in the image set.|
    |`$3$`|imageroot|The first path element of the first item specified in the image command (typically the image catalog ID of the catalog entry specifying the image set).|

1. (Optional) In the Info Panel Settings, in the Response Template box, type the text you want to appear if Scene7 encounters an error in retrieving information for an image map. For example, if the system receives a company name and an eCatalog name, but no rollover identifier, this message appears for the user.

>[!NOTE]
>
>To use this Response Template instead of the template defined in the eCatalog itself, add “fmt=1” to the end of the Information Server URL. For example: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Click **Save**.
1. Click Default if you want the eCatalog Viewer Preset you created to be the one that is used to display eCatalogs on your web page.

To delete an eCatalog Viewer Preset, select it on the Viewer Presets screen and click **Delete**.

>[!MORE_LIKE_THIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)
