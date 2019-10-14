---
title: Creating a PDF document
seo-title: Creating a PDF document
description: null
seo-description: Learn how to create a PDF document using the Web-to-Print process in Dynamic Media Classic.
uuid: 274fb06b-320b-40fa-8b61-c224d8aceaa1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 87e91e8e-10a2-4fba-87c7-aad2bd798146

---

# Creating a PDF document {#creating-a-pdf-document}

The final step in the Web-to-Print process is generating the customized PDF. After end-users personalize the template using the web application you created, they create a final PDF document. This final PDF is generally sent to a print service provider for professional-grade printing. To make sure that the final PDF prints as expected, developers use the correct joboptions file and set up fonts, printer marks, and colors correctly.

## Setting up PDF Presets {#setting-up-pdf-presets}

Specify the PDF compatibility level and printer settings by creating and uploading a PDF joboptions file to the Dynamic Media Classic Server. For example, you can choose to select PDF/X-4 compliant PDF output (recommended for PDF print publishing workflows). You can create the joboptions file in your authoring software (such as Adobe Illustrator), or in Acrobat. Always check with your printer, who can advise you on the appropriate job option settings for your print job.

For more information on creating joboptions files, and for information on creating a joboptions file in Acrobat, see Adobe Acrobat Help.

To create a joboptions file in Illustrator:

1. Choose Edit &gt; Adobe PDF Presets.
1. In the dialog box, select the preset you want to use.

   The following Job Option Settings are supported by Dynamic Media Classic:

    |Job Option|Description|
    |--- |--- |
    |General|<ul><li>Compatibility </li><li>Object Level Compression</li><li>Embed thumbnails</li><li>Optimize for fast web view</li></ul>|
    |Images|<ul><li>Downsample</li><li>Resolution</li><li>Threshold</li><li>Compression for color, gray, and mono</li></ul>|
    |Fonts|<ul><li>Embed all fonts (fonts are embedded by default)</li><li>Embed OpenType fonts</li><li>Subset embedded fonts when percent of characters used is less than:</li><li>Always Embed List</li><li>Never Embed List</li></ul>|
    |Color|<ul><li>Color Strategy (Tag only images is treated as tag everything)</li><li>Document Rendering Intent</li><li>Only the following working spaces are supported for 4.2.5. 4.3 will allow you to use any customer provide profile that has been uploaded to IPS.</li><li>As a workaround you can specify the destination color space for the artwork to be converted to using the default color profiles for the company.</li></ul>|
    |RGB|<ul><li>e-sRGB </li><li>scRGB with encoding range [-4.0, 4.0]</li><li>Lab D50</li><li>PCS XYZ</li><li>Flat XYZ</li><li>Linear ROMM-RGB</li><li>ROMM-RGB</li><li>sYCC 8-bit</li><li>e-sYCC 8-bit</li></ul>| 
    |Gray|<ul><li>Gray Gamma 1.8</li><li>Gray Gamma 2.2</li><li>Dot Gain 10%</li><li>Dot Gain 15%</li><li>Dot Gain 20%</li><li>Dot Gain 25%</li><li>Dot Gain 30%</li><li>sGray</li></ul>|
    |Preserve CMYK values for calibrated CMYK color spaces||
    |Advanced|Preserve OPI comments is always turned on|
    |Standards|Compliance Standard|

   >[!NOTE]
   >
   >Dynamic Media Classic ignores printer mark settings in the joboptions file. Rather, printer marks are configured through the use of Dynamic Media Classic URL commands.

1. Click Export, then specify a name and location and click Save.
1. Upload the job options file as an asset to the Scene7 Publishing System.

   Use it with your published template by referring to it in the URL. For example:

   `https://yourpublishserver.scene7.com/is/agm/SiliconPublishing/PetNews?&fmt=pdf,cmyk&joboption=SPSfilenameid`

## Preparing the PDF for print {#preparing-the-pdf-for-print}

Before finalizing the PDF for print, make sure you follow the guidelines in this section.

**Images**

Make sure that all images in your publish job have been uploaded to your Dynamic Media Classic Server and published.

**Fonts**

