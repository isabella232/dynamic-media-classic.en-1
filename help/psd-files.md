---
title: Work with PSD files
description: Learn how to work with PSD files in Adobe Dynamic Media Classic.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
---
# Work with PSD files{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD (Photoshop Document files) are most often used in Adobe Dynamic Media Classic to create templates. When you upload a PSD file, you can create an Adobe Dynamic Media Classic template automatically from the file (select the Create Template option on the Upload screen).

Adobe Dynamic Media Classic creates multiple images from a PSD file with layers if you use the file to create a template; it creates one image for each layer.

## PSD upload options {#psd-upload-options}

Options for uploading PSD files are located under Photoshop Options in the Upload Job Options dialog box. You can crop a file, choose a color profile for it, use it to create a template, and select an anchor.

These options are available when uploading PSD files:

* **Crop Options** - Located under **[!UICONTROL Crop Options]**. Select **[!UICONTROL Trim]** to automatically crop white space from the edges of a PSD file; select **[!UICONTROL Manual]** to crop sides of the PSD file:

  * **[!UICONTROL Trim]** - Select the **[!UICONTROL Trim Away Based On]** menu, and choose **[!UICONTROL Color]** or **[!UICONTROL Transparency]**.

    If you choose the **[!UICONTROL Color]** option, select the Corner menu and choose the corner of the PSD with the color that best represents the white-space color you want to crop.

    Drag the slider to specify a tolerance from 0 through 1. To trim based on color, specify 0 to crop pixels only if they exactly match the color you selected in the corner of the PSD. Numbers closer to 1 allow for more color difference. To trim based on transparency, specify 0 to crop pixels only if they are transparent; numbers closer to 1 allow for more transparency.

  * **[!UICONTROL Manual]** - Enter the number of pixels to crop from any side or each side of the image. How much of the image is cropped depends on the ppi (pixels per inch) setting in the image file. For example, if the image displays 150 ppi and you enter 75 in the Top, Right, Bottom, and Left text boxes, a half-inch is cropped from each side of the image.

* **Color Profile Options** - Located under **[!UICONTROL Color Profile Options]**.

  * **[!UICONTROL Default Color Preservation]**

  * **[!UICONTROL Keep Original Color Space]** - Retains the original color space of the image.

  * **[!UICONTROL Custom From]** > **[!UICONTROL To]** - Opens menus so you can choose a Convert From and Convert To color space. You can choose a standard Photoshop color space or a color space you uploaded to Adobe Dynamic Media Classic. See [ICC profiles](/help/icc-profiles.md).

* **Photoshop Options**

  * **[!UICONTROL Maintain Layers]** - Rips the layers in the PSD, if any, into individual assets. The asset layers remain associated with the PSD. You can view them by opening the PSD file in Detail View and selecting the layer panel. See Viewing and editing layers in a PSD file.

  * **[!UICONTROL Create Template]** - Creates a template from the layers in the PSD file.

  * **[!UICONTROL Extract Text]** - Extracts the text so that users can search for text in a Viewer.

  * **[!UICONTROL Extend Layers To Background Size]** - Extends the size of ripped image layers to the size of the background layer.

  * **[!UICONTROL Layer Naming]** - Layers in the PSD file are uploaded as separate images. To name these images in Adobe Dynamic Media Classic, choose from the following options:

    * **[!UICONTROL Layer Name]** - Names the images after their layer names in the PSD file. For example, a layer named Price Tag in the original PSD file becomes an image named Price Tag. However, if the layer names in the PSD file are default Photoshop layer names (Background, Layer 1, Layer 2, and so on), the images are named after their layer numbers in the PSD file. <!-- not their default layer names -->

    * **[!UICONTROL Photoshop and layer number]** - Names the images after their layer numbers in the PSD file, ignoring original layer names. Images are named with the Photoshop filename and an appended layer number. For example, the second layer of a file called `Spring Ad.psd` is named `Spring Ad_2` even if it had a non-default name in Photoshop.

    * **[!UICONTROL Photoshop and layer name]** - Names the images after the PSD file followed by the layer name or layer number. The layer number is used if the layer names in the PSD file are default Photoshop layer names. For example, a layer named `Price Tag` in a PSD file named `SpringAd` is named `Spring Ad_Price Tag`. A layer with the default name Layer 2 is called `Spring Ad_2`.

  * **[!UICONTROL Anchor]** - Specify how images are anchored in templates that are generated from the layered composition produced from the PSD file. By default, the anchor is the center. A center anchor allows replacement images to best fill the same space, no matter the aspect ratio of the replacement image. Images with a different aspect that replace this image, when referencing the template and using parameter substitution, effectively occupy the same space. Change to a different setting if your application requires the replacement images to fill the allocated space in the template.

## View and edit layers in a PSD file {#viewing-and-editing-layers-in-a-psd-file}

If you selected the Maintain Layers option when you uploaded your PSD, Adobe Dynamic Media Classic ripped the individual layers into assets. You can view and edit the asset layers belonging to a PSD file by opening the file in the Browse Panel in Detail View.

1. Double-click the full PSD file in the Browse Panel. The file opens in Detail View.

    >[!NOTE]
    >
    >Make sure that you open the full asset and not one of the PSD layers.

1. Select **[!UICONTROL Layers]**. All the layers appear as separate images in the Layers panel.
1. Double-click a layer and do any of the following:

    * To create an image map on the layer, select **[!UICONTROL Image Map]** icon. (See [Create Image Maps](creating-image-maps.md#creating_image_maps).)
    * To create zoom targets on the layer, select **[!UICONTROL Zoom Targets]** icon. (See [Create zoom targets for Guided Zoom](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
    * To crop the layer, select **[!UICONTROL Crop]** icon. (See [Crop an image](cropping-image.md#cropping_an_image).)
    * To sharpen the layer, select **[!UICONTROL Sharpen]**. (See [Sharpen an image](sharpening-image.md#sharpening_an_image).)
    * To adjust the layer, select **[!UICONTROL Adjust]**. (See [Adjust an image](adjusting-image.md#adjusting_an_image).)

1. Select **[!UICONTROL Save]** or **[!UICONTROL Save As]**.
1. To view or edit a different layer, select an arrow at the bottom of the layer preview.
1. To exit the layer Detail View, select the **[!UICONTROL Grid View]** icon.
