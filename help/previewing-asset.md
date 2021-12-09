---
title: Preview an asset
description: Learn how to preview an asset in Adobe Dynamic Media Classic.
uuid: 4a01be21-e37f-4d79-9220-f4e177e9179a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 17d0bfd6-fc62-4ed6-8a51-7ac1a6bb96cc
feature: Dynamic Media Classic,Asset Management,Viewers
role: User
exl-id: 7e6f652c-b197-4171-b11b-f532795f7cf2
---
# Preview an asset{#previewing-an-asset}

You can use Preview to see how a digital asset appears when viewed by a customer. The Preview uses the default viewer that is assigned to the asset. Default viewers are configured in Application Setup.

See [Configure default viewers](application-setup.md#configuring_default_viewers).

If you are previewing a template asset with parameter layers, you can change parameters or change the image preset. Because your changes are made inline, you can view the results immediately from the same Preview window.

See also [Adobe Viewers Reference Library Examples](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

**To preview an asset:**

1. In the Asset Library panel on the left side, navigate to the Asset folders that contains the asset you want to preview.
1. Do any one of the following:

    * Above the Assets window, on the right side of the toolbar, select **[!UICONTROL Grid View]**.
    * Above the Assets window, on the right side of the toolbar, select **[!UICONTROL List View]**.
    * Above the Assets window, on the right side of the toolbar, select **[!UICONTROL Detail View]**.

1. Depending on the view that you are using, do one of the following:

    * In the Asset window of the Grid View or List View, select a single asset, and then select **[!UICONTROL Preview]** near the thumbnail image.
    * On the toolbar above the Assets window of the Grid View, List View, or Detail View, select **[!UICONTROL Preview]**.

## Preview an asset based on viewer platform type {#previewing-an-asset-based-on-viewer-platform-type}

You can use Viewer List to preview how an asset appears on particular viewer platform type such as HTML5. Depending on the asset type and the associated viewer that you have selected to preview, not all platforms are available in Viewer List.

You can also use Viewer List to copy a viewer’s URL or view and copy the viewer code for embedding in your web pages.

For a given viewer platform, the Viewer List window lets you visually see what devices, such as tablets and Smartphones, that a viewer is available for use.

**To preview an asset based on viewer platform type:**

1. In the Asset Library panel on the left side, navigate to the Asset folders that contains the asset you want to preview.
1. Do any one of the following:

    * Above the Assets window, on the right side of the toolbar, select **[!UICONTROL Grid View]**. In the Asset window, select a single asset, and then below the thumbnail image, go to **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
    * Above the Assets window, on the right side of the toolbar, select **[!UICONTROL List View]**. In the Asset window, select a single asset, and then to the right of the thumbnail image, go to **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.
    * Above the Assets window, on the right side of the toolbar, select **[!UICONTROL Detail View]**. On the same toolbar, go to **[!UICONTROL Preview]** > **[!UICONTROL Viewer List]**.

1. (Optional) In the Viewer List window, select the column heading **[!UICONTROL Name]** or **[!UICONTROL Platform type]** to sort the column by ascending or descending order.
1. In the Viewer List window, under the Actions column of the table, select **[!UICONTROL Preview]** to see how the asset appears for a selected viewer and platform type.

   Close the displayed preview.

1. (Optional) In the Viewer List window, in the URL Encoding for Copy URL Generation drop-down list at the bottom, select the URL encoding that you want applied to the asset’s URL when it is copied.
1. (Optional) Do any of the following:

    * In the Viewer List window, under the Actions column of the table, select **[!UICONTROL Copy URL]** for a selected viewer and platform type.

      When you select **[!UICONTROL Copy URL]**, its associated URL is automatically copied to the clipboard.

    * In the Viewer List window, under the Actions column of the table, select **[!UICONTROL Embed Code]**.

      When you select **[!UICONTROL Embed Code]**, the Embed Code window is opened where you can review the viewer code. Editing of the code is not permitted in the window. You can also copy the code to the clipboard so you can paste it in your web pages.

      Close the displayed preview.

1. In the lower-right corner of the Viewer List window, select **[!UICONTROL Close]** to return to the Assets screen.

## Preview an image asset based on its Image Preset {#previewing-an-image-asset-based-on-its-image-preset}

You can preview an image asset based on its Image Preset to find out what your image looks like when it is delivered dynamically to your web site or application at different sizes.

An Image Preset is a collection of pre-defined settings that change the size, image quality, format, resolution, and other aspects of an image’s appearance when it is exported.

See [Set up Image Presets](setting-image-presets.md#setting_up_image_presets).

See [Create and enable Image Presets](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

**To preview an image asset based on its Image Preset:**

1. In the Asset Library panel on the left side, navigate to the Asset folders that contains the image asset you want to preview.
1. Do any one of the following:

    * Above the Assets window, on the right side of the toolbar, select **[!UICONTROL Grid View]**. In the Asset window, select a single image asset, and then below the thumbnail image, go to **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
    * Above the Assets window, on the right side of the toolbar, select **[!UICONTROL List View]**. In the Asset window, select a single image asset, and then to the right of the thumbnail image, go to **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.
    * Above the Assets window, on the right side of the toolbar, select **[!UICONTROL Detail View]**. On the same toolbar, go to **[!UICONTROL Preview]** > **[!UICONTROL Image Preset List]**.

1. In the Image Preset List window, in the table, select the name of a preset type whose image asset you want to preview inline in the right pane.
1. (Optional) In the Image Preset List window, in the **[!UICONTROL URL Encoding for Copy URL Generation]** drop-down list at the bottom, select the URL encoding to apply to the image asset’s URL when it is copied.
1. (Optional) In the Image Preset List window, in the upper-right area of the preview pane, select **[!UICONTROL Copy URL]** for the selected preset type.

   When you select **[!UICONTROL Copy URL]**, its associated URL is automatically copied to the clipboard.

1. In the lower-right corner of the Image Preset List window, select **[!UICONTROL Close]** to return to the Assets screen.
