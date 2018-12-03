---
title: Creating a Mixed Media Set
seo-title: Creating a Mixed Media Set
description: null
seo-description: Learn how to create a Mixed Media Set.
uuid: cc66d1af-f26d-40d5-af94-8c5f4460736c
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WS37cb61f8f3397d86-5c360d211229a65e45b-7ffb,scene7/using/WS37cb61f8f3397d86-5c360d211229a65e45b-7ff7,scene7/using/WS37cb61f8f3397d86-5c360d211229a65e45b-7ff4,scene7/using/WS402157739dd65419-ca9d1ac146c994663d-8000
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 4ac74c08-9f0d-4114-9d40-2ebaef304130
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 42.798-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/mixed_media_sets;/content/help/en/experience-manager/morehelp/mixed_media_sets
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Creating a Mixed Media Set{#creating-a-mixed-media-set}

Create a Mixed Media Set when you want to combine multiple types of viewers in one presentation. Make sure your files, Image Sets, Swatch Sets, and Spin Sets are ready to publish before you add them to the Mixed Media Set.

![]() 

## Create a Mixed Media Set {#create-a-mixed-media-set}

When you create a set, the **Publish after save** option affects the set and set members in the following ways:

<table border="1" cellpadding="4" cellspacing="0" frame="border" rules="all" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e25484" valign="top" width="NaN%"><p>“Publish after save” option selected before saving?</p></th> 
   <th class="cellrowborder" id="d19e25487" valign="top" width="NaN%"><p>State of set after saving</p></th> 
   <th class="cellrowborder" id="d19e25490" valign="top" width="NaN%"><p>State of set members after saving</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e25484 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e25487 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e25490 " valign="top" width="NaN%"><p>Published</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e25484 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e25487 " valign="top" width="NaN%"><p>Unpublished</p></td> 
   <td class="cellrowborder" headers="d19e25490 " valign="top" width="NaN%"><p>Set members retain their published or unpublished state.</p></td> 
  </tr> 
 </tbody> 
</table>

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To create a Mixed Media Set**

1. Click **Build** &gt; **Mixed Media Sets**.
1. Drag the videos, Image Sets, Spin Sets, and swatches from the Asset Library to the Mixed Media Set screen.

   >[!NOTE]
   >
   >Mixed Media Sets do not support assets with filenames that contain any of the following characters: ( ) { }.

1. Do any of the following:

    * To add a soundtrack, drag an audio file from the Asset Library to the Soundtrack box. The soundtrack plays while images are displayed. It stops when video is played.
    * To change the order of sets, drag them to new locations on the Mixed Media Set screen. The order of sets on the screen determines the left-to-right order in which users see sets in the Mixed Media Set Viewer.
    * (Optional) To add a custom thumbnail to represent a video in the Viewer, drag an image file from the Asset Library to the Thumbnail placeholder box.

1. Near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Save**, select a folder for storing your Mixed Media Set, enter a name for the set, and click **Save**.

   Click **Preview** to see what your combo Image Set looks like in an Image Set Viewer.

## Edit a Mixed Media Set {#edit-a-mixed-media-set}

You can edit a Mixed Media Set. If you want to edit a set within a Mixed Media Set, open that set separately, edit it, and save it. The edits appear in the Mixed Media set.

Depending on whether you edit a published or an unpublished set, the **Publish after save** option affects the set and set members in the following ways:

<table border="1" cellpadding="4" cellspacing="0" frame="border" rules="all" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e25597" valign="top" width="NaN%"><p>Set already published?</p></th> 
   <th class="cellrowborder" id="d19e25600" valign="top" width="NaN%"><p>“Publish after save” option selected before saving your edit?</p></th> 
   <th class="cellrowborder" id="d19e25603" valign="top" width="NaN%"><p>State of set after saving</p></th> 
   <th class="cellrowborder" id="d19e25606" valign="top" width="NaN%"><p>State of set members after saving</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e25597 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e25600 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e25603 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e25606 " valign="top" width="NaN%"><p>Published</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e25597 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e25600 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e25603 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e25606 " valign="top" width="NaN%"><p>Existing set members retain their published state.</p><p>Any new set members that you added during your edit retain their published or unpublished state.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e25597 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e25600 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e25603 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e25606 " valign="top" width="NaN%"><p>Published</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e25597 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e25600 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e25603 " valign="top" width="NaN%"><p>Unpublished</p></td> 
   <td class="cellrowborder" headers="d19e25606 " valign="top" width="NaN%"><p>Existing set members and any new set members that you added during your edit retain their published or unpublished state.</p></td> 
  </tr> 
 </tbody> 
</table>

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To edit a Mixed Media Set**

1. Click the Mixed Media Set’s rollover **Edit** button. 
1. Do any of the following:

    * To remove items, select them and click **Delete**.
    * To reorder items, drag them to new locations.

1. When you are finished editing the set, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Save** or **Save As**.

## Deleting a Mixed Media Set {#deleting-a-mixed-media-set}

When you delete a set, the set itself is moved to the Trash. However, the members (or “children”) within that set are not affected; instead, they each retain their existing published or unpublished state.

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To delete a Mixed Media Set**

1. In the Grid View, List View, or Details View, select one or more Mixed Media Sets.
1. On the Global Navigation Bar, click **File** &gt; **Delete** &gt; **Delete**.

