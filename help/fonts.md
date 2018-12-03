---
title: Fonts
seo-title: Fonts
description: null
seo-description: Learn how to use fonts in Dynamic Media Classic.
uuid: 15c8c79e-2797-44d9-b10a-6bdfa4417b8f
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WS0F37AB0B-B54A-411d-A92B-074265EEA926,scene7/using/WS4A5DEBF5-715D-4e02-A840-9742246D163B,scene7/using/WS3DC225D9-51FF-49a6-BA76-2A334FCE0189
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: f60f0c1d-1823-4f2b-a7f3-4a5531768e62
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 43.320-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/support_files;/content/help/en/experience-manager/morehelp/support_files
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Fonts{#fonts}

In some cases, the Scene7 Publishing System requires you to upload a font file to enter or render text in a particular font. For example, to use a particular font for text on a template layer, upload the font file. To display eCatalog Viewer page numbers in a particular font, upload the font file.

Scene7 supports these font types:

* All TrueType fonts
* PostScript® fonts
* OpenType/TrueType fonts
* OpenType/PostScript fonts
* PhotoFonts

After a font file has been uploaded, you can change its SPS ID, font name, and type information on the Edit Info screen.

>[!NOTE]
>
>Scene7 recommends uploading all font styles (bold, italic, bold/italic, and regular) if you plan to use fonts in template layers. Scene7 needs these font styles to process requests. Uploading all PostScript/Adobe Type 1 files associated with a font is also recommended because some of these fonts contain detailed kerning information.

## Uploading font files {#uploading-font-files}

Upload font files with the same techniques you use to upload other files. You can store font files in any SPS folder. See [Uploading your files](uploading-files.md#uploading_your_files).

## Editing font file information {#editing-font-file-information}

You can change the ID name of a font as well as its type information. Editing a font file can be helpful in searches and making fonts easier to identify.

In the Browse Panel, select the font file you want to edit in Detail view and choose File &gt; Edit Info. The Edit Info screen opens. Choose the following options and select the Submit button.

**Font Name** This name identifies the font when it is published.

**PostScript Name** This name is the full PostScript name for the font. It usually indicates the weight or style.

**RTF Name** This name appears on a pop-up menu in the RTF editor where template text layers are created.

**Font Family Name** This name lists the font name without the style, weight, or font-type indicator.

**Font Style** The options are Plain, Bold, Italic, and Bold-Italic.

**Font Type** The options are TrueType and Adobe Type 1. If you call these fonts by another name, you can enter it.

**Font Type Abbreviation** The options are as follows:

**TTF** TrueType font files used for PDF/PostScript rendering and image serving.

**AFM** Adobe PostScript font files that contain Adobe Font Metrics information and are used for image serving.

**PFM** Adobe PostScript font files that contain binary font metric information.

**PFB** Adobe PostScript font files that contain binary font outline information and are used for PDF/PostScript rendering and image serving.
