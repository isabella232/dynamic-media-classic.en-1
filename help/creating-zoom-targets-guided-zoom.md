---
title: Creating zoom targets for Guided Zoom
seo-title: Creating zoom targets for Guided Zoom
description: null
seo-description: Learn how to create zoom targets for Guided Zoom.
uuid: 652ac83f-2e26-4a01-b8c7-00864a1a1cac
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WSEEDDE48F-2809-4d31-B0BF-EEC4FC5152B8,scene7/using/WS07B67BF5-BC73-44b0-8C59-C42D850B25B3,scene7/using/WS124B037D-814F-4c3e-8958-44720C7C5CEE,scene7/using/WSef8d5860223939e2-2278be4412b1d305dbc-8000,scene7/using/WSef8d5860223939e258a5b1f312b1d3cdca6-8000,scene7/using/WSef8d5860223939e21763e15112b1d48b4a3-8000
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 2f47a19e-7e0d-4d77-b9d8-53c9ef7ef1f0
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 43.021-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/zoom;/content/help/en/experience-manager/morehelp/zoom
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Creating zoom targets for Guided Zoom{#creating-zoom-targets-for-guided-zoom}

Zoom targets guide your viewers to certain parts of an image. As well as free-form zooming, viewers can click a zoom target thumbnail and zoom to the part of the image you want them to focus on. Zoom targets are an opportunity for you to highlight the attractive or interesting parts of an image.

![]()

## About zoom targets {#about-zoom-targets}

The maximum zoom percentage of zoom targets is 100 percent. The minimum zoom percentage varies based on a combination of the viewer size and the image size, as shown in this table:

<table cellpadding="4" cellspacing="0">
 <thead align="left">
  <tr>
   <th class="cellrowborder" id="d19e14999" valign="top" width="NaN%"><p>Image size</p></th> 
   <th class="cellrowborder" id="d19e15002" valign="top" width="NaN%"><p>Viewer size</p></th> 
   <th class="cellrowborder" id="d19e15005" valign="top" width="NaN%"><p>Zoom percentage</p></th> 
  </tr> 
 </thead> 
 <tbody>
  <tr>
   <td class="cellrowborder" headers="d19e14999 " valign="top" width="NaN%"><p>Large</p></td> 
   <td class="cellrowborder" headers="d19e15002 " valign="top" width="NaN%"><p>Smaller</p></td> 
   <td class="cellrowborder" headers="d19e15005 " valign="top" width="NaN%"><p>Smaller minimum</p></td> 
  </tr> 
  <tr>
   <td class="cellrowborder" headers="d19e14999 " valign="top" width="NaN%"><p>Small</p></td> 
   <td class="cellrowborder" headers="d19e15002 " valign="top" width="NaN%"><p>Larger</p></td> 
   <td class="cellrowborder" headers="d19e15005 " valign="top" width="NaN%"><p>Larger minimum</p></td> 
  </tr> 
 </tbody> 
</table>

You can change the size of the Zoom Viewer to match the size being used on your web page. To permanently change this setting, you can change the viewer size on the Setup screen (if you are an administrator). See [Setting up Zoom Viewer Presets](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Creating and editing zoom targets {#creating-and-editing-zoom-targets}

Create and edit zoom targets on the Zoom Target Editor screen. To open this screen, select an image and do one of the following:

* Click the rollover **Edit** button and choose Zoom Targets.
* In the Browse Panel, display the image in Detail view and click **Zoom Targets**.

On the Zoom Target Editor screen, click **Select Targe**t button (the arrow) to select a target before changing its size or position. Click **Add Targets** (the rectangle) to create a zoom target on the image. The Zoom Target Editor screen also offers tools for deleting, copying, and naming zoom targets.

### Creating a zoom target {#creating-a-zoom-target}

Open the Zoom Target Editor screen and follow these steps to create a zoom target:

1. Click **Add Targets** (the rectangle), move the pointer over the image, and click where you want to the zoom target to be.

   A thumbnail image of the zoom target appears in the panel on the right side of the screen.

1. Click **Select Target** (the arrow), click to select the zoom target you created, and adjust the size and position of the target.

   **Resizing** Move the pointer over a corner of the zoom target and drag to enlarge or shrink the target.

   **Positioning** Move the pointer over the zoom target and drag it to a different location.

1. Enter a name for the zoom target in the Name box.

   >[!NOTE]
   >
   >What you enter in the Name box is more than a name. When users move the pointer over the zoom target, they see what you enter in the Name box. Enter a brief description of the zoom target in the Name box so users know what they can zoom on.

1. Optionally, enter user data in the User Data field. This field is for web site designers to add information to the zoom target.
1. Click **Save**.

   The coordinates and zoom level of the zoom target are saved. A thumbnail of your zoom target with the name you entered appears on the right side of the screen.

>[!NOTE]
>
>To see what your zoom targets look like in a Zoom Viewer, click the Preview button in the Zoom Target Editor screen and choose a Zoom Viewer in the Preview screen. For information about this screen, see [Previewing images with different Zoom Viewers](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Editing zoom targets {#editing-zoom-targets}

Use these techniques on the Zoom Target Editor screen to edit zoom targets:

**Repositioning** With the Select Target button (the arrow), click the target to select it. Then drag the target to a different location.

**Resizing** With the Select Target button (the arrow), click the target to select it. Then move the pointer over a corner of the zoom target and drag to enlarge or shrink the target.

**Deleting** Click the target’s thumbnail image on the right side of the screen. Then click Delete Target.

**Renaming** Click the target’s thumbnail image on the right side of the screen. Then enter a name in the Name box and click Save.

### Copying zoom targets {#copying-zoom-targets}

You can copy zoom targets from one image to another. Copy targets when two images present similar content and their zoom targets belong in the same locations. Follow these steps to copy zoom targets to another image:

1. Open the image with zoom targets you want to copy in the Zoom Target Editor screen. 
1. Click **Copy Targets To**.
1. In the Select Images dialog box, select an image and click **Select**.

