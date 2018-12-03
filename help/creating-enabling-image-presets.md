---
title: Creating and enabling Image Presets
seo-title: Creating and enabling Image Presets
description: null
seo-description: Learn how to create and enable image presets.
uuid: 54fcef6c-6013-42f3-a252-69dcb4fcdaf1
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WSef8d5860223939e2-573b004c12b186ea56e-8000
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8d4bcb27-48ee-4e89-b213-cac1792b4094
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 42.604-0400
lr-lastmodifiedby: admin
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Creating and enabling Image Presets{#creating-and-enabling-image-presets}

When users export image assets using Media Portal, they can choose an Image Preset in the Export Selected Assets dialog box. An Image Preset is a collection of pre-defined settings that change the size, image quality, format, resolution, and other aspects of an image’s appearance when it is exported.

Media Portal administrators can create Image Presets to control how images are reformatted when they are exported. Image Presets reformat images to the specifications of your company when users export images from the Scene7 Publishing System. Rather than reformatting images on their own, users export them to the precise specifications of an Image Preset.

The following restrictions apply when you export image assets:

* The width x height must be less than or equal to 100 MB per image. For example, the image cannot exceed 10K x 10K, or any aspect variation below, such as 8K x 12K.
* There is a maximum of 1 GB total file size per export job.
* You can have a maximum of 500 total assets per export job.

>[!NOTE]
>
>These restrictions apply only to the exporting of derived image assets, not the exporting of master files.

To create Image Presets, see [Image Presets](application-setup.md#image_presets).

To enable users to choose Image Presets when they export files, see [Specifying export options available to Media Portal users](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

To choose which Image Presets are available to the members of a group, see [Choose Image Preset access permissions for a group](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).
