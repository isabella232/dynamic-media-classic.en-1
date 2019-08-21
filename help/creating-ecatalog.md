---
title: Creating an eCatalog
seo-title: Creating an eCatalog
description: null
seo-description: Learn how to create an eCatalog.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932

---

# Creating an eCatalog{#creating-an-ecatalog}

Creating an eCatalog entails ordering the pages, choosing the page layout, and linking the pages by drawing Image Maps and entering rollover and hypertext link data. Optionally, you can customize the TOC so that viewers see page names rather than page numbers in the eCatalog Viewer.

## Creating an eCatalog {#create}

You can include image files as well as PDF files in your eCatalog.

When you create an eCatalog, the **Publish after save** option affects the set and set members in the following ways:

|“Publish after save” option selected before saving?|State of set after saving|State of set members after saving|
|--- |--- |--- |
|Yes|Published|Published|
|No|Unpublished|Set members retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To create an eCatalog**

1. Begin creating your eCatalog with one of these techniques:

   **Select the files first** In the Browse Panel, select files and then click Build > eCatalogs.

   **Start from the eCatalog screen** Click Build > eCatalogs. Select a folder in the Asset Library and drag files from the folder into the Order Pages tab of the eCatalog page.

   ***note**: To view the items in the Asset Library by name instead of thumbnail, select the Name option for Default Asset Library View in Personal Setup. *

1. Select an overall layout for your eCatalog. Click the 1 Up button for single pages, the 2 Up button for double-page spreads, or the Custom button for page spreads of more than two pages. The Change eCatalog Layout dialog box appears. Select the All Spreads options and click **OK**.
1. Optionally, change the layout of individual pages or page spreads by clicking them and then choosing the 1 Up button, 2 Up button, or Custom button. The Change eCatalog Layout dialog box appears. Select the Selected Spreads options and click **OK**.
1. Reorder the pages as necessary with one of these techniques:

   **Dragging** Drag a page or page spread to a new location. The vertical bar shows you where the page is being moved.

   **Move To button** Select a page or page spread, click the Move To button, and choose the page on the menu that you want your page to appear before.

   **Sequence #** In List View, enter page numbers in the Sequence # fields.

1. When you are finished, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Save**.
1. In the Save dialog box, select a folder for storing your eCatalog. In the File Name field, enter the spin set name.
1. Click **Save**.

   You can preview your eCatalog, after you save it, by clicking **Preview**.

## Editing an eCatalog {#editing-an-ecatalog}

Depending on whether you edit a published set or an unpublished set, the **Publish after save** option affects the set and set members in the following ways:

|Set already published?|“Publish after save” option selected before saving your edit?|State of set after saving|State of set members after saving|
|--- |--- |--- |--- |
|Yes|Yes|Published|Published|
|Yes|No|Published|Existing set members retain their published state.Any new set members that you added during your edit retain their published or unpublished state.|
|No|Yes|Published|Published|
|No|No|Unpublished|Existing set members and any new set members that you added during your edit retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To edit an eCatalog**

1. Click the eCatalog’s rollover **Edit** button.
1. Make your changes as necessary.
1. When you are finished editing, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Save**, select a storage folder, enter a name for the set, and then click **Save**.

## Deleting an eCatalog {#deleting-an-ecatalog}

When you delete a set, the set itself is moved to the Trash. However, the members (or “children”) within that set are not affected; instead, they each retain their existing published or unpublished state.

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To delete an eCatalog**

1. In the Grid View, List View, or Details View, select one or more eCatalogs.
1. On the Global Navigation Bar, click **File** &gt; **Delete** &gt; **Delete**.

## Customizing the table of contents (TOC) {#customizing-the-table-of-contents-toc}

Dynamic Media Classic provides default page numbers in your eCatalog on the Order Pages tab of the eCatalog screen. For custom page names, you can change the page labels that constitute the table of contents (TOC). Renaming the front and back cover is recommended. For example, the front cover page can read “Cover” instead of “Page 0-1.”

You can create a customized table of contents (TOC) for your eCatalog manually or by importing the page names from a CSV (Mac only)or XML file.

>[!NOTE]
>
>To restore default page titles, click the TOC Labels button on the Order Pages tab and choose Restore Defaults (All).

### Manually entering page names {#manually-entering-page-names}

To manually enter page names one at a time, go to the Order Pages tab of the eCatalog screen. Then click in the page number field and enter a name. Enter a name for each page you want to name.

### Importing page names {#importing-page-names}

Importing page names is recommended if you are dealing with an eCatalog with many pages. You can import the names from a tab-delimited or XML file.

The TOC label is stored in an image’s User Data field; format this data as a list of `name=<value>` ` pairs separated by two question marks “??” `. For example, to set one label for a TOC field named tocEN ``, set the User Data of the image to:

tocEN=&lt;EN_page_label&gt;

To set separate labels for TOC fields named tocEN and tocFR:

tocEN=&lt;EN_page_label&gt;??tocFR=&lt;FR_page_label&gt;

To import the User Data field in a tab-delimited file, include the field userdata:

|IPSID|Userdata|
|--- |--- |
|`<image_IPS_ID>`|tocEN=<EN_page_label>??tocFR=<FR_page_label>|

To import the User Data field in an XML file, include the attribute `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

To import page names from a tab-delimited or XML file, select the TOC Labels button and choose Import. The Upload Metadata dialog box appears. Click the Browse button and import the CSV file (Mac only) or XML file that associates each page with a page name.
