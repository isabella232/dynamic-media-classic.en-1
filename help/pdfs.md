---
title: Working with PDFs
seo-title: Working with PDFs
description: null
seo-description: Learn how to work with PDFs in Dynamic Media Classic.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a

---

# Working with PDFs{#working-with-pdfs}

PDF (Portable Document Format) files are most often used in Scene7 to create eCatalogs. When you upload a PDF file, Scene7 rasterizes, or rips, the pages by default so that the pages can be used to build rich media.

## PDF upload options {#pdf-upload-options}

When you upload a PDF file, you can format it in various ways. You crop its pages, extract search words, enter a pixels-per-inch resolution, and choose a color space. PDF files often contain a trim margin, crop marks, registration marks, and other printer’s marks. You can crop these marks from the sides of pages as you upload a PDF file.

Options for uploading PDF files are located on the Upload screen under PDF Options.

**Processing**

The Processing options are as follows:

**Rasterize** (Default) Rips the pages in the PDF file and converts vector graphics to bitmap images. Choose this option to create an eCatalog.

**Extract Search Words** Extracts words from the PDF file so that the file can be searched by keyword in an eCatalog Viewer.

**Extract Links** Extracts links from the PDF files and coverts them to Image Maps that are used in an eCatalog Viewer.

**Auto-Generate eCatalog With Multiple Page PDF** Automatically creates an eCatalog from the PDF file. The eCatalog is named after the PDF file you uploaded. (This option is only available if you rasterize the PDF file as you upload it.)

**Resolution**

Determines the resolution setting. This setting determines how many pixels are displayed per inch in the PDF file. The default is 150.

**Color Space**

Select the Color Space menu and choose a color space for the PDF file. Most PDF files have both RGB and CMYK color images. The RGB color space is preferable for online viewing.

**Detect Automatically** Retains the color space of the PDF file.

**Force As RGB** Converts to the RGB color space.

**Force As CMYK** Converts to the CMYK color space.

**Force As Grayscale** Converts to the Grayscale color space.

**Color Profile**

Choose a Color Profile option:

**Convert To sRGB** Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages.

**Keep Original Color Space** Retains the original color space.

**Custom From &gt; To** Opens menus so you can choose a Convert From and Convert To color space. You can choose a standard Photoshop color space or a color space you uploaded to SPS.

See [ICC profiles](icc-profiles.md#icc_profiles).

## Cropping white space from a PDF file {#cropping-white-space-from-a-pdf-file}

1. To automatically crop white-space pixels from a PDF file as you upload it, select the Crop menu and choose Trim. 
1. Specify the following options:

   **Trim Away&#xA;Based On** Choose whether to crop based on color or transparency:

   **Color** Choose the Color option. Then select the Corner menu and choose the corner of the PDF with the color that best represents the white-space color you want to crop.

   **Transparency** Choose the Transparency option.

   **Tolerance** Drag the slider to specify a tolerance from 0 through 1:

   **Trimming based on color** Specify 0 to crop pixels only if they exactly match the color you selected in the corner of the PDF. Numbers closer to 1 allow for more color difference.

   **Trimming based on transparency** Specify 0 to crop pixels only if they are totally transparent; numbers closer to 1 allow for more transparency.

## Cropping from the sides of PDF pages {#cropping-from-the-sides-of-pdf-pages}

You can manually remove printer’s marks from the sides of the pages in a PDF file as you upload it.

1. Select the Crop menu and choose Manual.
1. Enter pixel settings in the Top, Right, Bottom, and Left text boxes to crop from the top, bottom, and sides of pages.

How much of the page is cropped depends on the Resolution PX/Inch setting you enter for the PDF file. For example, if you enter 150 (the default) as the Resolution PX/Inch setting and you crop 75 pixels from the sides of pages, a half-inch is cropped because, at 150 pixels per inch, 75 pixels equals a half-inch.