Make sure that all fonts in your publish job have been uploaded to your Dynamic Media Classic Server and published. Be certain that you have legal rights to host the fonts if you plan to allow end-users to change them.

**Image resolution (pixels per inch)**

The resolution of bitmap images is preserved by the Dynamic Media Classic server in generated print-ready PDFs. Dynamic Media Classic upscales image resolution if necessary. For optimal results, leave the resolution at the default value (typically 72 dpi) when previewing on web. The default resolution for all the images in your company is set in the Publish Settings/Image Server window in the Default Print Resolution section. Higher resolutions (such as 300dpi) can result in longer processing time and should only be applied to a print-ready PDF. Use the imageRes= command in the URL to manually override the default resolution for PDF jobs.

**Color Management**

Your document and images can use grayscale, CMYK, named spot colors, RGB, or Lab color models. Each can be either uncalibrated or calibrated by employing an ICC color profile. For best results, embed the profile in the generated print-ready PDF. The Dynamic Media Classic Server does this by default. Make sure that all required color profiles have been uploaded to the Dynamic Media Classic platform. Preferably, make sure that the color management options set in your design application, match those set in your Dynamic Media Classic Server:

* **Design application color management settings:** In the Color Settings of your authoring application (such as Adobe Illustrator), specify the RGB and CMYK color profiles in the Working Spaces section.

* **Dynamic Media Classic color management settings:** Typically, the color management settings in the design application should match the default color profiles in your Dynamic Media Classic server. You can find these settings in the Publish Setup/Image Server window.

## Displaying printer marks {#displaying-printer-marks}

You might create a PDF for either of these cases:

* A finished document
* An intermediate document, such as a film or plate, which may be sent to a printer for production

An intermediate document might contain additional production content, such as bleed margins, printer marks, and so on. This content is usually shown outside the boundaries of the finished page.

All marks available from the "Add Printer Marks" screen in Acrobat are supported. The printer marks are controlled with the `printerMark` parameter. The syntax is `&printerMark=trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed`.

* trim marks = 0|1
* bleed marks = 0|1
* registration marks = 0|1
* color bars = 0|1
* page information = 0|1
* style = Illustrator | IllustratorJ | QuarkXPress
* line weight = 0.125 | 0.25 | 0.50
* layer embed = 0|1

When preparing a document for print production, printer marks may be needed to help the print service align separation films for producing proofs, measure film for correct calibration and ink density, trim film to size, and so on. Printer marks indicate the boundaries of document boxes such as trim boxes and bleed boxes. Production-related content may include:

* **Media box**
The boundaries of the physical medium on which the page will be printed. Content outside the media box can safely be discarded without affecting the meaning of the file.

* **Bleed box**
The region to which the contents of the page are clipped when output in a production environment. The bleed box may include areas needed to accommodate the physical limitations of cutting, folding, and trimming equipment. The default value is the page's crop box.

* **Trim box**
The intended dimensions of the finished page after trimming. The trim box may be smaller than the media box to allow for production-related content, such as printing instructions, cut marks, and color bars. The default value is the page's crop box.

* **Art box**
The extent of the page's meaningful content (including potential white space) as intended by the page's creator. The default value is the page's crop box.

You can use the modifiers shown in this table to replicate the printer marks available in Adobe Illustrator, InDesign, and Acrobat:

