---
title: Exporting assets from Dynamic Media Classic
description: Learn how to export assets from Dynamic Media Classic.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
---

# Exporting assets from Dynamic Media Classic{#exporting-assets-from-dmc}

You can save assets you edited in Dynamic Media Classic to a local network drive. Exported assets are bundled in a ZIP file for downloading or sending by e-mail.

The compressed Zip file has a maximum file size of 1 GB for the export job. Also, be aware that you are allowed a maximum of 500 total assets per export job.

Dynamic Media Classic keeps a record of export jobs in the Jobs screen.

**To export assets from Dynamic Media Classic**

1. Select the assets you want to export, and then click **File** > **Export**. 
1. In the Export Selected Assets window, click **Image Options**, and then specify any of the following options (administrators determine which options are available to their users):

   * **Presets**
   Optionally, choose an Image Preset to format the asset when you export it. If you choose an Image Preset, the other formatting options are not available, as the asset adopts the formats defined by the Image Preset.

   * **Conversion**
   Convert the asset file or the original image.

   * **Size**
   You can select a standard size. Or, you can click Other from the Size drop-down list, choose the desired unit of measure, and then specify the width and height.

        See also [Specifying export options available to Media Portal users](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **Format**
   Choose an image format.

   * **Color**
   Choose RGB, CMYK, or Gray.

   * **Resolution**
   Choose 72, 150, or 300 ppi.

   * **Job Name**
   You can assign a job name to the export.

   * **Send Email To**
   Optionally, enter an e-mail address to send the assets by e-mail. The e-mail message lists the URL where the recipient can go to download the assets.

1. Click **Export**.

Three basic export actions are supported:

* Original File (export the original file for the asset)
* Convert Using Preset (use an image preset to format the asset)
* Convert Without Preset (use the export dialog to specify image modifiers)

The following asset types cannot be exported. All others should generate an export.

* Image Sets
* Render Sets
* Spin Sets
* Media Sets
* Multi-bitrate Sets
* eCatalogs

In addition, templates cannot be exported as an “original file.”

You can use conversion to export the following asset types:

* Images
* Templates
* Adjusted Images
* PDF (will generate converted pages)
* Postscript

The following behavior results when a large selection of various asset types are fed into the exporter:

* All asset types which cannot be exported are removed from the list before job submittal 
* If a conversion is requested, all types which can be converted are, and all others are exported as original

