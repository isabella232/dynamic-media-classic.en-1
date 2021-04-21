---
title: Creating a Swatch Set
description: Learn how to create a swatch set.
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Viewers
role: Business Practitioner
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
---
# Creating a Swatch Set{#creating-a-swatch-set}

A Swatch Set gives users the opportunity to view an item in a different color, pattern, or finish. To create a Swatch Set with color swatches, you need one image for each different color, pattern, or finish you want to present to users. You also need one color, pattern, or finish swatch for each color, pattern, or finish.

For example, suppose you want to present images of caps with different color bills; the bills are red, green, and blue. In this case, you need three shots of the same cap. You need one shot with a red, one with a green, and one with a blue bill. You also need a red, green, and blue color swatch. The color swatches serve as the thumbnails that users click in the Swatch Set Viewer to see the red-billed, green-billed, or blue-billed cap.

## Creating a Swatch Set {#create}

When you create a set, the **Publish after save** option affects the set and set members in the following ways:
|**[!UICONTROL Publish after save]** option selected before saving?|State of set after saving|State of set members after saving|
|--- |--- |--- |
|Yes|Published|Published|
|No|Unpublished|Set members retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To create a Swatch Set:**

1. Do one of the following:

   * **Select the images first** - In the Browse Panel, select the images, and then click **[!UICONTROL Build]** > **[!UICONTROL Swatch Sets]**.

   * **Start from the Swatch Set screen** - Click **[!UICONTROL Build]** > **[!UICONTROL Swatch Sets]**. Select a folder in the Asset Library and drag the images onto the Views section of the Swatch Set page.

1. Drag swatch colors, patterns, or finishes into the Swatches placeholder box on the Swatch Set page.

   Make sure that the color, pattern, or finish swatch you drag into each placeholder represents the color, pattern, or finish of the adjacent image.

1. To change the order of images in your Swatch Set, drag the images to new locations.
1. Near the lower-right corner of the page, ensure that **[!UICONTROL Publish after save]** is selected (default).
1. Click **[!UICONTROL Save]**, select a folder for storing your color swatch Swatch Set, enter a name for the set, and click **[!UICONTROL Submit]**.
1. To see your Swatch Set in the Swatch Set Viewer, click **[!UICONTROL Preview]** on the Swatch Set screen. You can click swatch thumbnails in the Swatch Set Viewer to see how they behave.

## Editing a Swatch Set {#editing-a-swatch-set}

Whether you edit a published or an unpublished set, the **[!UICONTROL Publish after save]** option affects the set and set members in the following ways:

|Set already published?|**[!UICONTROL Publish after]** save option selected before saving your edit?|State of set after saving|State of set members after saving|
|--- |--- |--- |--- |
|Yes|Yes|Published|Published|
|Yes|No|Published|Existing set members retain their published state. Any new set members that you added during your edit retain their published or unpublished state.|
|No|Yes|Published|Published|
|No|No|Unpublished|Existing set members and any new set members that you added during your edit retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To edit a Swatch Set:**

1. In the Grid view, browse to an SwatchSet, and then below the image, click **[!UICONTROL Edit]**.
1. Do any of the following:

    * To add an image (published or unpublished), drag it from a folder in Add Assets onto the Swatch Set’s **[!UICONTROL Views]** page.
    * To remove an image, select it, and then click **[!UICONTROL Delete]** on the toolbar.
    * To reorder images, drag an image to a new position.

1. When you are finished editing the set, near the lower-right corner of the page, ensure that **[!UICONTROL Publish after save]** is selected (default).
1. Click **[!UICONTROL Save]**, select a storage folder, enter a name for the set, and then click **[!UICONTROL Save]**.

## Deleting a Swatch Set {#deleting-a-swatch-set}

When you delete a set, the set itself is moved to the Trash. However, the members (or “children”) within that set are not affected; instead, they each retain their existing published or unpublished state.

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To delete a Swatch Set:**

1. In the Grid View, List View, or Details View, select one or more Swatch Sets.
1. On the Global Navigation Bar, click **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.
