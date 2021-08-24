---
title: Create eCatalog Image Maps
description: Learn how to create eCatalog image maps in Dynamic Media Classic.
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
---
# Create eCatalog Image Maps{#creating-ecatalog-image-maps}

An Image Map is a region on an eCatalog page that you can roll over with your mouse or select to trigger actions of various kinds. When you move the pointer over an Image Map for example, you see a rollover-text description of an item. When you select an Image Map, another action is initiated. For example, you can open a web page so that viewers can learn more about an item or purchase it or you can launch a video to see an item in use.

## Draw eCatalog Image Maps {#drawing-ecatalog-image-maps}

For eCatalogs, you draw Image Maps on the Map Pages tab of the eCatalog screen. This screen consists of the Image Map area where eCatalog pages are displayed and, on the right, the Image Map list. As you create Image Maps, their names are entered on the Image Map List.

1. Select the eCatalog’s rollover **[!UICONTROL Edit]** button.
1. Select **[!UICONTROL Map Pages]**.
1. On the left of the Map Pages screen, select the page you want.
1. In the Image Map area, draw a rectangular or polygonal (many-sided) Image Map:

    * **Rectangular map** - Select the Rectangle Image Map tool and drag on the page to create the rectangle.

    * **Polygonal map** - Select the Polygon Image Map tool, then select as many times as necessary around the perimeter of the image. As you select, Dynamic Media Classic draws the borders of the Image Map.

        After you draw an Image Map, Dynamic Media Classic assigns it a name in the Image Map list. To form the name, Dynamic Media Classic appends a sequential number to the name of the eCatalog page in which you are working.

1. (Optional) From the Image Map list, in the [!UICONTROL Name] column, you can enter a new name for the Image Map. Do not include blank spaces in the name you enter.
1. You can have viewers open a new web page when they select the Image Map. In the Image Map list panel, enter the URL of the web page in the URL column.

   To make entering URLs (Href templates) easier, select **[!UICONTROL Edit]** and enter a template.

