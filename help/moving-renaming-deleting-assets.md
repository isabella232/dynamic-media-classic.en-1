---
title: Move, rename, and delete assets
description: Learn about how to move, rename, and delete assets in Adobe Dynamic Media Classic.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
---
# Move, rename, and delete assets{#moving-renaming-and-deleting-assets}

You can move, rename, and delete assets from the Browse Panel. As well, you can delete many assets simultaneously with a text file.

## Move assets {#move-assets}

You can move assets to different folders in the Browse Panel.

1. Select the asset or assets in the Browse Panel, and do one of the following:

    * Display the folder you want to move the assets to in the Asset Library and drag the assets to the folder.
    * Go to **[!UICONTROL File]** > **[!UICONTROL Move]**, select a folder in the Move Assets window, and select **[!UICONTROL Move]**.

## Rename assets {#rename-assets}

1. Select the asset in the Browse Panel, and do one of the following:

    * Select the name, type in a new name, and press **[!UICONTROL Enter]** or select away from the name.
    * Go to **[!UICONTROL File]** > **[!UICONTROL Rename]**. The name of the asset is highlighted. Enter a new name and press **[!UICONTROL Enter]**.

Be sure that you do not to enter the name of an existing Adobe Dynamic Media Classic asset.

## Delete assets {#delete-assets}

You can delete selected assets in the Browse Panel and delete entire folders. Deleted assets and folders are moved to the Trash folder, where they remain for seven days before being permanently deleted.

When you delete an asset, all assets derived from it are deleted as well. For example, deleting an image for which you created zoom targets deletes the zoom targets along with the image.

>[!NOTE]
>
>Zoom targets, image attributes, and history entries are permanently deleted when you delete the assets from which they derive. They are not moved along with the asset to the Trash folder; they cannot be restored from the Trash.

1. Do any of the following:

    * To delete one or more assets, select the assets in the Browse Panel, and press **[!UICONTROL Delete]** or go to **[!UICONTROL File]** > **[!UICONTROL Delete]**.
    * To delete a folder, select the folder in the Asset Library, and select **[!UICONTROL Remove Folder]**.

      Deleting a folder deletes the folder, all the assets in the folder, and all assets in its subfolders.

>[!NOTE]
>
>Adobe Dynamic Media Classic recommends overwriting asset files rather than deleting them if your reason for deleting an asset file is to replace it with another by the same name.

## Delete multiple assets with a text file {#delete-multiple-assets-with-a-text-file}

To delete many assets at once throughout the Asset Library, you can list the assets you want to delete in a text file and submit the list to Adobe Dynamic Media Classic.

Create the list of Adobe Dynamic Media Classic IDs and save it as a text (.txt) file. Each Adobe Dynamic Media Classic ID must be on its own line (followed by a hard return).

After you create the list, follow these steps to use it to delete assets:

1. Go to **[!UICONTROL File]** > **[!UICONTROL Delete Asset List]**.
1. In the Delete Asset list dialog box, browse, or type the path to the text file with the list of assets you want to delete.
1. Select **[!UICONTROL Delete]**.

When you delete assets with a text file, if any Adobe Dynamic Media Classic ID is not on the list, the message “Unable to validate these entries in your list:” is displayed and the list of entries. However, Adobe Dynamic Media Classic does not generate an error on the Job page.

>[!MORELIKETHIS]
>
>* [Select assets in the Browse Panel](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Prepare your assets and folders for uploading](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restore assets from the Trash folder](trash-folder.md#restoring_assets_from_the_trash_folder)
