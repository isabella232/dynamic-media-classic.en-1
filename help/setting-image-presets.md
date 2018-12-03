---
title: Setting up Image Presets
seo-title: Setting up Image Presets
description: null
seo-description: Learn how to set up Image Presets.
uuid: 5127ea29-d89c-4b0a-8d2b-2af2634797c2
contentOwner: admin
cq-gepid: scene7/using/WS2F6A1049-B41F-447d-A520-91227F9CDABF,scene7/using/WS8367FCD9-ABD6-41c0-B5EC-C0313562296F
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: ba998bcd-4f70-4c90-8ded-5395e2bd99cb
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 44.557-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/image_sizing;/content/help/en/experience-manager/morehelp/image_sizing
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Setting up Image Presets{#setting-up-image-presets}

Like a macro, an Image Preset is a predefined collection of sizing and formatting commands saved under a name. To understand how Image Presets work, suppose your web site requires each product image to appear at two different sizes: 500 x 500 pixels and 150 x 150 pixels. You create two Image Presets, one called “Enlarge” to display images at 500x500 pixels and one called “Thumbnail” to display images at 150 x 150 pixels. To deliver images at the “Enlarge” and “Thumbnail” size, a Scene7 Image Server looks up the definition of the Enlarge Image Preset and Thumbnail Image Preset. Then the server dynamically generates an image at the size and formatting specifications of each Image Preset.

Scene7 comes with several “best practice” Image Presets that are already set up for you to use. Administrators can create new Image Presets as well. To create an Image Preset, you can start from scratch or you can start from an existing one and save it under a new name.

Images that are reduced in size when they are delivered dynamically from a server can lose sharpness and detail. For this reason, each Image Preset contains formatting controls for optimizing an image when it is delivered at a particular size. These controls make sure that your images are sharp and clear when they are delivered to your web site or application.

## Creating an Image Preset {#creating-an-image-preset}

You can create your own Image Presets if you are a company administrator. You can create new Image Presets or start with a default Image Preset that Scene7 provides, edit it, and save it with a new name.

**To create an Image Preset**

1. Click **Setup** &gt; **Image Presets**.

   You can browse to an Image Preset name on this screen to preview an existing Image Preset. When you select an Image Preset name, the sample image in the Preview window changes size and appearance.

1. Do one of the following:

   **Creating an&#xA;Image Preset** Click Add.

   **Editing an Image Preset** Browse to the Image Preset that is most like the one you want to create and then click Edit.

1. Enter a name for the Image Preset.
1. Enter Width and Height measurements in pixels. These measurements determine the size at which images are delivered.
1. Fill in the Add Preset or Edit Preset screen. For details, see [Image Preset options](application-setup.md#image_preset_options).

   Scene7 recommends these “best practice” option choices to start:

   **Format** Choose JPEG or another format that meets your requirements. All web browsers support the JPEG image format; it offers a good balance between small files sizes and image quality. However, JPEG format images use a lossy compression scheme that can introduce unwanted image artifacts if the compression setting is too low. For that reason, Scene7 recommends setting the compression quality (on the slider) to 75. This setting offers a good balance between image quality and small file size.

   **Sharpening** Do not select Sharpening (this sharpening filter offers less control than Unsharp Masking settings).

   **Resample Mode** Choose Bi-Cubic.

   **Unsharp Masking (USM) options** Enter the settings shown here:

<table border="1" cellpadding="4" cellspacing="0" frame="border" rules="all" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e14523" valign="top" width="NaN%"><p>Preset type</p></th> 
   <th class="cellrowborder" id="d19e14526" valign="top" width="NaN%"><p>Size</p></th> 
   <th class="cellrowborder" id="d19e14529" valign="top" width="NaN%"><p>USM: Amount</p></th> 
   <th class="cellrowborder" id="d19e14532" valign="top" width="NaN%"><p>USM: Radius</p></th> 
   <th class="cellrowborder" id="d19e14535" valign="top" width="NaN%"><p>USM: Threshold</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e14523 " valign="top" width="NaN%"><p>Cross-Sell (mini-thumbnail)</p></td> 
   <td class="cellrowborder" headers="d19e14526 " valign="top" width="NaN%"><p>75 x 75</p></td> 
   <td class="cellrowborder" headers="d19e14529 " valign="top" width="NaN%"><p>1.5</p></td> 
   <td class="cellrowborder" headers="d19e14532 " valign="top" width="NaN%"><p>0.8</p></td> 
   <td class="cellrowborder" headers="d19e14535 " valign="top" width="NaN%"><p>5</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e14523 " valign="top" width="NaN%"><p>Thumbnail</p></td> 
   <td class="cellrowborder" headers="d19e14526 " valign="top" width="NaN%"><p>150 x 150</p></td> 
   <td class="cellrowborder" headers="d19e14529 " valign="top" width="NaN%"><p>1.1</p></td> 
   <td class="cellrowborder" headers="d19e14532 " valign="top" width="NaN%"><p>1</p></td> 
   <td class="cellrowborder" headers="d19e14535 " valign="top" width="NaN%"><p>5</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e14523 " valign="top" width="NaN%"><p>Main</p></td> 
   <td class="cellrowborder" headers="d19e14526 " valign="top" width="NaN%"><p>350 x 350</p></td> 
   <td class="cellrowborder" headers="d19e14529 " valign="top" width="NaN%"><p>1</p></td> 
   <td class="cellrowborder" headers="d19e14532 " valign="top" width="NaN%"><p>1</p></td> 
   <td class="cellrowborder" headers="d19e14535 " valign="top" width="NaN%"><p>6</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e14523 " valign="top" width="NaN%"><p>Enlarge</p></td> 
   <td class="cellrowborder" headers="d19e14526 " valign="top" width="NaN%"><p>500 x 500</p></td> 
   <td class="cellrowborder" headers="d19e14529 " valign="top" width="NaN%"><p>1.2</p></td> 
   <td class="cellrowborder" headers="d19e14532 " valign="top" width="NaN%"><p>1.2</p></td> 
   <td class="cellrowborder" headers="d19e14535 " valign="top" width="NaN%"><p>5</p></td> 
  </tr> 
 </tbody> 
</table>

1. Click **Save**.

The Scene7 “best practice” options for creating Image Presets listed here are general recommendations; sharpening is highly subjective. These “best practice” settings were based on a 2000 x 2000 master image; settings for larger or smaller masters can be different. If you want to adjust the Unsharp Masking settings, Scene7 recommends these ranges:

**Amount** Between .8 and 1.5.

**Radius** Between .6 and 2.

**Threshold** From 1-6.

To delete an Image Preset, select it on the Image Presets screen and select the Delete button.

>[!MORE_LIKE_THIS]
>
>* [Create and edit Image Presets](application-setup.md#creating_and_editing_image_presets)
>* [Image Preset options](application-setup.md#image_preset_options)
>* [Previewing an image asset based on its Image Preset](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
