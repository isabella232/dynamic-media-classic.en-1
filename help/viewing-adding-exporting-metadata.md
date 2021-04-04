---
title: Viewing, adding, and exporting metadata
description: Learn how to view, add, and export metadata.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
feature: Dynamic Media Classic,Asset Management,Metadata
role: Business Practitioner
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
---
# Viewing, adding, and exporting metadata{#viewing-adding-and-exporting-metadata}

You can store information specific to the files you work with in Dynamic Media Classic; this information is called *metadata*. You can use metadata in Dynamic Media Classic for organizing, searching, filtering, and sorting your assets.

Metadata appears in Detail view along with Dynamic Media Classic-generated information, such as the file creation date, publishing date, and keywords. To view metadata, open the asset in Detail view and select the Metadata panel. You can enter and edit metadata in Detail view.

Some metadata is embedded directly into a file. If a file contains this metadata, Dynamic Media Classic automatically uploads it with the file. You can embed metadata into source assets in Adobe Photoshop, InDesign, Illustrator, and other applications; Dynamic Media Classic recognizes this metadata. You can also add metadata to individual files in the Metadata panel in Detail view. To ensure consistency across assets, company administrators create Metadata templates that provide the metadata fields that can be filled in.

For more information about embedded metadata, see [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en).

## View metadata {#view-metadata}

To view an asset’s metadata, open the asset in Detail view, and tap the Metadata panel. To select a set of metadata fields, choose an option on the Metadata View menu. Dynamic Media Classic offers these Metadata Views:

* **Compact View**
A basic list of values.

* **IPTC**
Values as defined by the International Press Telecommunications Council.

* **XMP**
Values as defined by the extensible metadata platform.

