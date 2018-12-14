---
title: Searching assets
seo-title: Searching assets
description: null
seo-description: Learn how to search assets.
uuid: 058209bc-bac4-4d5c-8261-e242a543beaf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: effef4e7-37c5-42e2-9266-ecd026cad628
index: y
internal: n
snippet: y
---

# Searching assets{#searching-assets}

To locate file assets in Scene7 Publishing System, you can view assets by type, sort assets in the Browse Panel, conduct a simple search, conduct an advanced search, and filter for assets.

>[!NOTE]
>
>The Personal Setup screen offers options for choosing how you want to conduct searches. For example, you can choose a default search type and choose whether to include user-defined fields in searches. For more information, see [Personal Setup](personal-setup.md#personal_setup).

## Viewing assets by type {#viewing-assets-by-type}

To see only files of a certain type as you browse, open the Show drop-down menu in the Asset Library, and then choose a file type. Only assets of the type you chose appear in the Asset Library.

## Sorting files in the Browse Panel {#sorting-files-in-the-browse-panel}

To sort the contents of a folder or search results in the Browse Panel, select the Sort menu and choose an option. The options are Name, Size, Type, Date Created, and Last Modified.

You can choose Ascending or Descending to sort assets in ascending or descending order by the criteria you choose.

In List View, you can sort by clicking a column name.

## Conducting a simple search {#conducting-a-simple-search}

Use the Search field to conduct simple searches. You can search for items by name or search for items whose metadata contains a keyword.

To conduct a simple search:

1. Select the folder in the Asset Library to search in a particular folder and its subfolders
1. Click  ![](assets/search_button.png)

   in the Asset Library and choose an option that describes how narrow or broad you want the search to be. You can choose Within All Files & Folders, Within Selected Folder, or Within Selected Folder & Subfolders.
1. Enter a search term.
1. Click Go or press Enter.

   The results of your search appear in the Browse Panel.

>[!NOTE]
>
>Scene7 tracks searches. To run a search a second time, select the Search button and choose the name of a search at the bottom of the Search menu.

## Conducting an advanced search {#conducting-an-advanced-search}

Click Advanced Search in the Asset Library to search using many criteria, including values in metadata fields.

Specify any of the following criteria in your search:

**Filter By Asset Type** Narrow your search to one asset type only by choosing an asset type on the menu.

**Files and Folders** Choose where you want to search: Within All Files & Folders, Within Selected Folder, or Within Selected Folder & Subfolders.

**All Publish States** Search for files that are marked ready for publish, are not marked ready for publish, or all files.

**Conditions** If you specify metadata criteria for searching, select whether the search must match all conditions (an ALL search) or any condition (an OR search).

**Specify Metadata Search Criteria** Create one or more search fields for searching metadata. To create search fields:

1. Open the Metadata View list (to the left of the Add a Field menu) and choose a Metadata View. You can choose compact View, IPTC, XMP, or a view your administrator set up. 
1. Select the Add a Field menu and choose a field name on the drop-down list.
1. Choose a Contains option (Contains, Does Not Contain, Begins With, Ends With, or Equals).
1. For numeric fields, choose a value or enter a custom date range. 
1. (Optional) Repeat steps 1-4 to create more search fields.

You can click the Remove Search Field button to remove a search field.

Click Search to begin your search. The results of the search appear in the Browse Panel. You can change any search condition and click Search to run the search again.

Click Clear to clear search criteria and start a new search. Click Close when you finish searching to close the Search panel.

## Filter assets using metadata {#filter-assets-using-metadata}

Filter assets in the Filters tab of the Asset Library. To filter assets, you use metadata values as the criteria. After you choose a metadata field you want to use for filtering, the Filters tab lists all metadata values that were entered in the field you chose and the number of assets that were assigned each value. For example, in a filter operation on the Creator metadata field, the Filters tab lists all names that were entered in the Creator metadata field for different assets, and for each name, the number of assets assigned the name. You then click a metadata value to see all assets that were assigned that value. In the example, you click the Jimmy metadata value to see all assets in which the name Jimmy was entered in the Creator metadata field. You can filter using more than one metadata field as a filtering criterion.

You can save filter operations in order to run them many times.

>[!NOTE]
>
>Only metadata fields in the default Metadata View can be used for filter operations. The Metadata Views screen shows the name of the default Metadata View.

See [Metadata Views](application-setup.md#metadata_views).

### Running a filter operation {#running-a-filter-operation}

Follow these steps to locate assets by filtering with their metadata values:

1. Click the Filters tab in the Asset Library.

   The criteria of your previous filter operation appear in the Filters pane. The Filters pane is divided into panels, with each panel representing a metadata field. Use the panels to choose which metadata fields to filter with, and within each field, to choose a metadata value for the filter operation.

   To run a filter operation you created and saved, click the Select Preset button and choose the operation’s name on the menu.

   See [Saving, repeating, and deleting filter operations](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. Clicking the Field button  ![](assets/filters_field.png)

   on a panel, follow these instructions to display the filtering menu and construct the filter operation:

   **Choosing&#xA;a metadata field** Select the name of the field on the filtering menu.

   ***note**: Only the names of metadata fields in the default Metadata View appear on the filtering menu.*

   See [Metadata Views](application-setup.md#metadata_views).

   **Adding a metadata field** Choose Add a Panel. After the panel appears on the Filters pane, click its Field button and choose the name of a metadata field on the filtering menu.

   **Removing a metadata field** Choose Remove This Panel on the filtering menu.

   When you choose a metadata field, its panel lists:

    * All metadata values entered in the field.
    * For each metadata value, the number of assets given the value.

1. Repeat Step 2 as many times as necessary to list all metadata fields for the filter operation on panels.
1. In each panel, select a metadata value to filter on. You can’t select more than one metadata value in each panel.

   Assets that match all the values you selected appear in the Browse panel.

   >[!NOTE]
   >
   >To temporarily remove a field from the filter operation, click Deselect All. This option is located at the top of each panel, above metadata values.

1. (Optional) To save the filter operation and be able to run it later, click the Select Preset button, choose Save Current As New Presets, and enter a name in the Save dialog box.

### Saving, repeating, and deleting filter operations {#saving-repeating-and-deleting-filter-operations}

Follow these instructions on the Filters tab to save, repeat, and delete filter operations:

**Saving a filter operation** Click the Select Preset button, choose Save Current As New Presets, and enter a name in the Save dialog box.

**Repeating a filter operation** Click the Select Preset button and choose the name of a filter operation on the menu. The menu lists filter operations that you saved.

**Deleting a filter operation from the Select Preset&#xA;menu** Run the filter operation. Then click the Select Preset button and choose Delete Preset on the menu.

## Using the metadata server {#using-the-metadata-server}

The metadata server is a public API that you can use to search for assets by metadata via http requests.

To configure the metadata server, click Setup &gt; Application Setup &gt; Publish Setup &gt;Metadata Server.

The Metadata Server Publish screen opens. This screen lets you set the following options:

**Instant Publish** Automatically pushes any metadata changes when they are made, including new assets, keyword changes, and so on.

**XMP Packet** Publishes the XMP Packet. This packet is not used for searching, but provides the most up-to-date XMP/

**Keywords** Publishes your keywords to the metadata server for use in searches.

**Metadata Server Publish Fields** Select the fields to include in the metadata. This enables you to determine how much information about your assets is available to the public. These fields are also displayed in Metadata Views, but can only be changed in the metadata server.

Click Publish Now to start the job. A confirmation appears, telling you the job has started.

>[!MORE_LIKE_THIS]
>
>* [Navigation basics](navigation-basics.md#navigation_basics)
>* [Viewing, adding, and exporting metadata](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
