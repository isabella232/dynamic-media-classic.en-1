---
title: Create an eCatalog
description: Learn how to create an eCatalog in Dynamic Media Classic.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
---
# Creating an eCatalog {#creating-an-ecatalog}

Creating an eCatalog entails ordering the pages, choosing the page layout, and linking the pages by drawing Image Maps and entering rollover and hypertext link data. Optionally, you can customize the TOC so that viewers see page names rather than page numbers in the eCatalog Viewer.

## Create an eCatalog {#create}

You can include image files and PDF files in your eCatalog.

When you create an eCatalog, the **[!UICONTROL Publish after save]** option affects the set and set members in the following ways:

|“Publish after save” option selected before saving?|State of set after saving|State of set members after saving|
| --- | --- | --- |
|Yes|Published|Published|
|No|Unpublished|Set members retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To create an eCatalog:**

1. Begin creating your eCatalog with one of these techniques:

   * **Select the files first** - In the Browse Panel, select files and then go to **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**.

   * **Start from the eCatalog screen** - Go to **[!UICONTROL Build]** > **[!UICONTROL eCatalogs]**. Select a folder in the Asset Library and drag files from the folder into the Order Pages tab of the eCatalog page.

      >[!NOTE]
      >
      >To view the items in the Asset Library by name instead of thumbnail, select the Name option for Default Asset Library View in Personal Setup.

1. Select an overall layout for your eCatalog. Select **[!UICONTROL 1 Up]** for single pages, **[!UICONTROL 2 Up]** for double-page spreads, or **[!UICONTROL Custom]** for page spreads of more than two pages. In the **[!UICONTROL Change eCatalog Layout]** dialog box, select the **[!UICONTROL All Spreads]** options and select **[!UICONTROL OK]**.
1. Optionally, change the layout of individual pages or page spreads by selecting them and then choosing **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]**, or **[!UICONTROL Custom]** button. In the **[!UICONTROL Change eCatalog Layout]** dialog box, select the **[!UICONTROL Selected Spreads]** options and select **[!UICONTROL OK]**.
1. Reorder the pages as necessary with one of these techniques:

   * **Dragging** - Drag a page or page spread to a new location. The vertical bar shows you where the page is being moved.

   * **Move To button** - Select a page or page spread, select **[!UICONTROL Move To]**, and choose the page on the menu that you want your page to appear before.

   * **Sequence #** - In List View, enter page numbers in the Sequence # fields.

1. When you are finished, near the lower-right corner of the page, ensure that **[!UICONTROL Publish after save]** is selected (default).
1. Select **[!UICONTROL Save]**.
1. In the Save dialog box, select a folder for storing your eCatalog. In the File Name field, enter the spin set name.
1. Select **[!UICONTROL Save]**.

   You can preview your eCatalog, after you save it, by selecting **[!UICONTROL Preview]**.

## Edit an eCatalog {#editing-an-ecatalog}

Whether you edit a published set or an unpublished set, the **[!UICONTROL Publish after save]** option affects the set and set members in the following ways:

|Set already published?|“Publish after save” option selected before saving your edit?|State of set after saving|State of set members after saving|
| --- | --- | --- | --- |
| Yes | Yes | Published | Published |
| Yes | No | Published | Existing set members retain their published state. Any new set members that you added during your edit retain their published or unpublished state.|
| No | Yes | Published | Published |
| No | No | Unpublished | Existing set members and any new set members that you added during your edit retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To edit an eCatalog:**

1. Select the eCatalog’s rollover **[!UICONTROL Edit]** button.
1. Make your changes as necessary.
1. When you are finished editing, near the lower-right corner of the page, ensure that **[!UICONTROL Publish after save]** is selected (default).
1. Select **[!UICONTROL Save]**, select a storage folder, enter a name for the set, and then select **[!UICONTROL Save]**.

## Delete an eCatalog {#deleting-an-ecatalog}

When you delete a set, the set itself is moved to the Trash. However, the members (or “children”) within that set are not affected; instead, they each retain their existing published or unpublished state.

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To delete an eCatalog:**

1. In the Grid View, List View, or Details View, select one or more eCatalogs.
1. On the Global Navigation Bar, go to **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.

## Customize the table of contents (TOC) {#customizing-the-table-of-contents-toc}

Dynamic Media Classic provides default page numbers in your eCatalog on the Order Pages tab of the eCatalog screen. For custom page names, you can change the page labels that constitute the table of contents (TOC). Renaming the front and back cover is recommended. For example, the front cover page can read “Cover” instead of “Page 0-1.”

You can create a customized table of contents (TOC) for your eCatalog manually or by importing the page names from a CSV (Mac only) or XML file.

>[!NOTE]
>
>To restore default page titles, on the **[!UICONTROL Order Pages]** tab, select **[!UICONTROL TOC Labels]**, and then select **[!UICONTROL Restore Defaults (All)]**.

### Manually entering page names {#manually-entering-page-names}

To manually enter page names one at a time, go to the Order Pages tab of the eCatalog screen. Then, in the page number field, enter a name for each page you want to name.

### Import page names {#importing-page-names}

Importing page names is recommended if you are dealing with an eCatalog with many pages. You can import the names from a tab-delimited or XML file.

The TOC label is stored in an image’s User Data field; format this data as a list of `name=<value>` ` pairs separated by two question marks “??” `. For example, to set one label for a TOC field named `tocEN`, set the User Data of the image to:

`tocEN=&lt;EN_page_label>`

To set separate labels for TOC fields named `tocEN` and `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

To import the User Data field in a tab-delimited file, include the field user data:

|IPSID|User data|
| --- | --- |
|`<image_IPS_ID>`| `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

To import the User Data field in an XML file, include the attribute `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

To import page names from a tab-delimited or XML file, select the **[!UICONTROL TOC Labels]** button and select **[!UICONTROL Import]**. In the Upload Metadata dialog box, select **[!UICONTROL Browse]**, and then import the CSV file (Mac only) or XML file that associates each page with a page name.
