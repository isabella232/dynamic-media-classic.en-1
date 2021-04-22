---
title: Cropping an image
description: Learn how to crop an image.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
---
# Cropping an image{#cropping-an-image}

You can crop images in the Dynamic Media Classic. The system retains information about images that were cropped so you can restore them to their original state. You can also crop an image and save the cropped version under a new name.

You can crop an image to remove white space around it, or crop an area of the image.

>[!NOTE]
>
>After you crop, you can click the Save As button and save a cropped version of the image under a different name. In the Save As window, choose Save As New Master to save a second copy of the image. Click **[!UICONTROL Save As Addition View Of Master]** to save the original and its cropped version under a different name. Click **[!UICONTROL Replace Original]** to delete the original file from which you cropped your image. Then enter a name for the image, and click **[!UICONTROL Submit]**.

## Crop to remove white space around an image {#crop-to-remove-white-space-around-an-image}

You can crop off the transparent or solid-color pixels from the edge of an image.

1. To crop an image, click its rollover **[!UICONTROL Edit]** button and choose **[!UICONTROL Crop]**, or display it in the Browse Panel in Detail view and click the **[!UICONTROL Crop]** button.
1. On the Crop Editor page, do one of the following:

    * To trim color pixels, click **[!UICONTROL Trim]** > **[!UICONTROL Color]**. The Auto Crop By Color dialog box appears. Click the **[!UICONTROL Corner]** menu and choose a corner with the background color to crop away. Then enter a **[!UICONTROL Tolerance]** setting from 0 through 1. The 0 setting crops pixels only if they exactly match the color you selected in the corner of the image. Numbers closer to 1 allow for more color difference. Click the **[!UICONTROL Crop]** button.
    * To trim transparent pixels, select click **[!UICONTROL Trim]** > **[!UICONTROL Transparent]**. The Auto Crop By Transparency dialog box appears. Enter a tolerance setting from 0 through 1. The 0 setting crops pixels only if they are transparent. Numbers closer to 1 allow for more transparency. Click **[!UICONTROL Crop]**.

1. Click **[!UICONTROL Save]**.

>[!NOTE]
>
>To restore an image to its original state after you’ve cropped it, display the image in the Crop Editor screen and click **[!UICONTROL Reset]**.

## Select an area to crop {#select-an-area-to-crop}

1. To crop an image, click its rollover **[!UICONTROL Edit]** button, and choose **[!UICONTROL Crop]**, or display it in the Browse Panel in Detail view and click **[!UICONTROL Crop]**.

1. In the Crop Editor window, place the part of the image you do not want to crop in the crop box. What appears inside the box is what remains when you click **[!UICONTROL Save]** and crop the image.
1. To adjust the crop area, do one of the following:

    * Drag a side or corner of the box. Hold down the Shift key as you drag to change size but maintain the aspect ratio (the shape) of the crop box.
    * Enter pixel measurements in the Size boxes.
    * Drag to move the crop box. Move the pointer inside the boundary of the box. When you see the four-headed arrow, drag the box to a new location on the image.

1. Click **[!UICONTROL Save]**.

>[!NOTE]
>
>To restore an image to its original state after you have cropped it, display the image in the Crop Editor screen and click **[!UICONTROL Reset]**.

>[!MORELIKETHIS]
>
>* [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Cropping white space from a PDF file](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Cropping from the sides of PDF pages](pdfs.md#cropping_from_the_sides_of_pdf_pages)
