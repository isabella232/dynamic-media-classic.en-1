---
title: Uploading template files
seo-title: Uploading template files
description: null
seo-description: Learn how to upload template files.
uuid: b3f8c80a-df43-48a4-a9c0-1cdf12cc90ea
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WSECB8A9BF-35BB-4dda-ACB1-926D03F1966E
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: bb826b03-31c9-4226-a16f-619ed6bf9552
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 44.907-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/template_basics;/content/help/en/experience-manager/morehelp/template_basics
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Uploading template files{#uploading-template-files}

Upload the files you need for your template into the Scene7 Publishing System before you begin building the template. You can build templates from an Adobe® Photoshop® PSD or an image file. TIFF and PNG images are recommended because they allow for transparency.

>[!NOTE]
>
>Scene7 recommends using transparent TIFF or PSD images in your templates at the exact size you want to display them on your web site. When you publish the template, call the image with an Image Preset that is also the same size. Paying attention to size ensures that your template is not resized (resampled) at a size larger or smaller than the size at which it was designed.

Templates can be created from Adobe Photoshop PSD files or image files.

For detailed instructions on uploading files, see [Uploading files](uploading-files.md#uploading_files). Keep the following in mind when uploading template files:

* If you’re uploading a PSD file, you can create a template from it. Scene7 creates a separate image for each layer in the PSD. In the Upload Job Options dialog box, select Photoshop Options, select the Maintain Layers option, and select the Create Template option. Then choose an option on the Layer Naming menu for naming the images that Scene7 creates from layers in the PSD. See [PSD upload options](psd-files.md#psd_upload_options).
* If uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. See [Image editing options at upload](image-editing-options-upload.md#image_editing_options_at_upload).

>[!MORE_LIKE_THIS]
>
>* [Uploading your files](uploading-files.md#uploading_your_files)
>* [Working with PSD files](psd-files.md#working_with_psd_files)
