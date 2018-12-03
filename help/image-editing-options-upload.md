---
title: Image editing options at upload
seo-title: Image editing options at upload
description: null
seo-description: Learn about the image editing options that are available at the time of upload.
uuid: 256a25cb-8e76-4a68-9d79-ed5b1d7fdb66
contentOwner: admin
cq-gepid: scene7/using/WS1C6180F2-3FB5-4222-BB0F-08C53AB21188
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 935959d4-0935-4540-ac8d-89d92dce4943
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 43.420-0400
lr-lastmodifiedby: admin
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Image editing options at upload{#image-editing-options-at-upload}

When uploading image files, including AI, EPS, and PSD files, you can take the following editing actions in the Upload Job Options dialog box:

* Crop white space from the edge of images.
* Crop manually from the sides of images.
* Choose a color profile.
* Create a mask from a clipping path. 
* Sharpen images with unsharp masking options
* Knockout Background

These options are located on the Upload screen under Image Editing Options.

**Cropping white space from images**

To automatically crop white-space pixels from an image, select the Crop menu and choose Trim. Then choose these options:

**Trim&#xA;Away Based On** Choose whether to crop based on color or transparency:

**Color** Choose the Color option. Then, from the Corner drop-down list, select the corner of the image with the color that best represents the white-space color you want to crop.

**Transparency** Choose the Transparency option.

**Tolerance** Drag the slider to specify a tolerance from 0 through 1:

**Trimming based on color** Specify 0 to crop pixels only if they exactly match the color you selected in the corner of the image. Numbers closer to 1 allow for more color difference.

**Trimming based on transparency** Specify 0 to crop pixels only if they are totally transparent; numbers closer to 1 allow for more transparency.

**Cropping manually from the sides of images**

To manually crop from the sides of an image, select the Crop menu and choose Manual. Then enter the number of pixels to crop from any side or each side of the image. How much of the image is cropped depends on the ppi (pixels per inch) setting in the image file. For example, if the image displays 150 ppi and you enter 75 in the Top, Right, Bottom, and Left text boxes, a half-inch is cropped from each side.

**Choosing a color profile**

Choose a Color Profile option to select a color space for the image:

**Convert To sRGB** Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages.

**Keep Original Color Space** Retains the original color space.

**Custom From &gt; To** Opens menus so you can choose a Convert From and Convert To color space. You can choose a standard Photoshop color space or a color space you uploaded to SPS.

See [ICC profiles](icc-profiles.md#icc_profiles).

**Creating a mask from a clipping path**

Select **Create Mask From Clipping Path** to create a mask for the image based on its clipping path information. This option applies to images created with image-editing applications in which a clipping path was created.

**Sharpening an image using Unsharpen Mask**

This filter lets you fine-tune a sharpening filter effect on the final downsampled image, controlling the intensity of the effect, the radius of the effect (as measured in pixels), and a threshold of contrast that is ignored.

This effect uses the same options as Photoshop’s Unsharp Mask filter. Contrary to what the name suggests, Unsharp Mask is a sharpening filter.

Under Unsharp Masking, set the options you want. Setting options are described in the following table:

<table border="1" cellpadding="4" cellspacing="0" frame="border" id="WS77bcfb314d2978e71e03f6841611f94f84d-7f6b" rules="all" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e30288" valign="top" width="NaN%"><p>Unsharp Mask options</p></th> 
   <th class="cellrowborder" id="d19e30291" valign="top" width="NaN%"><p>Description</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e30288 " valign="top" width="NaN%"><p>Amount</p></td> 
   <td class="cellrowborder" headers="d19e30291 " valign="top" width="NaN%"><p>Controls the amount of contrast that is applied to edge pixels.</p><p>Think of it as the intensity of the effect. The main difference between the amount values of Unsharp Mask in SPS and the amount values in Adobe Photoshop, is that Photoshop has an amount range of 1% to 500%. Whereas, in SPS, the value range is 0.0 to 5.0. A value of 5.0 in SPS is the rough equivalent of 500% in Photoshop; a value of 0.9 is the equivalent of 90%, and so on. </p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e30288 " valign="top" width="NaN%"><p>Radius</p></td> 
   <td class="cellrowborder" headers="d19e30291 " valign="top" width="NaN%"><p>Controls the radius of the effect. The value range is 0-250.</p><p>The effect is run on all pixels in an image and radiates out from all pixels in all directions. The radius is measured in pixels. For example, to get a similar sharpening effect for a 2000 x 2000 pixel image and 500 x 500 pixel image, you would set a radius of two pixels on the 2000 x 2000 pixel image and a radius value of one pixel on the 500 x 500 pixel image. A larger value is used for an image that has more pixels.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e30288 " valign="top" width="NaN%"><p>Threshold</p></td> 
   <td class="cellrowborder" headers="d19e30291 " valign="top" width="NaN%"><p>Threshold is a range of contrast that is ignored when the Unsharp Mask filter is applied. This is important so that no "noise" is introduced to an image when this filter is used. The value range is 0-255, which is the number of brightness steps in a grayscale image. 0=black, 128=50% gray and 255=white.</p><p>For example, a threshold value of 12 ignores slight variations is skin tone brightness to avoid adding noise, but still add edge contrast to contrasty areas such as where eyelashes meet skin.</p><p>For example, if you have a photo of someone’s face, the Unsharp Mask affects the contrasty parts of the image, such as where eyelashes and skin meet to create an obvious area of contrast, and the smooth skin itself. Even the smoothest skin exhibits subtle changes in brightness values. If you do not use a threshold value, the filter accentuates these subtle changes in skin pixels. In turn, a noisy and undesirable effect is created while contrast on the eyelashes is increased, enhancing sharpness.</p><p>To avoid this issue, a threshold value is introduced that tells the filter to ignore pixels that do not change contrast dramatically, like smooth skin. </p><p>In the zipper graphic shown earlier, notice the texture next to the zippers. Image noise is exhibited because the threshold values were too low to suppress the noise.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e30288 " valign="top" width="NaN%"><p>Monochrome</p></td> 
   <td class="cellrowborder" headers="d19e30291 " valign="top" width="NaN%"><p>Select to unsharp-mask image brightness (intensity).</p><p>Deselect to unsharp-mask each color component separately.</p></td> 
  </tr> 
 </tbody> 
</table>

See also [Sharpening an image](sharpening-image.md#sharpening_an_image).

See also [Sharpening images in Scene7 Publishing System and on Image Server](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

**Knockout Background**

You can use Knockout Background to automatically remove the background of an image when you upload it. This technique is useful to draw attention to a particular object and make it stand out from a busy background.

<table border="1" cellpadding="4" cellspacing="0" frame="border" id="WS77bcfb314d2978e71e03f6841611f94f84d-7f69" rules="all" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e30359" valign="top" width="NaN%"><p>KnockOut Background options</p></th> 
   <th class="cellrowborder" id="d19e30362" valign="top" width="NaN%"><p>Description</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e30359 " valign="top" width="NaN%"><p>Knockout Background</p></td> 
   <td class="cellrowborder" headers="d19e30362 " valign="top" width="NaN%"><p>Select to enable or “turn on” the Knockout Background feature and options..</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e30359 " valign="top" width="NaN%"><p>Corner</p></td> 
   <td class="cellrowborder" headers="d19e30362 " valign="top" width="NaN%"><p>Required.</p><p>The corner of the image that is used to define the background color to knockout.</p><p>You can choose from <strong>Upper Left</strong>, <strong>Bottom Left</strong>, <strong>Upper Right</strong>, or <strong>Bottom Right</strong>.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e30359 " valign="top" width="NaN%"><p>Fill Method</p></td> 
   <td class="cellrowborder" headers="d19e30362 " valign="top" width="NaN%"><p>Required. </p><p>Controls pixel transparency from the Corner location that you set.</p><p>You can choose from the following fill methods:</p> 
    <ul> 
     <li><p><strong>Flood Fill</strong> - turns all pixels transparent that match the Corner that you have specified and are connected to it.</p></li> 
     <li><p><strong>Match Pixel</strong> - turns all matching pixels transparent, regardless of their location on the image.</p></li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e30359 " valign="top" width="NaN%"><p>Tolerance</p></td> 
   <td class="cellrowborder" headers="d19e30362 " valign="top" width="NaN%"><p>Optional.</p><p>Controls the allowable amount of variation in pixel color matching based on the Corner location that you set.</p><p>Use a value of 0.0 to match pixel colors exactly or, use a value of 1.0 to allow for the greatest variation.</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORE_LIKE_THIS]
>
>* [Cropping an image](cropping-image.md#cropping_an_image)
