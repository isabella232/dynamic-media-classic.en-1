---
title: Exporting assets from Scene7 Publishing System
seo-title: Exporting assets from Scene7 Publishing System
description: null
seo-description: Learn how to export assets from Scene7 Publishing System.
uuid: fc0aa9d3-58bc-4988-b20f-884ec5b6ff1d
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WS259993e42159a215-1c6a66df1265272619e-7fe8
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 7da2941b-4a2c-4f93-bf1b-0cec2d172909
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 43.294-0400
lr-lastmodifiedby: admin
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Exporting assets from Scene7 Publishing System{#exporting-assets-from-scene-publishing-system}

You can save assets you edited in Scene7 Publishing System to a local network drive. Exported assets are bundled in a ZIP file for downloading or sending by e-mail.

The compressed Zip file has a maximum file size of 1 GB for the export job. Also, be aware that you are allowed a maximum of 500 total assets per export job.

Scene7 keeps a record of export jobs in the Jobs screen.

**To export assets from Scene7 Publishing System**

1. Select the assets you want to export, and then click **File** &gt; **Export**. 
1. In the Export Selected Assets window, click **Image Options**, and then specify any of the following options (administrators determine which options are available to their users):

   **Presets** Optionally, choose an Image Preset to format the asset when you export it. If you choose an Image Preset, the other formatting options are not available, as the asset adopts the formats defined by the Image Preset.

   **Conversion** Convert the asset file or the original image.

   **Size** You can select a standard size. Or, you can click Other from the Size drop-down list, choose the desired unit of measure, and then specify the width and height.

   See also [Specifying export options available to Media Portal users](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   **Format** Choose an image format.

   **Color** Choose RGB, CMYK, or Gray.

   **Resolution** Choose 72, 150, or 300 ppi.

   **Job Name** You can assign a job name to the export.

   **Send Email To** Optionally, enter an e-mail address to send the assets by e-mail. The e-mail message lists the URL where the recipient can go to download the assets.

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

