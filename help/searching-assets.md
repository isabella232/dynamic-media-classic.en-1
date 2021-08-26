---
title: Searching assets
description: Learn how to search assets.
uuid: 058209bc-bac4-4d5c-8261-e242a543beaf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: effef4e7-37c5-42e2-9266-ecd026cad628
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3f690c-7dff-4bf0-9366-085ba918fe6b
---
# Searching assets{#searching-assets}

To locate file assets in Adobe Dynamic Media Classic, you can view assets by type, sort assets in the Browse Panel, conduct a simple search, conduct an advanced search, and filter for assets.

>[!NOTE]
>
>The Personal Setup page offers options for choosing how you want to conduct searches. For example, you can choose a default search type and choose whether to include user-defined fields in searches. For more information, see [Personal Setup](personal-setup.md#personal_setup).

## Viewing assets by type {#viewing-assets-by-type}

To see only files of a certain type as you browse, in the Asset Library on the left side, in the **[!UICONTROL Show]** drop-down list, choose a file type. Only assets of the type you chose to show, appear in the Asset Library.

>[!NOTE]
>
>If you do not see the Asset Library panel on the left side, click the right triangle arrow on the left side, half way down the Adobe Dynamic Media Classic window, to open the Asset Library.)

## Sorting files in the Browse Panel {#sorting-files-in-the-browse-panel}

To sort the contents of a folder or search results that appear in the Browse Panel on the right side, on the Global Navigation bar, click **[!UICONTROL Sort]**, and then choose an option. The options are **[!UICONTROL Name]**, **[!UICONTROL Size (KB)]**, **[!UICONTROL Type]**, **[!UICONTROL Date Created]**, and **[!UICONTROL Last Modified]**.

You can also choose **[!UICONTROL Ascending]** or **[!UICONTROL Descending]** to sort assets in ascending or descending order by the criteria you choose.

In List View, you can sort by clicking a column name.

## Conducting a simple search {#conducting-a-simple-search}

Use the Search field in Asset Library so you can conduct simple searches. You can search for items by name or search for items whose metadata contains a keyword.

1. In the Asset Library, in the **[!UICONTROL Folders]** panel, select the folder to search in a particular folder and its subfolders.
1. To the left of the Search field in the Asset Library, click the **[!UICONTROL Magnifying Glass]** icon to open the drop-down list.
1. In the drop-down list, choose an option that describes how narrow or broad you want the search to be. You can choose **[!UICONTROL Within All Files & Folders]**, **[!UICONTROL Within Selected Folder]**, or **[!UICONTROL Within Selected Folder & Subfolders]**.
1. In the Search field, enter a search term.
1. To the right of the Search field, click **[!UICONTROL Go]** or press **[!UICONTROL Enter]**.

   The results of your search appear in the Browse Panel on the right.

<!-- Does not appear to be working anymore >[!NOTE]
>
>Adobe Dynamic Media Classic tracks searches. To run a search a second time, click **[!UICONTROL Search]** and choose the name of a search at the bottom of the Search menu. -->

## Conducting an advanced search {#conducting-an-advanced-search}

In the Asset Library, directly below the Search field, click **[!UICONTROL Advanced Search]** to search using many criteria, including values in metadata fields.

Specify any of the following criteria in your advanced search:

* **Filter By Asset Type** - Narrow your search to one asset type only by choosing an asset type on the menu.

* **Files and Folders** - Choose where you want to search: **[!UICONTROL Within All Files & Folders]**, **[!UICONTROL Within Selected Folder]**, or **[!UICONTROL Within Selected Folder & Subfolders]**.

* **All publish states** - Search for files that are marked ready for publish, are not marked ready for publish, or all files.

* **Conditions** - If you specify metadata criteria for searching, select whether the search must match all conditions (an ALL search) or any condition (an OR search).

* **Search Criteria** - Create one or more search fields for searching metadata. To create search fields:

   1. In Advanced Search, under the **[!UICONTROL Search criteria]** heading, and to the left of the **[!UICONTROL Add a Field]** menu), click the down triangle arrow icon to open the drop-down list. Choose a Metadata view. You can choose **[!UICONTROL All properties with values]**, **[!UICONTROL Compact View]**, **[!UICONTROL IPTC]**, **[!UICONTROL Metadata Server Publish Fields]**, or **[!UICONTROL XMP]**.
   1. Click the **[!UICONTROL Add a Field]** drop-down menu and choose a field name.
   1. Choose a **[!UICONTROL Contains]** option: **[!UICONTROL Contains]**, **[!UICONTROL Does Not Contain]**, **[!UICONTROL Begins With]**, **[!UICONTROL Ends With]**, or **[!UICONTROL Equals]**.
   1. For numeric fields, choose a value or enter a custom date range. 
   1. (Optional) Repeat steps 1-4 to create more search fields.

Click the **[!UICONTROL Remove search field]** icon (circle with "X" inside) so the search field is deleted.

