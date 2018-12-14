---
title: Creating an Image Set
seo-title: Creating an Image Set
description: null
seo-description: Learn how to create an Image Set.
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
index: y
internal: n
snippet: y
---

# Creating an Image Set{#creating-an-image-set}

To create a multiple-view Image Set, you need images that show an item from different points of view or show different aspects of the same item. The goal is to present viewers with images of an item so they get a solid idea of what an item looks like or does.

## Creating an Image Set {#creating-an-image-set}

When you create a set, the **Publish after save** option affects the set and set members in the following ways:

<table border="1" cellpadding="4" cellspacing="0" frame="border" rules="all" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e17271" valign="top" width="NaN%"><p>“Publish after save” option selected before saving?</p></th> 
   <th class="cellrowborder" id="d19e17274" valign="top" width="NaN%"><p>State of set after saving</p></th> 
   <th class="cellrowborder" id="d19e17277" valign="top" width="NaN%"><p>State of set members after saving</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e17271 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e17274 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e17277 " valign="top" width="NaN%"><p>Published</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e17271 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e17274 " valign="top" width="NaN%"><p>Unpublished</p></td> 
   <td class="cellrowborder" headers="d19e17277 " valign="top" width="NaN%"><p>Set members retain their published or unpublished state.</p></td> 
  </tr> 
 </tbody> 
</table>

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To create an Image Set**

1. Do one of the following:

   **Select the&#xA;images first** In the Browse Panel, select the images you want for your Image Set, click Build > Image Sets.

   **Start from the Image Set screen** Click Build > Image Sets. The Image Set screen opens. Select a folder in the Asset Library and drag the images you want for your Image Set onto the Image Set screen.

1. To change the order of images, drag the images to new locations.
1. Near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Save**, select a folder for storing your Image Set, enter a name for the set, and then click **Save**.
1. To see your Image Set in the Image Set Viewer, click **Preview** on the Image Set screen. You can click swatch thumbnails in the Image Set Viewer to see how they behave.

## Editing an Image Set {#editing-an-image-set}

Depending on whether you edit a published or an unpublished set, the **Publish after save** option affects the set and set members in the following ways:

<table border="1" cellpadding="4" cellspacing="0" frame="border" rules="all" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e17385" valign="top" width="NaN%"><p>Set already published?</p></th> 
   <th class="cellrowborder" id="d19e17388" valign="top" width="NaN%"><p>“Publish after save” option selected before saving your edit?</p></th> 
   <th class="cellrowborder" id="d19e17391" valign="top" width="NaN%"><p>State of set after saving</p></th> 
   <th class="cellrowborder" id="d19e17394" valign="top" width="NaN%"><p>State of set members after saving</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e17385 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e17388 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e17391 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e17394 " valign="top" width="NaN%"><p>Published</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e17385 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e17388 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e17391 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e17394 " valign="top" width="NaN%"><p>Existing set members retain their published state.</p><p>Any new set members that you added during your edit retain their published or unpublished state.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e17385 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e17388 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e17391 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e17394 " valign="top" width="NaN%"><p>Published</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e17385 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e17388 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e17391 " valign="top" width="NaN%"><p>Unpublished</p></td> 
   <td class="cellrowborder" headers="d19e17394 " valign="top" width="NaN%"><p>Existing set members and any new set members that you added during your edit retain their published or unpublished state.</p></td> 
  </tr> 
 </tbody> 
</table>

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To edit an Image Set**

1. In the Grid view, browse to an ImageSet, and then below the image, click **Edit**.
1. Do any of the following:

    * To add an image (published or unpublished), drag it from a folder in Add Assets onto the Image Set’s **Views** page.
    * To remove an image, select it, and then click **Delete** on the toolbar.
    * To reorder images, drag an image to a new position.

1. When you are finished editing the set, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Save**, select a storage folder for your set, enter a name for the set, and then click **Save**.

## Deleting an Image Set {#deleting-an-image-set}

When you delete a set, the set itself is moved to the Trash. However, the members (or “children”) within that set are not affected; instead, they each retain their existing published or unpublished state.

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To delete an Image Set**

1. In the Grid View, List View, or Details View, select one or more Image Sets.
1. On the Global Navigation Bar, click **File** &gt; **Delete** &gt; **Delete**.

