---
title: Image fine-tuning options at upload
description: Learn about the image fine-tuning options that are available at the time of upload in Adobe Dynamic Media Classic.
uuid: 0912ae6f-41c9-41b5-94d1-e266face782e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: d3f21cdf-2cb3-46e8-955a-b8daf0b233bc
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
---
# Image fine-tuning options at upload{#image-editing-options-at-upload}

When uploading image files, including AI, EPS, and PSD files, you can take the following editing actions in the Upload Job Options dialog box:

* Crop white space from the edge of images.
* Crop manually from the sides of images.
* Choose a color profile.
* Create a mask from a clipping path. 
* Sharpen images with unsharp masking options
* Knockout Background

These options are on the Upload page under the **[!UICONTROL Imaging Edit Options]** heading.

## Crop white space from images

To automatically crop white-space pixels from an image, on the Upload Job Options dialog box, select **[!UICONTROL Crop Options]**. In the **[!UICONTROL Crop]** drop-down list, choose **[!UICONTROL Trim]**. Then choose these options:

* **[!UICONTROL Trim Away Based On]** - From this drop-down list, choose whether to crop based on color or transparency:

  * **[!UICONTROL Color]** - Choose the **[!UICONTROL Color]** option. Then, from the **[!UICONTROL Corner]** drop-down list, select the corner of the image with the color that best represents the white-space color you want to crop.

  * **[!UICONTROL Transparency]** - Choose the Transparency option.

* **[!UICONTROL Tolerance]** - Drag the slider to specify a tolerance from 0 through 1:

  * **Trimming based on color** - Specify 0 to crop pixels only if they exactly match the color you selected in the corner of the image. Numbers closer to 1 allow for more color difference.

  * **Trimming based on transparency** - Specify 0 to crop pixels only if they are transparent; numbers closer to 1 allow for more transparency.

## Crop manually from the sides of images

To manually crop from the sides of an image, select the Crop menu and choose Manual. Then enter the number of pixels to crop from any side or each side of the image. How much of the image is cropped depends on the ppi (pixels per inch) setting in the image file. For example, if the image displays 150 ppi and you enter 75 in the Top, Right, Bottom, and Left text boxes, a half-inch is cropped from each side.

## Choose a color profile

To select a color space for the image, choose a Color Profile option:

* **[!UICONTROL Convert To sRGB]** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages.

* **[!UICONTROL Keep Original Color Space]** - Retains the original color space.

* **[!UICONTROL Custom From]** > **[!UICONTROL To]** - Opens menus so you can choose a Convert From and Convert To color space. You can choose a standard Photoshop color space or a color space you uploaded to Adobe Dynamic Media Classic.

See [ICC profiles](icc-profiles.md#icc_profiles).

## Create a mask from a clipping path

To create a mask for the image based on its clipping path information, select **[!UICONTROL Create Mask From Clipping Path]**. This option applies to images created with image-editing applications in which a clipping path was created.

## Sharpen an image using Unsharpen Mask

This filter lets you fine-tune a sharpening filter effect on the final downsampled image. It helps you control the intensity of the effect, the radius of the effect (as measured in pixels), and a threshold of contrast that is ignored.

This effect uses the same options as Photoshop’s Unsharp Mask filter. Contrary to what the name suggests, Unsharp Mask is a sharpening filter.

Under Unsharp Masking, set the options you want. Setting options are described in the following table:

| Unsharp Mask options |Description |
| --- | --- |
| Amount | Controls the amount of contrast that is applied to edge pixels.<br><br>Think of it as the intensity of the effect. The main difference between the amount values of Unsharp Mask in Adobe Dynamic Media Classic and the amount values in Adobe Photoshop, is that Photoshop has an amount range of 1% to 500%. Whereas in Adobe Dynamic Media Classic, the value range is 0.0 to 5.0. A value of 5.0 in Adobe Dynamic Media Classic is the rough equivalent of 500% in Photoshop; a value of 0.9 is the equivalent of 90%, and so on. |
| Radius | Controls the radius of the effect. <br><br>The value range is 0-250. The effect is run on all pixels in an image and radiates out from all pixels in all directions. The radius is measured in pixels. For example, to get a similar sharpening effect for a 2000 x 2000 pixel image and 500 x 500 pixel image, you would set a radius of two pixels on the 2000 x 2000 pixel image. Then set a radius value of one pixel on the 500 x 500 pixel image. A larger value is used for an image that has more pixels. |
| Threshold | Threshold is a range of contrast that is ignored when the Unsharp Mask filter is applied. This effect is important so that no "noise" is introduced to an image when this filter is used. The value range is 0-255, which is the number of brightness steps in a grayscale image. 0=black, 128=50% gray and 255=white.<br><br>For example, a threshold value of 12 ignores slight variations is skin tone brightness to avoid adding noise, but still add edge contrast to contrasty areas such as where eyelashes meet skin.<br><br>For example, if you have a photo of someone’s face, the Unsharp Mask affects the contrasty parts of the image. For example, where eyelashes and skin meet to create an obvious area of contrast, and the smooth skin itself. Even the smoothest skin exhibits subtle changes in brightness values. If you do not use a threshold value, the filter accentuates these subtle changes in skin pixels. In turn, a noisy and undesirable effect is created while contrast on the eyelashes is increased, enhancing sharpness.<br><br>To avoid this issue, a threshold value is introduced that tells the filter to ignore pixels that do not change contrast dramatically, like smooth skin. <br><br>In the zipper graphic shown earlier, notice the texture next to the zippers. Image noise is exhibited because the threshold values were too low to suppress the noise. |
| Monochrome | Select to unsharp-mask image brightness (intensity).<br><br>Deselect to unsharp-mask each color component separately. |

See also [Sharpen an image](sharpening-image.md#sharpening_an_image).

See also [Sharpen images in Adobe Dynamic Media and on Image Server](/help/assets/s7_sharpening_images.pdf).

## Knockout Background

You can use Knockout Background to automatically remove the background of an image when you upload it. This technique is useful to draw attention to a particular object and make it stand out from a busy background.

| KnockOut Background options | Description |
| --- | --- |
| Knockout Background | Select to enable or “turn on” the Knockout Background feature and options. |
| Corner | Required.<br>The corner of the image that is used to define the background color to knockout.<br>You can choose from <b>Upper Left, Bottom Left, Upper Right, or Bottom Right</b>.|
|Fill Method|Required. <br>Controls pixel transparency from the Corner location that you set.<br>You can choose from the following fill methods:<br>&bull; <b>Flood Fill</b> - turns all pixels transparent that match the Corner that you have specified and are connected to it.<br>&bull; <b>Match Pixel</b> - turns all matching pixels transparent, regardless of their location on the image. |
| Tolerance | Optional.<br>Controls the allowable amount of variation in pixel color matching based on the Corner location that you set.<br>Use a value of 0.0 to match pixel colors exactly or, use a value of 1.0 to allow for the greatest variation. |

>[!MORELIKETHIS]
>
>* [Crop an image](cropping-image.md#cropping_an_image)