In the lower right corner of the Advanced Search panel, click **[!UICONTROL Search]** to begin your search. The results of the search appear in the Browse Panel on the right. You can change any search condition and click **[!UICONTROL Search]** to run the search again.

Click **[!UICONTROL Clear]** to clear search criteria and start a new search. Click **[!UICONTROL Close]** when you finish searching to close the Search panel.

## Filter assets using metadata {#filter-assets-using-metadata}

Filter assets in the Filters tab of the Asset Library. To filter assets, you use metadata values as the criteria. After you choose a metadata field you want to filter on, the Filters tab lists all metadata values that were entered in the field you chose. It also lists the number of assets that were assigned each value. For example, in a filter operation on the Creator metadata field, the Filters tab lists all names that were entered in the Creator metadata field for different assets. It also lists for each name, the number of assets assigned the name. You then click a metadata value to see all assets that were assigned that value. In the example, you click the Prairie Cat metadata value to see all assets in which the name Prairie Cat was entered in the Creator metadata field. You can filter using more than one metadata field as a filtering criterion.

You can save filter operations to run them many times.

>[!NOTE]
>
>Only metadata fields in the default Metadata View can be used for filter operations. The Metadata Views page shows the name of the default Metadata View.

See [Metadata Views](application-setup.md#metadata_views).

### Running a filter operation {#running-a-filter-operation}

Follow these steps so you can locate assets by filtering with their metadata values:

1. In the Asset Library, click the **[!UICONTROL Filters]** tab.

   The criteria of your previous filter operation appear in the Filters pane. The Filters pane is divided into panels, with each panel representing a metadata field. Use the panels to choose which metadata fields to filter with, and within each field, to choose a metadata value for the filter operation.

   To run a filter operation you created and saved, click **[!UICONTROL Select Preset]**, and then choose the operation’s name on the menu.

   See [Saving, repeating, and deleting filter operations](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. Click **[!UICONTROL Field]** on a panel, then follow these instructions so you can display the filtering menu and construct the filter operation:

   * **Choosing a metadata field** - Select the name of the field on the filtering menu.

      >[!NOTE]
      >
      >Only the names of metadata fields in the default Metadata View appear on the filtering menu.

      See [Metadata Views](application-setup.md#metadata_views).

   * **Adding a metadata field** - Click **[!UICONTROL Add a Panel]**. After the panel appears on the Filters pane, click its **[!UICONTROL Field]** button and choose the name of a metadata field on the filtering menu.

   * **Removing a metadata field** - Click **[!UICONTROL Remove This Panel]** on the filtering menu.

   When you choose a metadata field, its panel lists the following:

    * All metadata values entered in the field.
    * For each metadata value, the number of assets given the value.

1. Repeat Step 2 as many times as necessary to list all metadata fields for the filter operation on panels.
1. In each panel, select a metadata value to filter on. You cannot select more than one metadata value in each panel.

   Assets that match all the values you selected appear in the Browse panel.

   >[!NOTE]
   >
   >To temporarily remove a field from the filter operation, click **[!UICONTROL Deselect All]**. This option is at the top of each panel, above metadata values.

1. (Optional) To save the filter operation and be able to run it later, click **[!UICONTROL Select Preset]** > **[!UICONTROL Save Current As New Presets]**, and then enter a name in the **[!UICONTROL Save]** dialog box.

### Saving, repeating, and deleting filter operations {#saving-repeating-and-deleting-filter-operations}

Follow these instructions on the Filters tab so you can save, repeat, and delete filter operations:

* **Saving a filter operation** - Click **[!UICONTROL Select Preset]** > **[!UICONTROL Save Current As New Presets]**, and then enter a name in the **[!UICONTROL Save]** dialog box.

* **Repeating a filter operation** - Click **[!UICONTROL Select Preset]** and choose the name of a filter operation on the menu. The menu lists filter operations that you saved.

* **Deleting a filter operation from the Select Preset menu** - Run the filter operation. Then, click **[!UICONTROL Select Preset]** > **[!UICONTROL Delete Preset]** on the menu.

## Using the metadata server {#using-the-metadata-server}

The metadata server is a public API that you can use to search for assets by metadata via http requests.

To configure the metadata server, click **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Metadata Server]**.

The Metadata Server Publish page lets you set the following options:

* **Instant Publish** - Automatically pushes any metadata changes when they are made, including new assets, keyword changes, and so on.

* **XMP Packet** - Publishes the XMP Packet. This packet is not used for searching, but provides the most up-to-date XMP.

* **Keywords** - Publishes your keywords to the metadata server for use in searches.

* **Metadata Server Publish Fields** - Select the fields to include in the metadata. This option lets you determine how much information about your assets is available to the public. These fields are also displayed in Metadata Views, but can only be changed in the metadata server.
 
Click **[!UICONTROL Publish Now]** to start the job. A confirmation appears, telling you the job has started.

>[!MORELIKETHIS]
>
>* [Navigation basics](navigation-basics.md#navigation_basics)
>* [Viewing, adding, and exporting metadata](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
