---
title: Managing Info Panel content in Image Sets
seo-title: Managing info panel content in Image Sets
description: null
seo-description: Learn how to manage Info Panel content in Image Sets.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd

---

# Managing Info Panel content in Image Sets{#managing-info-panel-content-in-image-sets}

In addition to using Image Map text for your rollovers in Image Sets, you can use an info panel to add larger quantities of rollover text, including links. You can also manage the InfoPanel by using timed caching and scheduling content updates.  
  
You can manage your InfoPanel setup and data using the following features in Scene7 Publishing System:

* InfoPanel Setup panel lets you specify the template used to display the info panel text, a default response for errors, and the number of hours the information is cached. In addition, you can specify whether the Image Set is automatically published.
* InfoPanel Datafeed panel lets you specify a CSV file containing the text you want to appear in the info panel rollover text, as well as schedule times for updating the information.
* Import Metadata dialog box lets you import a tab-delimited TXT file containing the rollover text information. You can use this TXT option or the InfoPanel Datafeed panel with the CSV file option for your rollover text.

## Set up a response template for Image Sets {#set-up-a-response-template-for-image-sets}

You can select one of three preset response templates for displaying text in an Info Panel. These preset response templates determine how your information is presented in the Info Panel: how many columns and rows, typeface size, font, and so on. You can select a preset response template or create one of your own.

**To set up a response template**

1. Double-click your Image Set to open it in Detail View.
1. Click **InfoPanel Setup** to unfold the panel.
1. In the Response Template drop-down list, do one of the following:

    * Select Default to use the default response. The XML for the template design appears, dimmed, in the User Template text box.
    * Select Custom to create your own response template. In the User Template text box, type the template XML definition. You can use the default template that is already defined in the text box as a base for your own response.

1. (Optional) In the Default Response box, type the text that you want to appear if Dynamic Media Classic encounters an error in retrieving information for an image map. For example, if the system receives a company name and an Image Set name, but no rollover identifier, this message appears for the user.
1. In the Response TTL text field, enter the number of hours that you want to wait before caching the data.

    * Set a lower number if the data is updated frequently throughout the day.
    * Set a higher number if the data is relatively stable and does not require updating frequently throughout the day. The default is ten hours.

1. Click **Upload** to upload info panel content, based on the rollover_key values, to s7info.
1. In the S7Info Upload dialog box, browse to the file that you want to use, and then click **Upload**.

   Supported file formats are TAB delimited files with UTF-16 encoding and CSV files with ASCII encoding. For CSV files, non-ASCII characters must be HTML encoded.

1. In the InfoPanel Setup panel, click **Publish**.

## Import source content for the Info Panel in Image Sets {#import-source-content-for-the-info-panel-in-image-sets}

You can use a CSV (Comma-Separated Value) file with ASCII encoding (non-ASCII character must be HTML encoded) or a tab-delimited file for the source text for an info panel for an Image Set. Tab-delimited files must use UTF-16 (Unicode) encoding. You import the different file types using different methods.

When formatting source content, keep in mind the following guidelines:

* The tab- and comma-delimited data should contain as many columns as are necessary for the rollover template.
* The first item or column of data should be the rollover identifier (associated with the rollover_key value from the image map URLs).
* Make sure that each tab- or comma-delimited item after the identifier is the item that you want substituted into the response template (so the first column is substituted into $1$, the second column into $2$, and so on).

### Import CSV content into Image Sets from an externally hosted location {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Double-click the Image Set to open it in Detail View.
1. Click **InfoPanel Datafeed** to unfold the panel.
1. In the Externally hosted CSV file location (HTTP) text field, enter the URL to the CSV file.
1. (Optional) In the Schedule Update fields, specify a time to update the content, and then click **Add**.

   You can select multiple times for updating. Each update time appears in the Update Times text box. To remove a scheduled time, select it, and then click **Delete**.

1. (Optional) Click **Run Update** to immediately update the content.

