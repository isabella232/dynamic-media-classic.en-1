---
title: Crop an image
description: Learn how to crop an image in Adobe Dynamic Media Classic.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
---
# Crop an image{#cropping-an-image}

You can crop images in the Adobe Dynamic Media Classic. The system retains information about images that were cropped so you can restore them to their original state. You can also crop an image and save the cropped version under a new name.

You can crop an image to remove white space around it, or crop an area of the image.

>[!NOTE]
>
>After you crop, you can select **[!UICONTROL Save As]** and save a cropped version of the image under a different name. In the Save As window, select **[!UICONTROL Save As New Master]** to save a second copy of the image. Select **[!UICONTROL Save As Addition View Of Master]** so you can save the original and its cropped version under a different name. Select **[!UICONTROL Replace Original]** to delete the original file from which you cropped your image. Then enter a name for the image, and select **[!UICONTROL Submit]**.

## Crop to remove white space around an image {#crop-to-remove-white-space-around-an-image}

You can crop off the transparent or solid-color pixels from the edge of an image.

1. To crop an image, select its rollover **[!UICONTROL Edit]** button and then select **[!UICONTROL Crop]**, or display it in the Browse Panel in Detail View and select the **[!UICONTROL Crop]** button.
1. On the Crop Editor page, do one of the following:

    * To trim color pixels, go to **[!UICONTROL Trim]** > **[!UICONTROL Color]**. In the **[!UICONTROL Auto Crop By Color]** dialog box, select the **[!UICONTROL Corner]** menu and choose a corner with the background color that you want to crop away. Then enter a **[!UICONTROL Tolerance]** setting from 0 through 1. The 0 setting crops pixels only if they exactly match the color you selected in the corner of the image. Numbers closer to 1 allow for more color difference. Select **[!UICONTROL Crop]**.
    * To trim transparent pixels, go to **[!UICONTROL Trim]** > **[!UICONTROL Transparent]**. In the **[!UICONTROL Auto Crop By Transparency]** dialog box, enter a tolerance setting from 0 through 1. The 0 setting crops pixels only if they are transparent. Numbers closer to 1 allow for more transparency. Select **[!UICONTROL Crop]**.

1. Select **[!UICONTROL Save]**.

>[!NOTE]
>
>To restore an image to its original state after you have cropped it, display the image in the Crop Editor screen and select **[!UICONTROL Reset]**.

## Select an area to crop {#select-an-area-to-crop}

1. To crop an image, select its rollover **[!UICONTROL Edit]** button, and choose **[!UICONTROL Crop]**, or display it in the Browse Panel in Detail View and select **[!UICONTROL Crop]**.

1. In the Crop Editor window, place the part of the image you do not want to crop in the crop box. Whatever appears inside the box is what will remain after you select **[!UICONTROL Save]** and crop the image.
1. To adjust the crop area, do one of the following:

    * Drag a side or corner of the box. Hold down the Shift key as you drag to change size but maintain the aspect ratio (the shape) of the crop box.
    * Enter pixel measurements in the Size boxes.
    * Drag to move the crop box. Move the pointer inside the boundary of the box. When you see the four-headed arrow, drag the box to a new location on the image.

1. Select **[!UICONTROL Save]**.

>[!NOTE]
>
>To restore an image to its original state after you have cropped it, display the image in the Crop Editor screen and select **[!UICONTROL Reset]**.

>[!MORELIKETHIS]
>
>* [Options for image editing at upload](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Crop white space from a PDF file](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Crop from the sides of PDF pages](pdfs.md#cropping_from_the_sides_of_pdf_pages)
