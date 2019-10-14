---
title: "Quick Start: eCatalogs"
seo-title: "Quick Start: eCatalogs"
description: null
seo-description: An introduction and Quick Start to eCatalogs to help you get up and running quickly with eCatalog techniques.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d

---

# Quick Start: eCatalogs{#quick-start-ecatalogs}

An eCatalog is a digital, web version of print material—a catalog, brochure, flyer, product manual, or advertising circular, for example. An eCatalog is displayed in an eCatalog Viewer on a web site. This viewer simulates the experience of reading printed material. Depending on the settings you choose for your eCatalog, the viewer can let you do the following:

* Search the catalog for a keyword or keywords. The search results are displayed as a list of thumbnails in a search panel on the left side of the catalog. Each clickable thumbnail represents a catalog spread where the highlighted search term was found.

* Share the catalog by way of social media; download the catalog to view offline; enable Favorites to mark items you want to return to quickly, or print the catalog.
* Navigate the catalog using the table of contents or the page grid view; page forward or backward by clicking the middle edge of a page.
* Zoom in, zoom out, and pan to examine items on a page.
* Move the pointer over a page region (called an Image Map) to see a pop-up window with information about an item.
* Click a page region to open a new web page with more information about an item.
* Write a sticky note and attach it to an eCatalog page.
* Tap image map icons to launch related web pages or in-context info panels.
* Use gesture interactions, including pinching to zoom and swiping to turn pages.
* Search by keyword for items.

![The eCatalog as it looks to users. A) eCatalog opening page. B)eCatalog turned to page 2.](/help/assets/ec_cat_viewer_popup.png)

To create an eCatalog, you typically use high-resolution PDF files created in Adobe® Acrobat® or another print program, but you can also create an eCatalog from image files.

As part of creating your eCatalog, you can arrange pages or page spreads in the order you choose. You can also declare whether you want single pages, double-page spreads, or multi-page spreads. You can create Image Maps for page regions so that viewers can, for example, click an area on the page and open a new page on your web site. You can manage the rollover text that appears using InfoPanel settings within the eCatalog screen. You can also configure the eCatalog Viewer by choosing from more than 100 different configuration options. You can tailor the features and the appearance of your Viewer for your particular audience.