Administrators can create Metadata Views. These views also appear on the Metadata Views menu. For information about creating Metadata Views, see [Metadata Views](application-setup.md#metadata_views).

## Manually enter metadata for an asset {#manually-enter-metadata-for-an-asset}

1. Open the asset in Detail view.
1. Open the Metadata panel and do one or both of the following:

    * Choose a Metadata View to determine which metadata fields appear in the panel.
    * Choose a Preset Value and click Apply to populate metadata fields with preset values. Company administrators create these preset values.

1. Enter values in the Metadata panel.

>[!NOTE]
>
>To edit the metadata of several assets at once, select the assets and choose File > Edit Info. Edits you make to metadata in the Edit Info window apply to all the assets you selected.

## Add or edit keywords {#add-or-edit-keywords}

In addition to metadata, you can use keywords to help with searching and managing your assets.

If you’ve added keywords to other files during this session, or if you’ve removed keywords from your list, they appear in the Keyword Suggestions table.

1. Open the file in Detail View.
1. Click Keywords.
1. To add keywords, do any of the following:

    * Type a keyword in the text box and click Add.
    * Click a keyword in the Keyword Suggestions table.

1. To remove a keyword, select it and click Remove. It moves to the Keyword Suggestions table.

>[!NOTE]
>
>You can add keywords to files as you upload them to Dynamic Media Classic. In the Upload Job Options dialog box, choose Additional Metadata and enter keywords. See [Upload options](uploading-files.md#upload_options).

## Import metadata {#import-metadata}

Rather than manually enter metadata one asset at a time, you can import metadata for many different assets from a tab-delimited or XML file. Entering the metadata in a tab-delimited or XML file and importing the file is less time-consuming than entering metadata in individual assets. In the first row of the tab-delimited file, enter the ID and the names of fields for which you want to record metadata. In each subsequent row, enter an asset ID name followed by metadata values. Fields that are not included in the tab-delimited or XML file are not modified. To import metadata from an XML file, make sure that you conform to the DTD.

>[!NOTE]
>
>You can create a template for entering metadata so that it can be properly imported to Dynamic Media Classic. After you create the template, you can use it to enter the metadata. See [Create a template for entering metadata to upload](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

You can find more information about standardized properties at: https://www.adobe.com/devnet/xmp.html

1. In the Browse Panel, select the images to which you want to add metadata from the tab-delimited or XML file.
1. Click **File** > **Import Metadata**.
1. In the **Upload Metadata** dialog box, click **Browse**.
1. In the **Select files to upload** dialog box, select the tab-delimited or XML file with the metadata.
1. Enter a job name.
1. Click **Upload**.

**Identifying different metadata types in the import**

Keep the following in mind when identifying different metadata types to import:

* User-Defined Fields are identified by their name as created in Setup > Application Setup > Metadata > User-Defined fields. Use the Generate file functionality to get a list of all defined UDFs in the correct import format.
* XMP Metadata properties must have the related XMP-prefix before the (property-) name. A colon separates the prefix and name. The XMP prefix can be found in Setup > Application Setup > Metadata > Metadata Schema editor. The technical names can be found in documentation of related XMP schema. XMP properties names do not appear in the Generate file feature.
* Metadata Schema properties must have the related prefix before the (property-) name. A colon separates the prefix and name. The prefix and the property names are defined in the Metadata Schema editor. Metadata Schema properties names do not appear in the Generate file feature.

For example: The XMP property for keywords is the XMP schema "Dublin Core" with the prefix "dc" and “subject” is the technical XMP name. The prefix and technical XMP name are combined into the "dc:subject" full property name. In the XML metadata import format, "dc.subject" must be the property name. In the tab-delimited import format, it must be the column-header.

**Import Keywords**

Keywords can be imported as comma-separated list. If a comma appears in any of the individual values, it must be escaped by a backslash (\). A literal backslash is the usual double-backslash (\\).

For example, a metadata import file containing the value "Hello\, World!,back\\slash,foo" for "dc:subject" sets three XMP keywords on the asset: "Hello, World!," "back\slash," and "foo."

**Import XMP and Metadata Schema metadata XMP files**

The XML import accepts only valid XML. When importing XMP or Metadata Schema fields, the namespace prefix is added and behaves here like a XMP-namespace. This namespace must be declared. For example, in the top-level tag.

For example:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

**Import XMP and Metadata Schema metadata Tab Delimited files**

The prefix must be added to the related column header of the import field.

## Import metadata (via FTP) {#import-metadata-via-ftp}

You can import metadata for multiple files by entering the metadata in a tab-delimited or XML file and selecting the Process metadata files option on the Upload (Via FTP) screen.

Make sure the data in the tab-delimited or XML file is in the correct format. In the first row, enter the ID field followed by the names of metadata fields to be modified. In each subsequent row, enter an asset ID name followed by metadata values. Fields that are not included in the tab-delimited or XML file are not modified.

Click the Upload button on the Global Navigation Bar. To import the metadata, on the Jobs screen, select the **[!UICONTROL Via FTP]** tab, then click **[!UICONTROL Job Options]**. In the Upload Job Options dialog box, choose Process metadata files.

## Batch rename IDs using metadata {#batch-rename-ids-using-metadata}

Using metadata imported from a tab-delimited file or XML file, you can rename Dynamic Media Classic IDs. The imported metadata is applied only to the images specified in the metadata file itself. It doesn't matter whether images are selected on the Browse Panel.

To rename an image’s Dynamic Media Classic ID, add a column labeled *newipsid* to the tab-delimited file, or add a field called* new_vc_objectname* to the XML data.

For example:

|ipsid|newipsid|
|--- |--- |
|testjacket_1|Jacket_test_1|
|testjacket_blue|Jacket_test_2|

The job log for the Metadata job shows which IDs were successfully renamed and which ones were not.

## Create a template for entering metadata to upload {#create-a-template-for-entering-metadata-to-upload}

Dynamic Media Classic offers a command for creating a template for recording metadata. Using the template ensures that the metadata is entered in the right format so it can be uploaded correctly to Dynamic Media Classic. To create a template for use in recording and importing metadata to Dynamic Media Classic, follow these steps:

1. Select image assets with metadata fields you want for your template.
1. Choose File > Import Metadata.
1. Select Image for the Asset Properties Type.
1. From the Generate File menu, select Tab Delimited Template, Asset's XML Metadata, or XML DTD.
1. Click Generate.
1. In the dialog box that appears, copy the data. Use this data to construct the template.

## Working with Metadata Schemas {#working-with-metadata-schemas}

A company administrator can view a list of all available schemas. Open Application Setup -> Metadata -> Metadata Schema.

Initially, the list of global standard schemas like XMP is hidden. They can be shown using the checkbox at the bottom of the list.

The company administrator can create a custom schema, or edit an existing custom schema.

You can use the Metadata Schema Editor to perform the following actions:

|Action|Description|
|--- |--- |
|Add|Adds a property to the schema. A modal dialog collects the information: ID, Label, Structure, and Data Type.|
|Add Choice Value|Adds a new selectable choice to a property with structure Open Choice or Closed Choice. All choice values have the same type. Select the property itself to enable the button.|
|Edit|Edit the Label of a property or choice value. You can only change the Label, ID, and type information is immutable.|
|Move Up / Move Down|The order in the schema is reflected in the UI. To change the order, select a property or choice value and move it with the buttons. Drag & drop is not supported currently.|
|Delete|Deletes a property or choice value from the schema. It does not delete values from the XMP block or the Database. The property is no longer available for Metadata Views and is removed from the Asset Detail View. If the property was published to the Metadata Server, perform a force publish to remove the data from the public-facing Metadata Server.|

The system automatically generates a custom schema for User-defined fields with the prefix "s7udf". It is existing User-defined Fields and they are edited in their own Setup section.

>[!NOTE]
>
>Changes to the schema never change the asset metadata itself. However, they are not visible for all Dynamic Media Classic and Metadata Server functionality and can't be accessed after being changed. Likewise, if metadata for an asset exists, the creation of the matching schema makes the metadata usable in Dynamic Media Classic and the Metadata Server.

The Metadata Schema Editor offers a graphical way to add or edit a custom company schema inside Dynamic Media Classic. A schema is defined by a prefix, a namespace, and a list of properties.

* Name

  UI-Name for the schema. Used to identify the properties in Metadata Views and Advanced Search. Similar to XMP Sections like Basic, IPTC, PDF.

* Prefix

  Technical unique identifier for the schema. Restricted to the letters a-z and A-Z. The prefix is not visible in the Dynamic Media Classic UI, but used, when metadata for an asset is stored in the XMP block and the database. The prefix is used, to uniquely identify metadata fields in metadata search queries on the Metadata Server or import.

* Namespace

  Technical unique identifier for the schema, typically a URL in the form `https://your.company.com/name/version/`. See the list of standard schemas for examples. The namespace is not visible in the Dynamic Media Classic UI, but is used to store metadata in the XMP block.

* Description

  Free form description of the schema.

>[!NOTE]
>
>The prefix and namespace cannot be edited. To change these properties, you must delete and re-create the schema.

Properties describe the metadata that can be stored with this schema in the XMP block. A property consists of:

|Property|Description|
|--- |--- |
|ID|Technical identifier for this property. The ID is not visible in the Dynamic Media Classic UI, but used, when metadata for an asset is stored in the XMP block and the database. The ID is used, to create search queries on the Metadata Server. The ID has some restrictions such as: <ul><li>No spaces</li><li>No ".", ":", "$"</li><li>No number as first character</li><li>Best practice is to use a-z or A-Z as first character</li></ul> <br>Once created, the ID cannot be changed.|
|Label|UI-Name for this property.|
|Structure|Determines the type of the property together with Data Type. Structure can be one of:<ul><li>Simple Type: single value of data type</li><li>Sequence: a list of values of the same data type</li><li>Open Choice: select one item from a list of predefined values, or enter free text. Can be only of data type String or Integer</li><li>Closed Choice: select one item from a list of predefined values (a popup or combo-box)</li></ul>|
|Data Type|Select from these available types: <ul><li>String</li><li>Integer</li><li>Float</li><li>Yes/No (Boolean)</li><li>Date</li></ul>|


When the property has the structure Open Choice or Closed Choice, you must provide at least one Choice Value. Open Choice can be changed. Closed Choice cannot be changed. All Choice Values have the data type of the property.

|Property|Description|
|--- |--- |
|ID|Technical identifier for this value. The ID is not visible in the Dynamic Media Classic UI, but is used when metadata for an asset is stored in the XMP block and the database. The ID is used in search queries on the Metadata Server. The ID cannot contain any spaces. Once created, the ID cannot be changed.|
|Label|UI-Name for this value.|

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)
>* [Metadata Presets](application-setup.md#metadata_presets)