|Modifier/Values|Description|
|--- |--- |
|bleedMargin=top,left,bottom,right|Specified in Acrobat with the Set Page Boxes option. Select BleedBox, then specify the margins with the Margin Controls option.<br><br>Values represent the distance of the top, left, bottom, and right edges from the original edges of the artwork (the media box) going inwards. Values (0-1000) are in points.<br><br>New height=original height - (top+bottom)<br><br>New width= original width - (left+right)|
|mediaMargin=top,left,bottom,right|Specified in Acrobat with the Set Page Boxes option. Modify Custom Page Size under the Change Page Size option.<br><br>Values represent the distance of the top, left, bottom, and right edges from the original edges of the artwork (the media box) going outwards. Values (0-1000) are in points.<br><br>New height=top+bottom+original height<br><br>New width=top+bottom+original width<br><br>The new height and new width values determine the new page size of the generated PDF.<br><br>Once a new Media Box is defined, all calculations of trim margin and bleed margin need to consider the new Media Box as the edge of the artwork.|
|trimMargin=top,left,bottom,right|Specified in Acrobat with the Set Page Boxes option. Select Trim Box, then specify the margins with the Margin Controls option.<br><br>Values represent the distance of the top, left, bottom, and right edges from the original edges of the artwork (the media box) going inwards. Values (0-1000) are in points.<br><br>New height=original height - (top+bottom)<br><br>New width=original width - (left+right)|
|printerMark= trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed|Values are as follows:<br><br>trim marks = 0,1 (default is 0)<br><br>bleed marks = 0,1 (default is 0)<br><br>registration marks = 0,1 (default is 0)<br><br>color bars = 0,1 (default is 0)<br><br>page information = 0,1 (default is 0)<br><br>style = Default, InDesignJ1, InDesignJ2, Illustrator, illustratorJ, QuarkXPress (default is Default)<br><br>line weight= 0.125-0.2, both values inclusive (default is 0.25)<br><br>layer embed = 0, 1, with 1 creating a new layer containing all printer marks (default is 1)<br><br>Depending on what style is used, the marks and color bars appear different and match with the corresponding styles used by Acrobat.|

Note the following about printer marks:

* Specify bleed margins, trim margins, and media margins through URL calls when specifying printer marks. Specifying printer marks without specifying these margins causes these marks to appear outside the visible region of the generated PDF. Also, the trim marks and bleed marks overlap.
* Specifying the same margin values for the trim margin and bleed margin results in trim marks and bleed marks overlapping when both these flags are set to 1 in `&printerMark`.
* Specifying fmt=swf/image formats through URL calls results in output without any printer marks or margins because this feature is specific to PDF output.
* Specifying `&printerMark=`through the URL results in default values being used for all parameters. Specifying `&printerMark=1` results in trim marks being set to 1 and default values for other parameters. But to set the nth element to ON, all the (n-1) parameters need to be specified through URL.
* Specifying only one value for `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in that value being applied to all the top, bottom, left, and right margins of the original artwork.
* Specifying only the top and left values through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the top value being assigned to the bottom value and the left value being equal to the right.
* Not specifying the right value through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the left value being assigned to the right.
* For a multi-page PDF, printer marks/margins are applied to all the pages (in Acrobat, users can select page ranges for printer marks/margins).
* The output of a PDF with printer marks/margins enabled matches exactly with Acrobat X unless otherwise specified.

If you want to create a PDF/X-4 compliant PDF file through the &joboption modifier in the URL, you should be aware of the limitations related to printer marks specified in the PDF ISO_15930-7-2008.pdf:

* Each Page object of a PDF file includes a MediaBox. Each Page object in a PDF/X-4 conforming file shall include a TrimBox or an ArtBox, but not both. The MediaBox may be included by inheritance.
* If the BleedBox is present, the ArtBox or the TrimBox shall not extend beyond the boundaries of the BleedBox. If the CropBox is present, none of the ArtBox, the TrimBox, or the BleedBox shall extend beyond the boundaries of the CropBox.
* None of the ArtBox, the TrimBox, the CropBox, or the BleedBox shall extend beyond the boundaries of the MediaBox.
* Some industry practices require the use of the BleedBox. Appropriate trade practices should be followed.
* The use of the TrimBox is recommended over the use of the ArtBox.
* All annotations other than TrapNet and PrinterMark annotations shall have a value for Rect lying completely outside the BleedBox (or the TrimBox or the ArtBox if no BleedBox is present). All PrinterMark annotations shall have a value for Rect lying completely outside the TrimBox or ArtBox. A PDF/X-4 conforming reader may completely ignore annotations except for PDF TrapNet annotations.
* A Rect shall be regarded as completely outside a bounding box if all of the coordinates of the Rect lie either outside the bounding box or on its edge, and the intersection of the two rectangles is zero.
* If the ViewerPreferences dictionary contains the ViewArea, ViewClip, PrintArea or PrintClip keys, each of these keys present shall have the value MediaBox or (if a BleedBox is present in all page objects of the file) BleedBox.