See [Use a template to enter JavaScript and URLs](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Optional) In the Show drop-down list, select **[!UICONTROL Rollover Text]**, and then enter the text that you want users to see onscreen when they move their pointers over the Image Map.
1. (Optional) In the Show drop-down list, select **[!UICONTROL Other Actions]**, and enter an attribute to trigger a blur or focus action when users move their pointers over an Image Map.

   See [Define other actions for Image Maps](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Select **[!UICONTROL Save]**.
1. (Optional) Select **[!UICONTROL Preview]** to view the eCatalog with the default eCatalog Viewer preset.

To delete an Image Map, select its name in the Image Map list and select **[!UICONTROL Delete]**. To temporarily disable an Image Map on a page without deleting the Image Map, deselect the Image Map’s On option in the Image Map List panel.

## Embed rich media in an eCatalog {#embedding-rich-media-in-an-ecatalog}

You can use eCatalog’s Rich Media option to add videos in MP4 format or spin sets to Image Maps that you have added to an eCatalog. When a user selects the Image Map area in the eCatalog, the associated spin set or video is displayed. This functionality is especially helpful if you want customers to see an item in use or see an item from different angles and perspectives.

You can also optionally display tooltip text when customers move their pointers over your Image Map so they know what they are selecting.

**To embed rich media in an eCatalog:**

1. Draw an eCatalog Image Map.

   See [Draw eCatalog Image Maps](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. In the Show drop-down list, select **[!UICONTROL Rich Media]**.
1. In the Add Assets panel on the left, navigate to a folder that contains the spin set or video (MP4 format) asset that you want to embed.
1. Drag the asset onto the Image Map. 
1. (Optional) In the Image Map list panel, under the **[!UICONTROL Tool Tip]** column header, enter the text that you want viewers to see onscreen when they move their pointer over the Image Map.
1. Select **[!UICONTROL Save]**.

## Editing eCatalog Image Maps {#editing-ecatalog-image-maps}

Starting on the Map Pages tab of the eCatalog screen, use these techniques to edit eCatalog Image Maps:

* **Adjust the position** - Select the Pan tool and move the pointer near but not over the border of the map. When the pointer shows a four-headed arrow, drag the entire image map to a new location.

    See [Adjust the position, shape, and size of Image Maps](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Change the shape and size** - To resize a rectangular Image Map, select the Pan tool. Then move the pointer over a borderline or a corner, and when you see the double-headed arrow icon, drag. To resize a polygonal Image Map, drag a square selection handle. To create a selection handle, select the border of the Image Map and drag.

    See [Adjust the position, shape, and size of Image Maps](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Deleting Image Maps** - Select the Pan tool, select the Image Map to select it, and then select **[!UICONTROL Delete]**.

    To remove all Image Maps from an eCatalog, select the **[!UICONTROL Order Pages]** tab, and then select **[!UICONTROL Clear Maps]**.

* **Handling overlapping Image Maps** - Drag to change the order of Image Maps on the Image Map list.

    See [Handle overlapping Image Maps](creating-image-maps.md#handling_overlapping_image_maps).

* **Copying Image Maps to other pages** - Select **[!UICONTROL Copy Maps To]** (make sure you are on the Map Pages tab). On the Select Images screen, select the page or pages where you want to copy the Image Maps, and select **[!UICONTROL Select]**.

    See [Copy Image Maps to other images](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Besides copying Image Maps to different pages in an eCatalog, you can copy all the Image Maps in an eCatalog to a different eCatalog. See [Copy Image Maps between eCatalogs](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Review and import Image Map data {#reviewing-and-importing-image-map-data}

The Map Summary screen provides metadata about your eCatalog. You can also batch-import Image Map data for your eCatalog starting on the Map Summary screen. Importing Image Map data this way makes it easier to enter Image Map URLs and rollover text.

To see the Map Summary screen, on the Map Pages tab of the eCatalog screen, select **[!UICONTROL Summary]**.

### Review Image Map data summary {#review-image-map-data-summary}

1. On the Map Pages screen, select **[!UICONTROL Summary]**.

   The Map Summary screen displays how many Image Maps, URLs, rollover text descriptions, and other actions are in your eCatalog. 

1. If there are rollover key errors, select the error in the **[!UICONTROL Rollover_Key Error]** column to see what must change in your spreadsheet to correct the error. You can select and copy the text from this message and paste it into your spreadsheet.
1. Select **[!UICONTROL Preview]** so you can examine a page in the eCatalog Viewer; select the X to close the Summary screen and return to the Map Pages screen, or select **[!UICONTROL Close]** to return to Browse.

### Import Image Map data {#import-image-map-data}

Rather than enter Image Map data on each page, you can import the data for your entire eCatalog into the Map Summary screen. You import the Image Map data in the form of a tab-delimited file or XML DTD. The fields in your file must be in the order shown in the Map Summary screen: Name, TOC Labels, Maps, URLs, Rollover Text, Other Actions, and Search Strings. Importing Image Map data saves you the trouble of entering the data in the Image Map List as you create each Image Map.

>[!NOTE]
>
>Before importing Image Map data, you must have already created the Image Maps.

Starting on the Map Summary screen, follow these steps to import Image Map data for Image Maps you have created:

1. Select **[!UICONTROL Import Map Data]**.
1. In the Import Metadata dialog box, select **[!UICONTROL Browse]**, and then select the tab-delimited or XML DTD file.
1. In the Job Name field, type a name for the file (be careful to retain its extension).
1. Select **[!UICONTROL Upload]**.

## Copy Image Maps between eCatalogs {#copying-image-maps-between-ecatalogs}

You can copy all the Image Maps in an eCatalog to a different eCatalog. Copying Image Maps this way is a convenient method of copying Image Maps between foreign-language translations of the same eCatalog. For the copying to be successful, Dynamic Media Classic recommends copying between eCatalogs with the same number of pages and same images.

>[!NOTE]
>
>If the eCatalog to which you copy Image Maps already contains Image Maps, those Image Maps are deleted when the copy is made.

To copy all the Image Maps in one eCatalog to another eCatalog, do the following:

1. Select the eCatalog with the Image Maps you want to copy, and select the eCatalog’s rollover **[!UICONTROL Edit]** button.
1. On the Order Pages tab, select **[!UICONTROL Copy Maps]**.
1. In the Select Asset dialog box, select the eCatalog where you want to copy the Image Maps, and then select **[!UICONTROL Select]**.

Dynamic Media Classic displays a warning message if the target eCatalog (the eCatalog to which you copy Image Maps) has a different number of pages or images that are a different size. Select **[!UICONTROL Continue]** to copy the Image Maps despite the warning.
