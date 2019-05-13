---
title: Moving, renaming, and deleting assets
seo-title: Moving, renaming, and deleting assets
description: null
seo-description: Learn about how to move, rename, and delete assets.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683

---

# Moving, renaming, and deleting assets{#moving-renaming-and-deleting-assets}

You can move, rename, and delete assets from the Browse Panel. As well, you can delete many assets simultaneously with a text file.

## Move assets {#move-assets}

You can move assets to different folders in the Browse Panel.

1. Select the asset or assets in the Browse Panel, and do one of the following:

    * Display the folder you want to move the assets to in the Asset Library and drag the assets to the folder.
    * Choose File &gt; Move, select a folder in the Move Assets window, and select Move.

## Rename assets {#rename-assets}

To rename an asset:

1. Select the asset in the Browse Panel, and do one of the following:

    * Select the name, type in a new name, and press Enter or click away from the name.
    * Choose File &gt; Rename. The name of the asset is highlighted. Enter a new name and press Enter.

Be sure that you do not to enter the name of an existing Scene7 Publishing System asset.

## Delete assets {#delete-assets}

You can delete selected assets in the Browse Panel as well as delete entire folders. Deleted assets and folders are moved to the Trash folder, where they remain for seven days before being permanently deleted.

When you delete an asset, all assets derived from it are deleted as well. For example, deleting an image for which you created zoom targets deletes the zoom targets along with the image.

>[!NOTE]
>
>Zoom targets, image attributes, and history entries are permanently deleted when you delete the assets from which they derive. They are not moved along with the asset to the Trash folder; they cannot be restored from the Trash.

1. Do any of the following:

    * To delete one or more assets, select the assets in the Browse Panel, and press Delete or choose File &gt; Delete.
    * To delete a folder, select the folder in the Asset Library, and click **Remove Folder**.

      Deleting a folder deletes the folder, all the assets in the folder, as well as all assets in its subfolders.

>[!NOTE]
>
>Dynamic Media Classic recommends overwriting asset files rather than deleting them if your reason for deleting an asset file is to replace it with another by the same name.

## Delete multiple assets with a text file {#delete-multiple-assets-with-a-text-file}

To delete many assets at once throughout the Asset Library, you can list the assets you want to delete in a text file and submit the list to Dynamic Media Classic.

Create the list of Scene7 Publishing System IDs and save it as a text (.txt) file. Each Scene7 Publishing System ID must be on its own line (followed by a hard return).

After you create the list, follow these steps to use it to delete assets:

1. Choose File &gt; Delete Asset List.
1. In the Delete Asset list dialog box, browse or type the path to the text file with the list of assets you want to delete.
1. Click the Delete button.

When you delete assets with a text file, if any Scene7 Publishing System ID is not on the list, a message is displayed letting you know that Dynamic Media Classic is “Unable to validate these entries in your list:” along with the list of entries. However, Dynamic Media Classic will not generate an error on the Job screen.

>[!MORELIKETHIS]
>
>* [Selecting assets in the Browse Panel](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Preparing your assets and folders for uploading](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restoring assets from the Trash folder](trash-folder.md#restoring_assets_from_the_trash_folder)
