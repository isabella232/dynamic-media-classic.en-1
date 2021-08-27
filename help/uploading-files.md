---
title: Upload files
description: Learn how to upload files in Adobe Dynamic Media Classic.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
---
# Upload files{#uploading-files}

Before you upload assets files to Adobe Dynamic Media Classic, make sure that the asset files are named correctly, and that your folder structure is set up and organized the way you want. You can upload files from an Adobe Dynamic Media Classic-provided FTP site or directly from your computer or network. Adobe Dynamic Media Classic offers options for optimizing files as you upload them. If you installed Adobe Dynamic Media Classic desktop application, you can upload files and folders by dragging them directly from your desktop. See [Application General Settings](application-setup.md#general_settings).

## Prepare your assets and folders for uploading {#preparing-your-assets-and-folders-for-uploading}

Before uploading assets to Adobe Dynamic Media Classic, make sure that they are in the right format and size. You also have to observe the Adobe Dynamic Media Classic rules for naming assets. By setting up a folder organization and structure for the files, you make sure you can locate and work with files easily.

### Supported asset file formats {#supported-asset-file-formats}

This table lists the asset file formats that Adobe Dynamic Media Classic supports. For information on supported Camera Raw files, see [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html).

| Asset file formats | Description |
| --- | --- |
| Audio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Cascading Style Sheet | CSS |
| Color profiles |ICC, ICM |
| Fonts | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Images | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (Windows® only), TIF, TIFF |
| InDesign | INDD, INDT |
| MS® Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG, and Camera Raw |
| PostScript | EPS, PS |
| Adobe Dynamic Media Classic Image Authoring | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Video | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR and ZIP upload support includes a check box to select if you want to unpack the files.

### Unsupported image formats in Dynamic Media {#unsupported-image-formats-dynamic-media}

The following list describes the subtypes of raster image file formats that are *not* supported in Dynamic Media.

See also [Detect unsupported file formats for Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* PNG files that have an IDAT chunk size greater than 100 MB.
* PSB files.
* PSD files with a color space other than CMYK, RGB, Grayscale, or Bitmap are not supported. DuoTone, Lab, and Indexed color spaces are not supported.
* PSD files that have a bit depth greater than 16.
* TIFF files that have floating point data.
* TIFF files that have Lab color space.

### Asset types {#asset-types}

To achieve optimal results with the Adobe Dynamic Media Classic program, be sure to use the recommended file formats and sizes. This table lists asset types, some with recommended formats and file sizes for commonly used assets.

| Asset type | Description/Recommendations |
| --- | --- |
| Audio | Input audio asset formats include AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. You can transcode audio to the following formats: MP3, AAC, and HE-AAC. |
| Images (for Image Sizing, Zoom, Image Sets, Spin Sets) | Images have to be at least 2000 pixels at the longest size; typical image sizes range from 1500 to 2500 pixels in the longest size. Lossless image formats, including TIFF and PNG files, are recommended. If you use a JPEG image, use the highest-quality settings. Animate GIF files are handled like other static content. |
| eCatalogs | Use high-resolution PDF files created in Adobe® Acrobat® or a Creative Suite application saved as “press-ready.” PDFs include all needed fonts, images, masks, and referenced graphical elements, either as single-pages, double-page spreads, or in a multi-page format. Order your pages by naming the files in alphanumeric order. Place all PDFs for your eCatalog in a single folder for ease of uploading. You can select cropping options on upload to remove the trim area from PDFs, including crop marks, registration targets, or color bars. Most press-ready PDF files are in the CMYK color space, so it is important to obtain the CMYK ICC color profile used with your PDF files. |
| Templates | Layered image or layout design that can include text, images, and layers. Image layers, text strings, and attributes, such as color and size, can be parameterized so that variable data can be customized. Image requirements for use in templates are the same as other images. Prepare your graphics in Photoshop or another image-editing program. Save each graphic as a flattened transparent file in TIFF or PNG format. Ensure that the image resolution is appropriate for expected use. Images for print are 300 ppi.|
| Videos | Adobe Dynamic Media Classic supports video files saved in the OGV and MP4 format. You can transcode files to MP4 format at upload. See [Supported asset file formats](#supported-static-file-formats). |
| Fonts | Uploaded TrueType, Type1 (Windows® Only), OpenType® fonts, and PhotoFonts. |
| Images | Images and layered image files. |
| Image Sets and Swatch Sets | A set of related images that can be displayed in a viewer. |
| ICC profiles | A color profile you can use to convert an uploaded image from its source color space into a different color space.|
| Vignettes | Images authored with the Image Authoring program, and related files. |
| Content files | Adobe InDesign, Illustrator, or Photoshop content files. |
| FXG files | Resolution-independent graphic format files that you can use to create customizable templates for output to print, web, email, desktop, and devices. |
| SVG files | Scalable vector graphic files that Image Serving servers can render. |
| XML files | Files that define pre-processing rules that are used to modify the path and query portions of requests. |
| Cascading Style Sheet files.| Upload CSS skins for customization of HTML5 viewers. |
| JavaScript files | JavaScript files are used for viewer instrumentation to hold account information. Adobe Security recommends this asset type only for client accounts that have a separate domain in use for delivery (to avoid cross site scripting). |

>[!NOTE]
>
>When you upload image files and PDFs to Adobe Dynamic Media Classic, the system converts these source files to P-TIFF (Pyramid TIFF) files. These P-TIFFs are the files that are later published to Dynamic Media Image Servers. Adobe Dynamic Media Classic uses the Pyramid Tiff file format because it contains various zoom ratios that allow for fast zooming when viewed with an Adobe Dynamic Media Classic Zoom Viewer.

### Supported Static File Formats {#supported-static-file-formats}

Adobe Dynamic Media Classic supports several static file formats. Static content is any asset that is published "as-is," such as CSS, PDF, SVG, and XML.

The following file types can be published:

* Animated GIF
* Audio files
* CSS
* JavaScript (when the company is configured with its own domain)
* Master video
* PDF (when PDF is marked for publish after upload, to avoid delivery of all PDFs for existing eCatalog/PDF workflow)
* PrX video
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic does not provide the option to generate a preview URL of static content.

### Filename requirements {#filename-requirements}

Because filename extensions are stripped from filenames during the upload process, the system does not allow files to have the same root name. In the Adobe Dynamic Media Classic system, the asset filename minus the filename extension becomes the asset ID for the asset. For this reason, no two assets can have the same name.

Make sure that all users in your company understand these file naming rules:

* Asset IDs with the same exact name are not allowed in the system. 
* Asset ID names are case-sensitive. 
* As a best practice, make sure that asset IDs do not contain blank spaces (for example, black jacket.tif and blue jacket.jpg). Adobe Dynamic Media Classic ASCII-encodes blank spaces in asset names when it uses asset names to construct URL strings. These ASCII codes are hard to read, which can make reading URLs more difficult.
* Language-specific characters are permitted in filenames. However, the following characters are not permitted in filenames:

  \ ; / ? : @ & = + $ , &#42; " &lt; > | ' { } %

  If a filename contains one or more of the above characters, the characters are removed from the filename on upload.

Usually, an asset filename can be the same as its item number, product SKU, or other name as in the following:

|Item|Filename|Asset ID|
|--- |--- |--- |
|896649|896649.jpg|896649|
|48A3_2X|48A3_2X.tif|48A3_2X|

### Folder organization and structure {#folder-organization-and-structure}

Organize and structure folders and subfolders for your content in Adobe Dynamic Media Classic before you upload your content to the system. Planning ahead this way has two major advantages:

* When you upload your content to Adobe Dynamic Media Classic via FTP, you can tell the system to replicate your folder structure during the upload. This way, your content is organized in the same folders and subfolders in Adobe Dynamic Media Classic as it is on your computer or network. (To replicate your folder structure in Adobe Dynamic Media Classic, select the Include Subfolders option when you upload assets via FTP.)
* Reorganizing folders inside the system after files are uploaded is much more difficult than starting with a carefully considered folder structure.

The folder-naming approach and structure you choose for storing your content on the Adobe Dynamic Media Classic depends on the needs of your organization. Here are some sample folder structures:

**SKU-based** - Folders are named according to SKUs or item numbers. For example, separate folders are created for all 0-, 20-, 30- number series.

**Brand-based** - For manufacturers with multiple brand lines and retailers who market other brands from other companies, separate files into product folders named for different brands.

**Project-based** - Folders are organized according to rollout/drop date or project name. Clients who primarily produce eCatalogs favor this approach.

**Mirror of web site folder hierarchy** - This folder structure mirrors the folder structure of the website, with the folders named, for example, for product categories.

## About uploading files {#uploading-your-files}

You can upload individual files from the desktop or upload folders via FTP. If you want to upload more than 100 MB of files or upload entire folders and subfolders, select the **VIA FTP** tab.

Adobe Dynamic Media Classic sends you an email message to confirm when your upload job begins and ends, and to notify you of any problems.

During (or immediately after) a large upload job, some new items could display the “Image not yet optimized” message. This message appears because the files are not yet fully processed and added to Adobe Dynamic Media Classic. You can optimize these files later. See [Optimize Files](application-setup.md#optimize_files).

### Upload files using the From Desktop tab {#upload-files-using-sps-desktop-application}

The Adobe Dynamic Media Classic Desktop application lets you upload files and folders by dragging.

1. In the Adobe Dynamic Media Classic Desktop application, on the Global Navigation bar, select **[!UICONTROL Upload]**.
1. On the Upload page, select the **[!UICONTROL From Desktop]** tab.
1. On the left side of the Upload page, in the **[!UICONTROL Select Files for Upload]** area, select **[!UICONTROL Browse]** to select the files or folders you want to upload, then select **[!UICONTROL Open]**.
1. On the right side of the Upload page, in the **Choose Folder Destination** area, navigate to a destination folder where you want the uploaded files or folders added.
1. (Optional) Near the bottom of the Upload page, in the Job Name text field, enter the new name of the upload job. Or, you can simply use the default, system-generated name that Adobe Dynamic Media Classic provides. The job and other upload and publishing jobs are recorded on the Jobs page, where you can check the status of jobs. See [Checking job files](checking-job-files.md#checking_job_files).
1. (Optional) Near the bottom of the Upload page, select **[!UICONTROL Publish After Uploading]** if you want to automatically publish the assets that you upload.
When you publish files, files are sent to live servers. URLs for these files can then be used on external websites and applications. This same option is also available in the Job Options dialog box.
1. (Optional) Near the bottom of the Upload page, select **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** if you want the files you upload to replace existing files with the same names. This same option is also available in the Job Options dialog box.
The name of this option could be different, depending on the settings in **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.
1. Near the lower-right corner of the Upload page, select **[!UICONTROL Job Options]**, then specify the options you want.

   See [Upload options](uploading-files.md#upload_options).

1. In the Upload Job Options dialog box, select **[!UICONTROL Save]**.
1. In the lower-right corner of the Upload page, select **[!UICONTROL Submit Upload]**.
   To see the progress of the upload, select **[!UICONTROL Jobs]** on the Global Navigation Bar. You can continue working in Adobe Dynamic Media Classic and return to the Jobs page at any time to review an in-progress job. To cancel an upload job in progress, select **[!UICONTROL Cancel]** next to the Duration time.

### Upload files using the VIA FTP tab {#upload-files-using-via-ftp}

1. Log in to the Adobe Dynamic Media Classic FTP site that is specific to your particular region. Use the FTP user name and password that you received from your administrator.
1. In Adobe Dynamic Media Classic, on the Global Navigation bar, select **[!UICONTROL Upload]**.
1. On the Upload page, select the **[!UICONTROL VIA FTP]** tab.
1. On the left side of the Upload page, in the **[!UICONTROL Choose FTP Folder For Upload]** area, choose an FTP folder from which to upload files. 
1. On the right side of the Upload page, in the **[!UICONTROL Choose Adobe Dynamic Media Folder Destination]** area, choose a destination folder in Adobe Dynamic Media Classic.
1. (Optional) Near the bottom of the Upload page, in the Job Name text field, enter the new name of the upload job. Or, you can simply use the default, system-generated name that Adobe Dynamic Media Classic provides. The job and other upload and publishing jobs are recorded on the Jobs page, where you can check the status of jobs.
See [Checking job files](checking-job-files.md#checking_job_files).
1. (Optional) Near the bottom of the Upload page, select **[!UICONTROL Publish After Upload]** if you want to automatically publish the assets that you upload.
When you publish files, files are sent to live servers. URLs for these files can then be used on external websites and applications. This same option is also available in the Job Options dialog box.
1. (Optional) Near the bottom of the Upload page, select **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** if you want the files you upload to replace existing files with the same names. This same option is also available in the Job Options dialog box.
The name of this option could be different, depending on the settings in **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.
1. Optional; available only if you clicked the **[!UICONTROL VIA FTP]** tab. Near the bottom of the Upload page, select **[!UICONTROL Uncompress Zip or Tar Files on Upload]** if you want to automatically extract all files from your uploaded ZIP or TAR file. This same option is also available in the Job Options dialog box. 
1. Near the lower-right corner of the Upload page, select **[!UICONTROL Job Options]**, then specify the options you want.

   See [Upload options](uploading-files.md#upload_options).

1. In the Upload Job Options dialog box, select **[!UICONTROL Save]**. 
1. In the lower-right corner of the Upload page, select **[!UICONTROL Submit Upload]**.

   To see the progress of the upload, on the Global Navigation Bar, select **[!UICONTROL Jobs]**. The Jobs page shows you the progress of the upload. You can continue working in Adobe Dynamic Media Classic and return to the Jobs page at any time to review an in-progress job.

To cancel an upload job in progress, select **[!UICONTROL Cancel]** next to the Duration time.

## Upload Job Options dialog box {#upload-options}

When uploading files, you can choose from the following options in the Upload Job Options dialog box:

* **JOB** - Select **[!UICONTROL JOB]** to choose options that affect the entire upload job.

    You can also choose *default* options for uploading jobs by using the **[!UICONTROL Default Upload Options]** dialog box in General Settings. Go to **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Default Upload Options]**, then set the default options you want.

  * **[!UICONTROL When]** - This option is available only if you selected the **[!UICONTROL VIA FTP]** tab.
    * **[!UICONTROL One-Time]** - Specify an upload job that runs once. Options include the following:
      * **[!UICONTROL Now]** - Runs the upload job immediately after you select **[!UICONTROL Save]** in the Upload Job Options dialog box, then select **[!UICONTROL Submit Upload]** on the Upload page.
      * **[!UICONTROL Schedule For Later]** - Select the year, month, day, and time (in 15-minute increments) that you want the upload job to run.
    * **[!UICONTROL Recurring]** - Specify an upload job that runs daily, weekly, or monthly. Or, customize the upload job to your own specifications.
      * **[!UICONTROL Daily]** - Set the time you want the job to run every day. If you want the job to run only Monday to Friday, select **[!UICONTROL Weekdays Only]**.
      * **[!UICONTROL Weekly]** - Choose a specific day of the week and time that you want the job to run.
      * **[!UICONTROL Monthly]** - Choose a specific day of the month or day of the week, including the start time, that you want the job to run.
      * **[!UICONTROL Custom]** - Customize an upload  or publish job time interval to your own specifications. See [Create a custom upload or publish job time interval](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).

  * **[!UICONTROL Publish After Uploading]** - Available if you selected either the **[!UICONTROL FROM DESKTOP]** tab or the **[!UICONTROL VIA FTP]** tab. Select this option to automatically publish the assets that you upload. When you publish files, files are sent to live servers. URLs for these files can then be used on external websites and applications. This option is also available on the Upload page.

  * **[!UICONTROL Overwrite in any folder, same base asset name regardless of extension]** - Available if you selected either the **[!UICONTROL FROM DESKTOP]** tab or the **[!UICONTROL VIA FTP]** tab. Select this option if you want the files you upload to replace existing files with the same names. This option is also available on the Upload page. The name of this option could be different, depending on the settings in **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]** > **[!UICONTROL Upload to Application]** > **[!UICONTROL Overwrite Images]**.

  * **[!UICONTROL Uncompress Zip or Tar Files on Upload]** - Available if you selected either the **[!UICONTROL FROM DESKTOP]** tab or the **[!UICONTROL VIA FTP]** tab.
Select this option if you want to automatically extract all files from your uploaded ZIP or TAR file. This same option is also available in the Job Options dialog box. 

  * **[!UICONTROL Include subfolders]** - Available only if you selected the **[!UICONTROL VIA FTP]** tab.
Select this option if you want to upload subfolders of the folder you intend to upload. The names of the folder and its subfolders you upload are entered automatically in Adobe Dynamic Media Classic.

  * **[!UICONTROL Process metadata files]** - Available only if you selected either the **[!UICONTROL VIA FTP]** tab. Select this option if you want to upload a tab-delimited or XML file to add metadata to multiple assets.
See [Import metadata (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).

* **CROP OPTIONS** - To automatically crop white-space pixels from an image, open the **[!UICONTROL Crop]** menu, select **[!UICONTROL Manual]**, and enter pixel measurements in the Top, Right, Bottom, and Left text fields to crop from the sides. You can also select **[!UICONTROL Trim]** on the Crop menu and choose these options:

  * **[!UICONTROL Trim Away Based On]** - Choose whether to crop based on color or transparency:
    * **[!UICONTROL Color]** - Choose the Color option. Then select the Corner menu and choose the corner of the image with the color that best represents the white-space color you want to crop.
      Trimming based on color: Specify 0 to crop pixels only if they exactly match the color you selected in the corner of the image. Numbers closer to 1 allow for more color difference.
    * **[!UICONTROL Transparency]** -  Choose the **[!UICONTROL Transparency]** option.
      Trimming based on transparency: Specify 0 to crop pixels only if they are transparent; numbers closer to 1 allow for more transparency.
    * **[!UICONTROL Tolerance]** - Drag the slider to specify a tolerance from 0 through 1.

* **COLOR PROFILE OPTIONS** - Choose a color conversion when you create optimized files that are used for Adobe Dynamic Media Classic dynamic delivery:

  * **[!UICONTROL Default Color Preservation]** - Maintains the source image colors whenever the images contain color space information; there is no color conversion. Nearly all images today have the appropriate color profile already embedded. However, if a CMYK source image does not contain an embedded color profile, the colors are converted to sRGB (standard Red Green Blue) color space. sRGB is the recommended color space for displaying images on web pages.
  * **[!UICONTROL Keep Original Color Space]** - Retains the original colors without any color conversion at the point of ingestion into Adobe Dynamic Media Classic. For images without an embedded color profile, any required color conversion to process requests for the image is done using the default color profiles as configured in the Publish settings. These color profiles do not always align with the color in the files created with this option. Therefore, you are encouraged to use the option Default Color Preservation.
  * **[!UICONTROL Custom From]** > **[!UICONTROL To]** - Opens menus so you can choose a **[!UICONTROL Convert From]** and **[!UICONTROL Convert To]** color space. This advanced option overrides any color information that is embedded in the source file. Select this option only when all the images that you are submitting contain incorrect or missing color profile data.

* **Image Edit Options** - You can preserve the clipping <> masks in images, and choose a color profile.
See [Image fine-tuning options at upload](image-editing-options-upload.md#image-editing-options-at-upload).

* **PostScript® Options** - You can rasterize PostScript® files, crop files, maintain transparent backgrounds, choose a resolution, and choose a color space.
See [Work with PostScript and Illustrator files](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Photoshop Options** - You can create templates from Adobe® Photoshop® files, maintain layers, specify how layers are named, extract text, and specify how images are anchored into templates.
See [PSD upload options](psd-files.md#psd_upload_options).

* **PDF Options** - You can rasterize the files, extract search words and links, auto-generate an eCatalog, set the resolution, and choose a color space.
See [PDF upload options](pdfs.md#pdf_upload_options).

* **Illustrator Options** - You can rasterize Adobe Illustrator® files, maintain transparent backgrounds, choose a resolution, and choose a color space.
See [Work with PostScript and Illustrator files](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **EVIDEO Options** - You can transcode a video file by choosing a Video Preset.
See [Work with video encoding presets](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **Additional Metadata** - Enter keywords that describe the files you intend to upload. Separate keywords by comma. Keywords make searching for assets easier.
See [Conduct an advanced search](searching-assets.md#conducting_an_advanced_search).

* **Batch Set Presets** - If you want to create an Image Set, Spin Set, or Swatch Set from the uploaded files, select the **[!UICONTROL Active]** column for the preset you want to use. You can select more than one preset. You create the presets in the Application Setup/Batch Set Presets page.
See [Batch Set Presets](application-setup.md#batch_set_presets).

* **Advanced** - See [Follow an upload with another job](uploading-files.md#follow-an-upload-with-another-job).

## Follow an upload with another job {#follow-an-upload-with-another-job}

When you upload items using FTP, you can schedule a subsequent job to begin when the upload is complete. If other jobs are scheduled to begin, the job you schedule here is queued after them.

The new job sends a notification to the address you specify so that the code at that location can be triggered. This follow-on publishing job uses the same name as the upload job, but with the text *Pub_* added to the beginning.

**To follow an upload with another job:**

1. Select **[!UICONTROL Upload]**, then select the **[!UICONTROL VIA FTP]** tab.
1. In the lower-right corner of the Upload page, select **[!UICONTROL Job Options]**.
1. In the Upload Job Options dialog box, expand the **[!UICONTROL ADVANCED]** section.
1. Choose one of the following from the **[!UICONTROL Follow Upload with another job]** drop-down list:

    * None
    * HTTP Request
    * Image Serving Publish
    * Image Rendering Publish
    * Video Publish

1. Specify the HTTP address.
1. Specify if you want to run only if files were uploaded.
1. Indicate whether you want to run this request every time this job completes, or only when files were published.

   >[!NOTE]
   >
   >Regularly scheduled jobs can sometimes result in no files being published.

>[!MORELIKETHIS]
>
>* [Work with asset folders](asset-folders.md#working_with_asset_folders)
>* [Handle recurring upload and publish jobs](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Use an upload or publish job as a trigger](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
