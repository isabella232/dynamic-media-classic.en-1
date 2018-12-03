---
title: Cropping an image
seo-title: Cropping an image
description: null
seo-description: Learn how to crop an image.
uuid: f10aaf77-24b8-4a56-8bab-60a1db670ad6
contentOwner: admin
cq-gepid: scene7/using/WSD6998310-4166-482a-9874-C8858B29FD34,scene7/using/WS3841FF00-F056-4612-8625-92F00D0A3960,scene7/using/WSFCE037B0-608D-4c81-BCE2-5DC70EBC0D61
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: e6005fe6-1763-433b-9ce0-e5a8775a641c
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 43.086-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/master_files;/content/help/en/experience-manager/morehelp/master_files
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Cropping an image{#cropping-an-image}

You can crop images in the Scene7 Publishing System. The system retains information about images that were cropped so you can restore them to their original state. You can also crop an image and save the cropped version under a new name.

You can crop an image to remove white space around it, or crop an area of the image.

>[!NOTE]
>
>After you crop, you can click the Save As button and save a cropped version of the image under a different name. In the Save As window, choose Save As New Master to save a second copy of the image. Choose Save As Addition View Of Master to save the original and its cropped version under a different name. Choose Replace Original to delete the original file from which you cropped your image. Then enter a name for the image and select the Submit button.

## Crop to remove white space around an image {#crop-to-remove-white-space-around-an-image}

You can crop off the transparent or solid-color pixels from the edge of an image.

1. To crop an image, click its rollover Edit button and choose Crop, or display it in the Browse Panel in Detail view and click the Crop button  ![](assets/Crop_up.png)

   . The Crop Editor screen opens.
1. Do one of the following:

    * To trim color pixels, select the Trim menu and choose Color. The Auto Crop By Color dialog box appears. Select the Corner menu and choose a corner with the background color to crop away. Then enter a Tolerance setting from 0 through 1. The 0 setting crops pixels only if they exactly match the color you selected in the corner of the image. Numbers closer to 1 allow for more color difference. Select the Crop button.
    * To trim transparent pixels, select the Trim menu and choose Transparent. The Auto Crop By Transparency dialog box appears. Enter a tolerance setting from 0 through 1. The 0 setting crops crop pixels only if they are totally transparent. Numbers closer to 1 allow for more transparency. Select the Crop button.

1. Click Save.

>[!NOTE]
>
>To restore an image to its original state after you’ve cropped it, display the image in the Crop Editor screen and select the Reset button.

## Select an area to crop {#select-an-area-to-crop}

1. To crop an image, click its rollover Edit button and choose **Crop**, or display it in the Browse Panel in Detail view and click **Crop** ![](assets/Crop_up.png).

1. In the Crop Editor window, place the part of the image you do not want to crop in the crop box. What appears inside the box remains when you click **Save** and crop the image.
1. To adjust the crop area, do one of the following:

    * Drag a side or corner of the box. Hold down the Shift key as you drag to change size but maintain the aspect ratio (the shape) of the crop box.
    * Enter pixel measurements in the Size boxes.
    * Drag to move the crop box. Move the pointer inside the boundary of the box. When you see the four-headed arrow, drag the box to a new location on the image.

1. Click **Save**.

>[!NOTE]
>
>To restore an image to its original state after you’ve cropped it, display the image in the Crop Editor screen and select the Reset button.

>[!MORE_LIKE_THIS]
>
>* [Image editing options at upload](image-editing-options-upload.md#image_editing_options_at_upload)
>* [Cropping white space from a PDF file](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Cropping from the sides of PDF pages](pdfs.md#cropping_from_the_sides_of_pdf_pages)
