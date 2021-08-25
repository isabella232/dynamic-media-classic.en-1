---
title: Create zoom targets for Guided Zoom
description: Learn how to create zoom targets for Guided Zoom in Dynamic Media Classic.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
---
# Create zoom targets for Guided Zoom{#creating-zoom-targets-for-guided-zoom}

Zoom targets guide your viewers to certain parts of an image. Besides free-form zooming, viewers can select a zoom target thumbnail and zoom to the part of the image you want them to focus on. Zoom targets are an opportunity for you to highlight the attractive or interesting parts of an image.

![Create zoom targets for Guided Zoom](/help/assets/zo_guided_zoom.png)

## About zoom targets {#about-zoom-targets}

The maximum zoom percentage of zoom targets is 100 percent. The minimum zoom percentage varies based on a combination of the viewer size and the image size, as shown in this table:

| Image size | Viewer size | Zoom percentage |
| --- | --- | --- |
| Large | Smaller | Smaller minimum |
| Small | Larger | Larger minimum |

You can change the size of the Zoom Viewer to match the size being used on your web page. To permanently change this setting, you can change the viewer size on the Setup screen (if you are an administrator). See [Set up Zoom Viewer Presets](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Create and edit zoom targets {#creating-and-editing-zoom-targets}

Create and edit zoom targets on the Zoom Target Editor screen. To open this screen, select an image and do one of the following:

* select the rollover **[!UICONTROL Edit]** button and choose Zoom Targets.
* In the Browse Panel, display the image in **[!UICONTROL Detail View]**, then select **[!UICONTROL Zoom Targets]**.

On the Zoom Target Editor screen, select **[!UICONTROL Select Target]** button (arrow) to select a target before changing its size or position. To create a zoom target on the image, select **[!UICONTROL Add Targets]** (rectangle). The Zoom Target Editor page also offers tools for deleting, copying, and naming zoom targets.

### Create a zoom target {#creating-a-zoom-target}

To create a zoom target, open the Zoom Target Editor page and do the following:

1. Select **[!UICONTROL Add Targets]** (rectangle), move the pointer over the image, and select where you want to the zoom target to be.

   A thumbnail image of the zoom target appears in the panel on the right side of the screen.

1. Pick **[!UICONTROL Select Target]** (arrow), and then select the zoom target you created, and adjust the size and position of the target.

    * **Resize** - Move the pointer over a corner of the zoom target and drag to enlarge or shrink the target.

    * **Position** -  Move the pointer over the zoom target and drag it to a different location.

1. Enter a name for the zoom target in the Name box.

   >[!NOTE]
   >
   >What you enter in the Name box is more than a name. When users move the pointer over the zoom target, they see what you enter in the Name box. Enter a brief description of the zoom target in the Name box so users know what they can zoom on.

1. Optionally, enter user data in the User Data field. This field is for web site designers to add information to the zoom target.
1. Select **[!UICONTROL Save]**.

   The coordinates and zoom level of the zoom target are saved. A thumbnail of your zoom target with the name you entered appears on the right side of the screen.

>[!NOTE]
>
>To see what your zoom targets look like in a Zoom Viewer, select the **[!UICONTROL Preview]** button in the Zoom Target Editor screen and choose a Zoom Viewer in the Preview screen. For information about this screen, see [Preview images with different Zoom Viewers](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Edit zoom targets {#editing-zoom-targets}

To edit zoom targets, use the following techniques on the Zoom Target Editor page:

* **Reposition** - With the Select Target button (the arrow), select the target. Then drag the target to a different location.

* **Resize** - With the Select Target button (the arrow), select the target. To enlarge or shrink the target, move the pointer over a corner of the zoom target and drag.

* **Delete** - Select the target’s thumbnail image on the right side of the screen. Then select **[!UICONTROL Delete Target]**.

* **Renaming** - Select the target’s thumbnail image on the right side of the screen. Then enter a name in the **[!UICONTROL Name]** text field and select **[!UICONTROL Save]**.

### Copy zoom targets {#copying-zoom-targets}

You can copy zoom targets from one image to another. Copy targets when two images present similar content and their zoom targets belong in the same locations. To copy zoom targets to another image, do the following:

1. Open the image with zoom targets you want to copy in the Zoom Target Editor screen.
1. Select **[!UICONTROL Copy Targets To]**.
1. In the Select Images dialog box, select an image and pick **[!UICONTROL Select]**.
