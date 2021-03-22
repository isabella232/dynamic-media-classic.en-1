---
title: Uploading the PDF files
description: Learn how to upload the PDF files associated with an eCatalog.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: Business Practitioner
---

# Uploading the PDF files{#uploading-the-pdf-files}

Typically, Adobe PDF files are the source for an eCatalog. These files contain all image information, fonts, and vector graphics. You can build an eCatalog with images as well. After you have prepared your PDF files for uploading, select the Upload button on the Global Navigation bar to begin uploading the PDFs.

## Preparing your PDF files {#preparing-your-pdf-files}

Prepare your PDF files before uploading them to Dynamic Media Classic:

* To make uploading the files easier, place all the files in the same folder on your computer or network.
* Name the files in alphanumeric order by page. Ordering the pages will make it easier to place the pages in the proper order after the files are uploaded.
* To see whether PDF pages contain crop marks, registration targets, or color bars, examine the pages. These marks determine where to cut the paper when documents are printed; they must be removed before your eCatalog is placed on the web. Dynamic Media Classic provides options for cropping marks when you upload PDF files.
* If you want viewers to search your eCatalog by keyword, find out whether your PDF files are “flattened.” You cannot extract search words from flattened PDF files. To find out whether a PDF is flattened, try to select text inside it. If you can’t select text, the PDF is flattened and viewers cannot search by keyword in your eCatalog. 
* Because they are meant to be printed, PDF files usually contain CMYK images. By default, Dynamic Media Classic can intelligently detect these CMYK images and convert them using an internal CMYK color profile. However, if you want to use a custom color profile to convert CMYK images, you can do so.

  See [ICC profiles](icc-profiles.md#icc_profiles).

## Best practice PDF upload options {#best-practice-pdf-upload-options}

For detailed information about the different upload methods, see [Uploading your files](uploading-files.md#uploading_your_files).

Select the files you want to upload, and then select these *best practice* PDF Options:

* **Crop**
Select the Crop menu and choose Manual if the pages contain crop marks, registration marks, or other marks. Enter the number of pixels to crop from the top, right, bottom, and left sides of pages. Crop marks are often set to a half-inch margin. Assume that you choose 150 (recommended) as the pixel-per-inch resolution, and enter 75, 75, 75, 75 in the Top, Right, Bottom, and Left text boxes. In such case, it crops a half inch from the margins (at 150 ppi, half of 1 equals 75 pixels).

* **Processing**
Select the Processing menu and choose Rasterize. The PDF file must be rasterized so that all pages and images can be displayed in the eCatalog.

* **Extract Search Words (optional)**
Select this option if you want your viewers to be able to search by keyword in your eCatalog.

* **Auto-Generate eCatalog from multiple page PDF (optional)**
Select this option to automatically create an eCatalog when you upload. You can go straight to the eCatalog screen and begin working on your eCatalog without having to first select PDF files and select the Build command. The eCatalog is named after your PDF file.

* **Resolution**
Dynamic Media Classic recommends 150 pixels per inch.

* **Colorspace**
Dynamic Media Classic recommends choosing Detect Automatically. Usually, PDFs created for print output are in CMYK; PDFs for online viewing are RGB. If a PDF uses both color spaces, you can select a specific color space by choosing Force As RGB or Force As CMYK. PDFs use both color spaces, for example, when page graphics use a CMYK color space but pictures use RGB. If you uploaded an ICC profile, its name appears on the Colorspace menu and you can choose it there.

    See [ICC profiles](icc-profiles.md#icc_profiles).

* **Color Profile**
Choose a Color Profile option:

* **Convert&#xA;To SRGB**
Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages.

* **Keep Original Color Space**
Retains the original color space.

* **Custom From > To**
Opens menus so you can choose a Convert From and Convert To color space. You can choose a standard Photoshop color space or a color space you uploaded to Dynamic Media Classic.

See [ICC profiles](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>For details on all PDF options, see [PDF upload options](pdfs.md#pdf_upload_options).

