---
title: Managing Info Panel content in eCatalogs
description: Learn how to manage Info Panel content in eCatalogs.
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
---
# Managing Info Panel content in eCatalogs{#managing-info-panel-content-in-ecatalogs}

In addition to using Image Map text for your rollovers in eCatalogs, you can use an Info Panel to add larger quantities of rollover text, including links. You can also manage the InfoPanel by using timed caching and scheduling content updates.

You can manage your InfoPanel setup and data using the following features in Dynamic Media Classic:

* InfoPanel Setup panel lets you specify the template used to display the Info Panel text, a default response for errors, and the number of hours the information is cached. In addition, you can specify whether the eCatalogs is automatically published.
* InfoPanel Datafeed panel lets you specify a CSV file containing the text you want to appear in the InfoPanel rollover text, and schedule times for updating the information.
* Import Metadata dialog box (accessed from the Map Pages view) lets you import a tab-delimited TXT file containing the rollover text information. You can use this TXT option or the Datafeed panel with the CSV file option for your rollover text.
* Map Pages view provides an option for previewing the xml that appears for specific image maps.

## Set up a response template for eCatalogs {#set-up-a-response-template-for-ecatalogs}

You can select one of three preset response templates for displaying text in an Info Panel. These preset response templates determine how your information is presented in the Info Panel: how many columns and rows, typeface size, font, and so on. You can select a preset response template or create one of your own.

>[!NOTE]
>
>You can also set up the Response Template in the Viewer Preset. To use the Response Template in the Viewer Preset instead, add `fmt=1` to the end of the Information Server URL in the Viewer Preset.
>
>See [Setting up eCatalog Viewer Presets](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Double-click your eCatalog to open it in Detail View.
1. Click the InfoPanel Setup panel.
1. Select a Response Template:

    * Select a preset from the Response Template menu. The XML for the template design appears in the User Template box.
    * To create your own response template, select **[!UICONTROL Custom]**. Type the template XML definition in the User Template box. You can use the preset templates as a base for your own.

1. (Optional) In the Default Response box, type the text you want to appear if Dynamic Media Classic encounters an error in retrieving information for an image map. For example, if the system receives a company name and an eCatalog name, but no rollover identifier, this message appears for the user.
1. In the Response TTL box, enter the number of hours you want to wait before caching the data:

    * Set a lower number if the data is updated frequently throughout a day.
    * Set a higher number if the data is relatively stable and doesn’t require updating frequently throughout the day. The default is ten hours.

1. Click **[!UICONTROL Publish]**.

## Import source content for the Info Panel in eCatalogs {#import-source-content-for-the-info-panel-in-ecatalogs}

You can use a comma-separated value file (CSV) or tab-delimited file (TXT) for the source text for an Info Panel for an eCatalog. Tab-delimited files must use UTF16 (Unicode) encoding. You import the different file types using different methods.

When formatting source content, keep in mind the following guidelines:

* Make sure that the tab- and comma-delimited data contains as many columns as are necessary for the rollover template.
* Make sure that the first item or column of data is the rollover identifier (associated with the rollover_key value from the image map URLs). 
* Make sure that each tab- or comma-delimited item after the identifier is the item you want substituted into the response template. So, the first column is substituted into $1$, the second column into $2$, and so on.

### Import CSV content into eCatalogs from an externally hosted location {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Double-click the eCatalog to open it in Detail View.
1. Click the InfoPanel Datafeed panel.
1. Enter the URL for the CSV file in the Externally Hosted CSV File Location box. You can paste the URL into this field or type it directly.
1. (Optional) Specify a time to update the content using the Schedule Update menus and click Add. You can select multiple times for updating. Each update time appears in the Update Times box. (To remove a time, select it and click Delete.)
1. (Optional) Click Run Update Now to immediately update the content.

### Import a tab-delimited or CSV file {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Double-click the eCatalog to open it in Detail View.
1. Click the InfoPanel Setup panel.
1. Click **[!UICONTROL Upload S7Info Content]**.
1. Click **[!UICONTROL Browse]**, select the tab-delimited TXT file, CSV, or SSV file you want to use, and click **[!UICONTROL Open]**.
1. Click **[!UICONTROL Upload]**.

Dynamic Media Classic sends you an e-mail message letting you know if the upload was successful or not.

## Preview rollover key text for an Image Map {#preview-rollover-key-text-for-an-image-map}

Using the Map Pages screen, you can easily and quickly view Info Panel text for the Image Maps on a specific page of your eCatalog.

1. Click the Catalog’s rollover **[!UICONTROL Edit]** button.
1. Click **[!UICONTROL Map Pages]**.
1. At the top of the table on the right side of the screen, choose **[!UICONTROL Info Panel]** from the Show menu.

   The rollover-key text appears next to each Image Map that contains Info Panel text.
