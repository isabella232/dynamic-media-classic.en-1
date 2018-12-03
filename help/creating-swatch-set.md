---
title: Creating a Swatch Set
seo-title: Creating a Swatch Set
description: null
seo-description: Learn how to create a swatch set.
uuid: 2675aeb1-4176-438b-b06a-0e76cae345e0
contentOwner: admin
cq-gepid: scene7/using/WS37cb61f8f3397d86-1045e5c5123106176ad-7ffb,scene7/using/WS37cb61f8f3397d86-1045e5c5123106176ad-7ffa,scene7/using/WS42c677b49dfa3d1d-142a3d59146b5c2eef3-8000,scene7/using/WS42c677b49dfa3d1d4b49c609146b5c2198a-8000
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 25df287c-7324-4f3f-b206-940981756896
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 42.949-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/swatch_sets;/content/help/en/experience-manager/morehelp/swatch_sets
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Creating a Swatch Set{#creating-a-swatch-set}

A Swatch Set gives users the opportunity to view an item in a different color, pattern, or finish. To create a Swatch Set with color swatches, you need one image for each different color, pattern, or finish you want to present to users. You also need one color, pattern, or finish swatch for each color, pattern, or finish.

For example, suppose you want to present images of caps with different color bills; the bills are red, green, and blue. In this case, you need three shots of the same cap. You need one shot with a red, one with a green, and one with a blue bill. You also need a red, green, and blue color swatch. The color swatches serve as the thumbnails that users click in the Swatch Set Viewer to see the red-billed, green-billed, or blue-billed cap.

## Creating a Swatch Set {#creating-a-swatch-set}

When you create a set, the **Publish after save** option affects the set and set members in the following ways:

<table border="1" cellpadding="4" cellspacing="0" frame="border" rules="all" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e18178" valign="top" width="NaN%"><p>“Publish after save” option selected before saving?</p></th> 
   <th class="cellrowborder" id="d19e18181" valign="top" width="NaN%"><p>State of set after saving</p></th> 
   <th class="cellrowborder" id="d19e18184" valign="top" width="NaN%"><p>State of set members after saving</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e18178 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e18181 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e18184 " valign="top" width="NaN%"><p>Published</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e18178 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e18181 " valign="top" width="NaN%"><p>Unpublished</p></td> 
   <td class="cellrowborder" headers="d19e18184 " valign="top" width="NaN%"><p>Set members retain their published or unpublished state.</p></td> 
  </tr> 
 </tbody> 
</table>

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To create a Swatch Set**

1. Do one of the following:

   **Select the&#xA;images first** In the Browse Panel, select the images, and then click Build > Swatch Sets.

   **Start from the Swatch Set screen** Click Build > Swatch Sets. Select a folder in the Asset Library and drag the images onto the Views section of the Swatch Set page.

1. Drag swatch colors, patterns, or finishes into the Swatches placeholder box on the Swatch Set page.

   Make sure that the color, pattern, or finish swatch you drag into each placeholder represents the color, pattern, or finish of the adjacent image.

1. To change the order of images in your Swatch Set, drag the images to new locations.
1. Near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Save**, select a folder for storing your color swatch Swatch Set, enter a name for the set, and click Submit.
1. To see your Swatch Set in the Swatch Set Viewer, click **Preview** on the Swatch Set screen. You can click swatch thumbnails in the Swatch Set Viewer to see how they behave.

## Editing a Swatch Set {#editing-a-swatch-set}

Depending on whether you edit a published or an unpublished set, the **Publish after save** option affects the set and set members in the following ways:

<table border="1" cellpadding="4" cellspacing="0" frame="border" rules="all" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e18294" valign="top" width="NaN%"><p>Set already published?</p></th> 
   <th class="cellrowborder" id="d19e18297" valign="top" width="NaN%"><p>“Publish after save” option selected before saving your edit?</p></th> 
   <th class="cellrowborder" id="d19e18300" valign="top" width="NaN%"><p>State of set after saving</p></th> 
   <th class="cellrowborder" id="d19e18303" valign="top" width="NaN%"><p>State of set members after saving</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e18294 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e18297 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e18300 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e18303 " valign="top" width="NaN%"><p>Published</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e18294 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e18297 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e18300 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e18303 " valign="top" width="NaN%"><p>Existing set members retain their published state.</p><p>Any new set members that you added during your edit retain their published or unpublished state.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e18294 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e18297 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e18300 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e18303 " valign="top" width="NaN%"><p>Published</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e18294 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e18297 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e18300 " valign="top" width="NaN%"><p>Unpublished</p></td> 
   <td class="cellrowborder" headers="d19e18303 " valign="top" width="NaN%"><p>Existing set members and any new set members that you added during your edit retain their published or unpublished state.</p></td> 
  </tr> 
 </tbody> 
</table>

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To edit a Swatch Set**

1. In the Grid view, browse to an SwatchSet, and then below the image, click **Edit**.
1. Do any of the following:

    * To add an image (published or unpublished), drag it from a folder in Add Assets onto the Swatch Set’s **Views** page.
    * To remove an image, select it, and then click **Delete** on the toolbar.
    * To reorder images, drag an image to a new position.

1. When you are finished editing the set, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Save**, select a storage folder, enter a name for the set, and then click **Save**.

## Deleting a Swatch Set {#deleting-a-swatch-set}

When you delete a set, the set itself is moved to the Trash. However, the members (or “children”) within that set are not affected; instead, they each retain their existing published or unpublished state.

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To delete a Swatch Set**

1. In the Grid View, List View, or Details View, select one or more Swatch Sets.
1. On the Global Navigation Bar, click **File** &gt; **Delete** &gt; **Delete**.

