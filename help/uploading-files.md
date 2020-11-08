---
title: Uploading files
seo-title: Uploading files
description: null
seo-description: Learn how to upload files.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a

---

# Uploading files{#uploading-files}

Before you upload assets files to Dynamic Media Classic, make sure that the asset files are named correctly, and that your folder structure is set up and organized the way you want. You can upload files from a Dynamic Media Classic-provided FTP site or directly from your computer or network. Dynamic Media Classic offers options for optimizing files as you upload them. If you installed Adobe Dynamic Media Classic desktop application, you can upload files and folders by dragging them directly from your desktop. (See [Application General Settings](application-setup.md#general_settings).)

## Preparing your assets and folders for uploading {#preparing-your-assets-and-folders-for-uploading}

Before uploading assets to Dynamic Media Classic, make sure that they are in the right format and size. You also have to observe the Dynamic Media Classic rules for naming assets. By setting up a folder organization and structure for the files, you make sure you can locate and work with files easily.

### Supported asset file formats {#supported-asset-file-formats}

This table lists the asset file formats that Dynamic Media Classic supports. For information on supported Camera Raw files, see [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

|Asset file formats|Description|
|--- |--- |
|Audio|AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3|
|Cascading Style Sheet|CSS|
|Color profiles|ICC, ICM|
|Fonts|AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF|
|FXG|FXG|
|Illustrator|AI, FXG|
|Images|BMP, FPX, GIF, JPEG, JPG, PNG, PICT (Windows only), TIF, TIFF|
|InDesign|INDD, INDT|
|MS Office|DOC, PPT, RTF, XLS|
|PDF|PDF|
|Photoshop|PSD, FXG, and Camera Raw|
|PostScript|EPS, PS|
|Dynamic Media Classic Image Authoring|VNC, VNT, VNW|
|SVG|SVG, SVGX|
|TAR|TAR|
|Video|3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF|
|XML|XML|
|ZIP|ZIP|

TAR and ZIP upload support includes a check box to select if you want to unpack the files.

### Unsupported image formats in Dynamic Media {#unsupported-image-formats-dynamic-media}

The following list describes the sub-types of raster image file formats that are *not* supported in Dynamic Media.

See also [Detect unsupported file formats for Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* PNG files that have an IDAT chunk size greater than 100 MB.
* PSB files.
* PSD files with a color space other than CMYK, RGB, Grayscale, or Bitmap are not supported. DuoTone, Lab, and Indexed color spaces are not supported.
* PSD files that have a bit depth greater than 16.
* TIFF files that have floating point data.
* TIFF files that have Lab color space.

### Asset types {#asset-types}

To achieve optimal results with the Dynamic Media Classic platform, be sure to use the recommended file formats and sizes. This table lists asset types, some with recommended formats and file sizes for commonly used assets.

|Asset type|Description/Recommendations|
|--- |--- |
|Audio|Input audio asset formats include AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. You can transcode audio to the following formats: MP3, AAC, and HE-AAC.|
|Images (for Image Sizing, Zoom, Image Sets, Spin Sets)|Images have to be at least 2000 pixels at the longest dimension; typical image sizes range from 1500 to 2500 pixels in the longest dimension. Lossless image formats, including TIFF and PNG files, are recommended. If you use a JPEG image, use the highest-quality settings. Animate GIF files are handled like other static content.|
|eCatalogs|Use high-resolution PDF files created in Adobe® Acrobat® or a Creative Suite application saved as “press-ready.” PDFs include all needed fonts, images, masks, and referenced graphical elements, either as single-pages, double-page spreads, or in a multi-page format. Order your pages by naming the files in alphanumeric order. Place all PDFs for your eCatalog in a single folder for ease of uploading. You can select cropping options on upload to remove the trim area from PDFs, including crop marks, registration targets, or color bars. Most press-ready PDF files are in the CMYK color space, so it is important to obtain the CMYK ICC color profile used with your PDF files.|
|Templates|Layered image or layout design that can include text, images, and layers. Image layers, text strings, and attributes, such as color and size, can be parameterized so that variable data can be customized. Image requirements for use in templates are the same as other images. Prepare your graphics in Photoshop or another image-editing program. Save each graphic as a flattened transparent file in TIFF or PNG format. Ensure that the image resolution is appropriate for expected use. Images for print should be 300 ppi.|
|Videos|Dynamic Media Classic supports video files saved in the OGV and MP4 format. You can transcode files to MP4 format at upload.See [Supported asset file formats](#supported-static-file-formats).|
|Fonts|Uploaded TrueType, Type1 (Windows Only), OpenType fonts, and PhotoFonts|
|Images|Images and layered image files.|
|Image Sets and Swatch Sets|A set of related images that can be displayed in a viewer.|
|ICC profiles|A color profile you can use to convert an uploaded image from its source color space into a different color space.|
|Vignettes|Images authored with the Image Authoring program, as well as related files.|
|Content files|Adobe InDesign, Illustrator, or Photoshop content files.|
|FXG files|Resolution-independent graphic format files that you can use to create customizable templates for output to print, web, email, desktop, and devices.|
|SVG files|Scalable vector graphic files that Image Serving servers can render.|
|XML files|Files that define pre-processing rules that are used to modify the path and query portions of requests.|
|Cascading Style Sheet files.|Upload CSS skins for customization of HTML5 viewers.|
|JavaScript files|Javascript files are used for viewer instrumentation to hold account information. Adobe Security recommends this only for client accounts that have a separate domain in use for delivery (to avoid cross site scripting).|

>[!NOTE]
>
>When you upload image files and PDFs to Dynamic Media Classic, the system converts these source files to P-TIFF (Pyramid TIFF) files. These P-TIFFs are the files that are later published to Dynamic Media Image Servers. Dynamic Media Classic uses the Pyramid Tiff file format because it contains various zoom ratios that allow for fast zooming when viewed with a Dynamic Media Classic Zoom Viewer.

### Supported Static File Formats {#supported-static-file-formats}

Dynamic Media Classic supports several static file formats. Static content is any asset that is published "as-is," such as CSS, PDF, SVG, XML, and so on.

The following file types can be published:

* Animated GIF
* Audio files
* CSS
* JavaScript (when the company is configured with its own domain)
* Master video
* PDF (when PDF is specifically marked for publish after upload, to avoid delivery of all PDFs for existing eCatalog/PDF workflow)
* PrX video
* SVG
* XML
* ZIP

Dynamic Media Classic does not provide the option to generate a preview URL of static content.

### Filename requirements {#filename-requirements}

Because filename extensions are stripped from filenames during the upload process, the system does not allow files to have the same root name. In the Dynamic Media Classic system, the asset filename minus the filename extension becomes the asset ID for the asset. For this reason, no two assets can have the same name.

Make sure that all users in your company understand these file naming rules:

* Asset IDs with the same exact name are not allowed in the system. 
* Asset ID names are case sensitive. 
* As a best practice, make sure that asset IDs do not contain blank spaces (for example, black jacket.tif and blue jacket.jpg). Dynamic Media Classic ASCII-encodes blank spaces in asset names when it uses asset names to construct URL strings. These ASCII codes are hard to read, which can make reading URLs more difficult.
* Language-specific characters are permitted in filenames. However, the following characters are not permitted in filenames:

  \ ; / ? : @ & = + $ , &#42; " &lt; > | ' { } %

  If a filename contains one or more of the above characters, the characters are removed from the filename on upload.

In most cases, an asset filename can be the same as its item number, product SKU, or other name as in the following:

|Item|Filename|Asset ID|
|--- |--- |--- |
|896649|896649.jpg|896649|
|48A3_2X|48A3_2X.tif|48A3_2X|

### Folder organization and structure {#folder-organization-and-structure}

Organize and structure folders and subfolders for your content in Dynamic Media Classic before you upload your content to the system. Planning ahead this way has two major advantages:

* When you upload your content to Dynamic Media Classic via FTP, you can tell the system to replicate your folder structure during the upload. This way, your content is organized in the same folders and subfolders in Dynamic Media Classic as it is on your computer or network. (To replicate your folder structure in Dynamic Media Classic, select the Include Subfolders option when you upload assets via FTP.)
* Reorganizing folders inside the system after files are uploaded is much more difficult than starting with a carefully considered folder structure.

The folder-naming approach and structure you choose for storing your content on the Dynamic Media Classic depends on the needs of your organization. Here are some sample folder structures:

**SKU-based** Folders are named according to SKUs or item numbers. For example, separate folders are created for all 0-, 20-, 30- number series.

**Brand-based** For manufacturers with multiple brand lines and retailers who market other brands from other companies, separate files into product folders named for different brands.

**Project-based** Folders are organized according to rollout/drop date or project name. Clients who primarily produce eCatalogs favor this approach.

**Mirror of web site folder hierarchy** This folder structure mirrors the folder structure of the website, with the folders named, for example, for product categories.

## About uploading files {#uploading-your-files}

You can upload individual files from the desktop or upload folders via FTP. If you want to upload more than 100 MB of files or upload entire folders and subfolders, select the **VIA FTP** tab.

Dynamic Media Classic sends you an email message to confirm when your upload job begins and ends, and to notify you of any problems.

During (or immediately after) a large upload job, some new items may display the “Image not yet optimized” message. This message appears because the files are not yet fully processed and added to Dynamic Media Classic. You can optimize these files later. (See [Optimize Files](application-setup.md#optimize_files).)

### Uploading files using the FROM DESKTOP tab {#upload-files-using-sps-desktop-application}

The Dynamic Media Classic Desktop application lets you upload files and folders by dragging.

1. In the Dynamic Media Classic Desktop application, on the Global Navigation bar, click **Upload**.
1. On the Upload page, click the **FROM DESKTOP** tab.
1. On the left side of the Upload page, in the **Select Files for Upload** area, click **Browse** to select the files or folders you want to upload, then click **Open**.
1. On the right side of the Upload page, in the **Choose Folder Destination** area, navigate to a destination folder where you want the uploaded files or folders added.
1. (Optional) Near the bottom of the Upload page, in the **Job Name** field, specify the new name of the upload job. Or, you can simply use the default, system-generated name that Dynamic Media Classic provides. The job and other upload and publishing jobs are recorded on the Jobs page, where you can check the status of jobs.
See [Checking job files](checking-job-files.md#checking_job_files).
1. (Optional) Near the bottom of the Upload page, select **Publish After Uploading** if you want to automatically publish the assets that you upload.
When you publish files, files are sent to live servers. URLs for these files can then be used on external websites and applications. Note that this same option is also available in the Job Options dialog box.
1. (Optional) Near the bottom of the Upload page, select **Overwrite in any folder, same base asset name regardless of extension** if you want the files you upload to replace existing files with the same names. Note that this same option is also available in the Job Options dialog box.
The name of this option could be different, depending on the settings in **Application Setup > General Settings > Upload to Application > Overwrite Images**.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   See [Upload options](uploading-files.md#upload_options).

1. In the Upload Job Options dialog box, click **Save**.
1. In the lower-right corner of the Upload page, click **Submit Upload**.
   To see the progress of the upload, click **Jobs** on the Global Navigation Bar. You can continue working in Dynamic Media Classic and return to the Jobs page at any time to review an in-progress job. To cancel an upload job in progress, select **Cancel** next to the Duration time.

### Uploading files using the VIA FTP tab {#upload-files-using-via-ftp}

1. Log in to the Dynamic Media Classic FTP site that is specific to your particular region. Use the FTP user name and password that you received from your administrator.
1. In Dynamic Media Classic, on the Global Navigation bar, click **Upload**.
1. On the Upload page, click the **VIA FTP** tab.
1. On the left side of the Upload page, in the **Choose FTP Folder For Upload** area, choose an FTP folder from which to upload files. 
1. On the right side of the Upload page, in the **Choose Adobe Dynamic Media Folder Destination** area, choose a destination folder in Dynamic Media Classic.
1. (Optional) Near the bottom of the Upload page, in the **Job Name** field, specify the new name of the upload job. Or, you can simply use the default, system-generated name that Dynamic Media Classic provides. The job and other upload and publishing jobs are recorded on the Jobs page, where you can check the status of jobs.
See [Checking job files](checking-job-files.md#checking_job_files).
1. (Optional) Near the bottom of the Upload page, select **Publish After Upload** if you want to automatically publish the assets that you upload.
When you publish files, files are sent to live servers. URLs for these files can then be used on external websites and applications. Note that this same option is also available in the Job Options dialog box.
1. (Optional) Near the bottom of the Upload page, select **Overwrite in any folder, same base asset name regardless of extension** if you want the files you upload to replace existing files with the same names. Note that this same option is also available in the Job Options dialog box.
The name of this option could be different, depending on the settings in **Application Setup > General Settings > Upload to Application > Overwrite Images**.
1. (Optional; available only if you clicked the **VIA FTP** tab) Near the bottom of the Upload page, select **Uncompress Zip or Tar Files on Upload** if you want to automatically extract all files from your uploaded ZIP or TAR file. Note that this same option is also available in the Job Options dialog box. 
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   See [Upload options](uploading-files.md#upload_options).

1. In the Upload Job Options dialog box, click **Save**. 
1. In the lower-right corner of the Upload page, click **Submit Upload**.

   To see the progress of the upload, on the Global Navigation Bar, click **Jobs**. The Jobs page shows you the progress of the upload. You can continue working in Dynamic Media Classic and return to the Jobs page at any time to review an in-progress job.

To cancel an upload job in progress, click **Cancel** next to the Duration time.

## Upload Job Options dialog box {#upload-options}

When uploading files, you can choose from the following options in the Upload Job Options dialog box:

* **JOB** &mdash; Click **JOB** to choose options that affect the entire upload job.

    Note that you can also choose *default* options for uploading jobs by using the **Default Upload Options** dialog box in General Settings. Click **Setup > Application Setup > General Settings > Default Upload Options**, then set the default options you want.

    * **When** &mdash; The **When** option is available only if you selected the **VIA FTP** tab.
        * **One-Time** &mdash; Specify an upload job that runs once. Options include the following:
            * **Now** &mdash; Runs the upload job immediately after you click **Save** in the Upload Job Options dialog box, then click **Submit Upload** on the Upload page.
            * **Schedule For Later** &mdash; Select the year, month, day, and time (in 15 minute increments) that you want the upload job to run.
        * **Recurring** &mdash; Specify an upload job that runs daily, weekly, or monthly. Or, customize the upload job to your own specifications.
            * **Daily** &mdash; Set the time you want the job to run every day. If you want the job to run only Monday to Friday, select **Weekdays Only**.
            * **Weekly** &mdash; Choose a specific day of the week and time that you want the job to run.
            * **Monthly** &mdash; Choose a specific day of the month or day of the week, including the start time, that you want the job to run.
            * **Custom** &mdash; Customize an upload  or publish job time interval to your own specifications. See [Creating a custom upload or publish job time interval](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).

    * **Publish After Uploading** &mdash; Available if you selected either the **FROM DESKTOP** tab or the **VIA FTP** tab. Select this option to automatically publish the assets that you upload. When you publish files, files are sent to live servers. URLs for these files can then be used on external websites and applications. This option is also available on the Upload page.

    * **Overwrite in any folder, same base asset name regardless of extension** &mdash; Available if you selected either the **FROM DESKTOP** tab or the **VIA FTP** tab. Select this option if you want the files you upload to replace existing files with the same names. This option is also available on the Upload page. The name of this option could be different, depending on the settings in **Application Setup > General Settings > Upload to Application > Overwrite Images**.

    * **Uncompress Zip or Tar Files on Upload** &mdash; Available if you selected either the **FROM DESKTOP** tab or the **VIA FTP** tab.
Select this option if you want to automatically extract all files from your uploaded ZIP or TAR file. Note that this same option is also available in the Job Options dialog box. 

    * **Include subfolders** &mdash; Available only if you selected the **VIA FTP** tab.
Select this option if you want to upload subfolders of the folder you intend to upload. The names of the folder and its subfolders you upload are entered automatically in Dynamic Media Classic.

    * **Process metadata files** &mdash; Available only if you selected either the **VIA FTP** tab. Select this option if you want to upload a tab-delimited or XML file to add metadata to multiple assets.
See [Import metadata (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).

* **CROP OPTIONS** &mdash; To automatically crop white-space pixels from an image, open the Crop menu, choose Manual, and enter pixel measurements in the Top, Right, Bottom, and Left fields to crop from the sides. You can also choose Trim on the Crop menu and choose these options:

    * **Trim Away Based On** &mdash; Choose whether to crop based on color or transparency:

        * **Color** &mdash; Choose the Color option. Then select the Corner menu and choose the corner of the image with the color that best represents the white-space color you want to crop.

            Trimming based on color: Specify 0 to crop pixels only if they exactly match the color you selected in the corner of the image. Numbers closer to 1 allow for more color difference.

        * **Transparency** &mdash;  Choose the Transparency option.

            Trimming based on transparency: Specify 0 to crop pixels only if they are totally transparent; numbers closer to 1 allow for more transparency.

        * **Tolerance** &mdash; Drag the slider to specify a tolerance from 0 through 1.

* **COLOR PROFILE OPTIONS** &mdash; Choose a color conversion when you create optimized files that are used for Dynamic Media Classic dynamic delivery:

    * **Default Color Preservation** &mdash; Maintains the source image colors whenever the images contain color space information; there is no color conversion. Nearly all images today have the appropriate color profile already embedded. However, if a CMYK source image does not contain an embedded color profile, the colors are converted to sRGB (standard Red Green Blue) color space. sRGB is the recommended color space for displaying images on web pages.

    * **Keep Original Color Space** &mdash; Retains the original colors without any color conversion at the point of ingestion into Dynamic Media Classic. For images without an embedded color profile, any required color conversion to process requests for the image are done using the default color profiles as configured in the Publish settings. These color profiles may not align with the color in the files created with this option. Therefore, you are encouraged to use the option Default Color Preservation.

    * **Custom From > To** &mdash; Opens menus so you can choose a Convert From and Convert To color space. This advanced option overrides any color information that is embedded in the source file. You should select this option only when all the images that you are submitting contain incorrect or missing color profile data.

* **IMAGE EDITING OPTIONS** &mdash; You can preserve the clipping <> masks in images, and choose a color profile.
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload).

* **POSTSCRIPT OPTIONS** &mdash; You can rasterize PostScript® files, crop files, maintain transparent backgrounds, choose a resolution, and choose a color space.
See [Working with PostScript and Illustrator files](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **PHOTOSHOP OPTIONS** &mdash; You can create templates from Adobe® Photoshop® files, maintain layers, specify how layers are named, extract text, and specify how images are anchored into templates.
See [PSD upload options](psd-files.md#psd_upload_options).

* **PDF OPTIONS** &mdash; You can rasterize the files, extract search words and links, auto-generate an eCatalog, set the resolution, and choose a color space.
See [PDF upload options](pdfs.md#pdf_upload_options).

* **ILLUSTRATOR OPTIONS** &mdash; You can rasterize Adobe Illustrator® files, maintain transparent backgrounds, choose a resolution, and choose a color space.
See [Working with PostScript and Illustrator files](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **EVIDEO OPTIONS** &mdash; You can transcode a video file by choosing a Video Preset.
See [Working with video encoding presets](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **ADDITIONAL METADATA** &mdash; Enter keywords that describe the files you will upload. Separate keywords by comma. Keywords make searching for assets easier.
See [Conducting an advanced search](searching-assets.md#conducting_an_advanced_search).

* **BATCH SET PRESETS** &mdash; If you want to create an Image Set, multi-axis Spin Set, or Swatch Set from the uploaded files, click the Active column for the preset you want to use. You can select more than one preset. You create the presets in the Application Setup/Batch Set Presets page.
See [Batch Set Presets](application-setup.md#batch_set_presets).

* **ADVANCED** &mdash; See [Follow an upload with another job](uploading-files.md#follow-an-upload-with-another-job).

## Follow an upload with another job {#follow-an-upload-with-another-job}

When you upload items using FTP, you can schedule a subsequent job to begin as soon as the upload is complete. (If other jobs are scheduled to begin at that time, the job you schedule here will be queued after them.)

The new job sends a notification to the address you specify so that the code at that location can be triggered. This follow-on publishing job uses the same name as the upload job, but with the text *Pub_* added to the beginning.

**To follow an upload with another job**

1. Click **Upload**, then click the **VIA FTP** tab.
1. In the lower-right corner of the Upload page, click **Job Options**.
1. In the Upload Job Options dialog box, expand the **ADVANCED** section.
1. Choose one of the following from the **Follow Upload with another job** drop-down list:

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
   >Regularly scheduled jobs may not result in any files being published.

>[!MORELIKETHIS]
>
>* [Working with asset folders](asset-folders.md#working_with_asset_folders)
>* [Handling recurring upload and publish jobs](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Using an upload or publish job as a trigger](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
