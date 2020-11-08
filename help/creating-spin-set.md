---
title: Creating a Spin Set
seo-title: Creating a Spin Set
description: null
seo-description: Learn how to create a Spin Set.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf

---

# Creating a Spin Set{#creating-a-spin-set}

To create an effective Spin Set, make sure that you shoot the images correctly. You can create a Spin Set in Dynamic Media Classic by selecting the Build button and choosing Spin Sets. Edit Spin Sets in the Spin Sets screen.

>[!NOTE]
>
>Previous versions of Dynamic Media Classic did not offer two-dimensional Spin Sets. If you created a Spin Set in a previous version of Dynamic Media Classic, you cannot save your one-dimensional Spin Set without first saving it under a different name. Click Save As in the Spin Set screen and enter a new name so that you can edit it in Dynamic Media Classic.

## Guidelines for shooting Spin Set images {#guidelines-for-shooting-spin-set-images}

In general, the more images you have in a Spin Set, the better the image spinning effect is. However, including many images in the set also increases the amount of time it takes for the images to load. Dynamic Media Classic recommends these guidelines for shooting images for use in Spin Sets:

* At minimum, use 8-12 images in a one-dimensional spin set and 16-24 images in a two-dimensional Spin Set.
* Use a lossless format; TIFF and PNG are recommended.
* Mask all images so the item appears on a pure white or other high-contrast background. Optionally, add shadows.
* Make sure that product details are well lighted and in focus.
* Take spin images for fashion clothing with a mannequin or model. Often the mannequin is either completely masked (using a glass mannequin) or a stylized mannequin/dressform is shown in the image. You can create an on-model spin set by defining the number of angles. Mark each angle with tape on the floor to guide the model to step and look in the direction of each shot.

## Creating a Spin Set {#create}

Be aware that the order in which the Spin Set is authored or created in Dynamic Media Classic is important. Depending on how you order the assets when you drag and drop images into the grid on the Spin Set page, the Spin Set spins in a certain direction . Therfore, the order in which it is visually displayed in the builder is how the asset is spun when a user moves their mouse pointer or moves their finger, left to right.

When you create a set, the **Publish after save** option affects the set and set members in the following ways:

|“Publish after save” option selected before saving?|State of set after saving|State of set members after saving|
|--- |--- |--- |
|Yes|Published|Published|
|No|Unpublished|Set members retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually-publishing-assets) and [Manually unpublishing assets](publishing-files.md#manually-unpublishing-assets).

After you save a Spin Set, you can use Preview in the Build: Spin Set page to see what your Spin Set looks like in the default viewer.

**To create a Spin Set**

1. On the **Build** drop-down menu, click **Spin Sets**.
1. In the Spin Set Size dialog box, set the number of rows and cells that you want.

   To make a one-dimensional spin set, select one row only.

   To make a two-dimensional Spin Set, select two or more rows.

1. Click **OK**.
1. Drag and drop images into the grid on the Spin Set screen.
1. When you are finished, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Save**.
1. In the Save dialog box, select a folder for storing your spin set. In the File Name field, enter the spin set name.
1. Click **Save**.

## Editing a Spin Set {#editing-a-spin-set}

Depending on whether you edit a published set or an unpublished set, the **Publish after save** option affects the set and set members in the following ways:

|Set already published?|“Publish after save” option selected before saving your edit?|State of set after saving|State of set members after saving|
|--- |--- |--- |--- |
|Yes|Yes|Published|Published|
|Yes|No|Published|Existing set members retain their published state.Any new set members that you added during your edit retain their published or unpublished state.|
|No|Yes|Published|Published|
|No|No|Unpublished|Existing set members and any new set members that you added during your edit retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually-publishing-assets) and [Manually unpublishing assets](publishing-files.md#manually-unpublishing-assets).

**To edit a Spin Set**

1. Click the Spin Set’s rollover **Edit** button.
1. Do any of the following:

    * **Removing images**
    Select the image, and then click **Delete**.

    * **Adding images**
    Drag the image into a cell.

    * **Reordering rows (two-dimensional Spin Sets)**
    Click a row-selector box (to the left of the row) and then click **Move Row Down** or **Move Row Up**.

    * **Adding rows and cells**
    Enter a number in the Rows box and Cells box to determine the number of rows and the number of cells in each row.

1. When you are finished editing, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Save**, select a storage folder, enter a name for the set, and then click **Save**.

## Deleting a Spin Set {#deleting-a-spin-set}

When you delete a set, the set itself is moved to the Trash. However, the members (or “children”) within that set are not affected; instead, they each retain their existing published or unpublished state.

See also [Manually publishing assets](publishing-files.md#manually-publishing-assets) and [Manually unpublishing assets](publishing-files.md#manually-unpublishing-assets).

**To delete a Spin Set**

1. In the Grid View, List View, or Details View, select one or more Spin Sets.
1. On the Global Navigation Bar, click **File** > **Delete** > **Delete**.