>[!NOTE]
>
>If you are an AEM Dynamic Media - Scene7 mode user and want to use eCatalogs, you will need to edit the `pdfbrochure` value in CRXDE Lite. To do so, in AEM, click **[!UICONTROL Tools > General > CRXDE Lite]**. In the left panel navigation tree, navigate to `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
In the lower right pane, in the **[!UICONTROL Properties]** tab, select the `jobParam` row. Set the value for `pdfbrochure` from `false` to `true`. As in `pdfbrochure=true`
In the upper-left corner of the CRXDE Lite page, click **[!UICONTROL Save All]**.
You will now be able to author eCatalogs in SPS.

**Quick Start**

This eCatalog Quick Start is designed to help you get up and running quickly with eCatalogs. Follow steps 1 through 7. After each step is a cross-reference to a topic heading where you can find more information.

**1. Uploading the PDF files**

Adobe PDF files are usually the source for an eCatalog. Because they are meant to be printed, PDF files usually contain CMYK images. The Scene7 Publishing System detects these images and converts them using a standard CMYK color profile. However, you may have to upload and use a custom color profile.

Click Upload on the Global Navigation bar to start uploading PDF files or images for your eCatalog. You can upload files from your desktop or via FTP; FTP is recommended if you are uploading many files or files larger than 100 MB.

Under PDF Options, the Upload screen provides options for uploading PDF files at the proper resolution and correct color space. A 150 pixels-per-inch resolution is recommended. You can select the Auto-Generate eCatalog option to create an eCatalog when you upload a PDF file.

See [Uploading the PDF files](uploading-pdf-files.md#uploading_the_pdf_files).

**2. Creating an eCatalog**

Create your eCatalog by selecting PDF or image files in the Browse Panel, and then clicking the Build button and choosing eCatalogs. The eCatalog screen opens.

On the Order Pages tab, select a Layout button—1 Up, 2 Up, or Custom—to choose whether you want single, double, or custom page spreads. You can rearrange pages or spreads by dragging them or, in a large eCatalog, choosing a page name on the Move To menu.

To add pages, select a folder in the Asset Library, and then drag PDF or image files from into the Order Pages screen. Instead of default page numbers, you can provide custom page names or import a large number of page names.

Click **[!UICONTROL Save]**, enter a name for your eCatalog, choose an SPS folder for storing it, and click **[!UICONTROL Save]**. Each time you change the page order or edit your eCatalog, save your changes by clicking **[!UICONTROL Save]**.

See [Creating an eCatalog](creating-ecatalog.md).

**3. Creating Image Maps**

Image Maps add another dimension to eCatalog pages. An Image Map is a region on a page that delivers more information about an item. When viewers roll the pointer over an Image Map, they see a description of the item. Clicking an Image Map activates an external reference that opens a new web page where you can learn more about an item.

To create an Image Map, open the eCatalog screen. Then go to the **[!UICONTROL Map Pages]** tab of the eCatalog screen, and draw the map with the Rectangle Image Map tool or Polygon Image Map tool. You can adjust the position and size of Image Maps by dragging map borders with the Pan tool.

After you draw the Image Map, enter the URL address that you want to go to when you click the Image Map. You can also enter the rollover text that appears when you move your pointer over the Image Map.

See [Creating eCatalog Image Maps](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

See [Using Image Maps to embed rich media in an eCatalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

You can set up and manage the image map text using the Info Panel settings in the eCatalog screen.

See [Managing Info Panel content](info-panel-content.md#managing-info-panel-content).

**4. Setting up eCatalog Viewer Presets**

End users see your eCatalog in the eCatalog Viewer. If you are an administrator, you can configure the eCatalog Viewer. You can change its outline color and select a new “skin” to brand your eCatalog. Dynamic Media Classic comes with several “best practice” eCatalog Viewer Presets. You can choose one of these presets for displaying your eCatalogs. You can also create an eCatalog Viewer Preset of your own if you are an administrator.

To create an eCatalog Viewer Preset, on the Global Navigation bar, click **[!UICONTROL Setup]** and choose **[!UICONTROL Viewer Presets]**. Then click **[!UICONTROL Add]**, choose a platform, then click **[!UICONTROL eCatalog > Viewer]**.

See [Setting up eCatalog Viewer Presets](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

**5. Previewing eCatalogs in the eCatalog Viewer**

eCatalog Viewer Presets determine the style and behavior of your eCatalog Viewers.

To find out how eCatalog Viewer Presets display your eCatalog, select your eCatalog in the Browse Panel and click **[!UICONTROL Preview]**. The Preview screen opens in the default viewer.

Notice the orientation, color scheme, what the controls for changing pages look like, and what pages look like when they are turned.

See [Previewing eCatalogs in the eCatalog Viewer](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

**6. Publishing eCatalog and associated PDFs**

Publishing your eCatalog and associated PDF places it on Dynamic Media Image Servers so that it can be delivered to your web site and application. As part of the publishing process, the Scene7 Publishing System activates the URL string for your eCatalog. Use this URL to call the eCatalog from Dynamic Media Image Servers to your web site or application.

After marking your eCatalog and PDF for publish in the Browse Panel, select the Publish button on the Global Navigation bar to initiate a publish. On the Publish screen, click **[!UICONTROL Start Publish]**.

See [Publishing eCatalogs and associated PDFs](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

**7. Linking an eCatalog to a web page**

Dynamic Media Classic activates the URL callout string necessary for displaying your eCatalog when you publish it to Dynamic Media Image Servers. You can copy this URL string from the Preview screen and the Browse Panel (in Detail view) by selecting URLs in the panel. After you copy the URL string, it is available to your web sites and applications.

Work with your IT team to place the link to the eCatalog in the appropriate place in your web page. When users click the link, the eCatalog Viewer appears and users can browse your eCatalog.

See [Linking an eCatalog to a web page](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
