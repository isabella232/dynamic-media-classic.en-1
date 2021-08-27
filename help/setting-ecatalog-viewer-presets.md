---
title: Setting up eCatalog Viewer Presets
description: Learn how to set up eCatalog Viewer Presets.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
---
# Setting up eCatalog Viewer Presets{#setting-up-ecatalog-viewer-presets}

eCatalog Viewer Presets determine the style, behavior, and look of eCatalog Viewers. Adobe Dynamic Media Classic provides eCatalog Viewer Presets, and you can create your own eCatalog Viewer Presets as well if you are an administrator.

To create a preset, you can start from scratch or start with an Adobe Dynamic Media Classic-provided eCatalog Viewer Preset and save it under a new name. You can create your own eCatalog Viewer Presets to present printed material in your company colors and set the tone.

eCatalog Viewer Presets offer many settings for going from page to page, zooming, searching, and choosing “skins.” What these controls look like and how the Viewer appears, depends on your choice of eCatalog Viewer Presets.

Follow these steps so you can create a eCatalog Viewer Preset (you must be an administrator):

1. On the Global Navigation bar, click **[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**.
1. In the Viewer Presets screen, create an eCatalog Viewer Preset by starting anew or by starting from an existing eCatalog Viewer Preset:

   * **Creating an eCatalog Viewer Preset** - Click **[!UICONTROL Add]**. In the Add Viewer Preset dialog box, choose a platform, choose eCatalog Viewer, then click **[!UICONTROL Add]**.

   * **Editing an eCatalog Viewer Preset** - Select an eCatalog Viewer Preset, then click **[!UICONTROL Edit]**. Click **[!UICONTROL Save As]** after you finish creating the preset.

1. On the Configure Viewer screen, enter a name for your eCatalog Viewer Preset.
1. In the Configure Viewer screen, set the options you want.

   Click the **[!UICONTROL Info Tip]** icon next to the option if you want to read its description.

   The Preview page displays the viewer as you update and change settings.

1. (Optional) In the **[!UICONTROL Info Panel Settings]**, the **[!UICONTROL Information Server URL]** option can include the following special tokens, which the viewer substitutes:

    |Token|Substituted with|Notes|
    |--- |--- |--- |
    |`$1$`|rollover_key value|The item identifier from the `<area>` element of the map.|
    |`$2$`|frame|The sequence number of the currently shown frame in the image set.|
    |`$3$`|imageroot|The first path element of the first item specified in the image command (typically the image catalog ID of the catalog entry specifying the image set).|

1. (Optional) In the **[!UICONTROL Info Panel Settings]**, in the **[!UICONTROL Response Template]** box, type the text you want to appear if Adobe Dynamic Media Classic encounters an error in retrieving information for an image map. For example, if the system receives a company name and an eCatalog name, but no rollover identifier, this message appears for the user.

>[!NOTE]
>
>To use this Response Template instead of the template defined in the eCatalog itself, add `fmt=1` to the end of the Information Server URL. For example: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Click **Save**.
1. Click Default if you want the eCatalog Viewer Preset you created to be the one that is used to display eCatalogs on your web page.

To delete an eCatalog Viewer Preset, select it on the Viewer Presets screen and click **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)
