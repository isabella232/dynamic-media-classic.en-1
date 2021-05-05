---
title: Uploading template files
description: Learn how to upload template files.
uuid: e19979b5-3f41-49c5-99aa-107ede3be98c
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 75658717-5c39-473e-9d32-718d00706310
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
---
# Uploading template files{#uploading-template-files}

Upload the files you need for your template into Dynamic Media Classic before you begin building the template. You can build templates from an Adobe® Photoshop® PSD or an image file. TIFF and PNG images are recommended because they allow for transparency.

>[!NOTE]
>
>Dynamic Media Classic recommends using transparent TIFF or PSD images in your templates at the exact size you want to display them on your web site. When you publish the template, call the image with an Image Preset that is also the same size. Paying attention to size ensures that your template is not resized (resampled) at a size larger or smaller than the size at which it was designed.

Templates can be created from Adobe Photoshop PSD files or image files.

For detailed instructions on uploading files, see [Uploading files](uploading-files.md#uploading_files). Keep the following in mind when uploading template files:

* If you are uploading a PSD file, you can create a template from it. Dynamic Media Classic creates a separate image for each layer in the PSD. In the Upload Job Options dialog box, click **[!UICONTROL Photoshop Options]**, and select **[!UICONTROL Maintain Layers]** and **[!UICONTROL Create Template]**. Then choose an option from the **[!UICONTROL Layer Naming]** drop-down list for naming the images that Dynamic Media Classic creates from layers in the PSD. 
See [PSD upload options](psd-files.md#psd_upload_options).
<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [Uploading your files](uploading-files.md#uploading_your_files)
>* [Working with PSD files](psd-files.md#working_with_psd_files)
