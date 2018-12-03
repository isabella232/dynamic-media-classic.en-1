---
title: Moving, renaming, and deleting assets
seo-title: Moving, renaming, and deleting assets
description: null
seo-description: Learn about how to move, rename, and delete assets.
uuid: 08a99a03-118d-4f90-ad72-982661ec9440
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WS259993e42159a215-1c6a66df1265272619e-7ff3,scene7/using/WS56d35d2f221c8d0e-4fedb9501266c5ace33-8000,scene7/using/WS259993e42159a215-1c6a66df1265272619e-7ff2,scene7/using/WS259993e42159a215-1c6a66df1265272619e-7ff1,scene7/using/WSef8d5860223939e24e8e560a128ad9e5593-8000
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: a9c9c138-7fb6-4e8e-b957-9062e604863e
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 43.717-0400
lr-lastmodifiedby: admin
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
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
    * To delete a folder, select the folder in the Asset Library, and click Remove Folder  ![](assets/DeleteFolder.png)    
    
      .

      Deleting a folder deletes the folder, all the assets in the folder, as well as all assets in its subfolders.

>[!NOTE]
>
>Scene7 recommends overwriting asset files rather than deleting them if your reason for deleting an asset file is to replace it with another by the same name.

## Delete multiple assets with a text file {#delete-multiple-assets-with-a-text-file}

To delete many assets at once throughout the Asset Library, you can list the assets you want to delete in a text file and submit the list to Scene7.

Create the list of Scene7 Publishing System IDs and save it as a text (.txt) file. Each Scene7 Publishing System ID must be on its own line (followed by a hard return).

After you create the list, follow these steps to use it to delete assets:

1. Choose File &gt; Delete Asset List.
1. In the Delete Asset list dialog box, browse or type the path to the text file with the list of assets you want to delete.
1. Click the Delete button.

When you delete assets with a text file, if any Scene7 Publishing System ID is not on the list, a message is displayed letting you know that Scene7 is “Unable to validate these entries in your list:” along with the list of entries. However, Scene7 will not generate an error on the Job screen.

>[!MORE_LIKE_THIS]
>
>* [Selecting assets in the Browse Panel](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Preparing your assets and folders for uploading](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Restoring assets from the Trash folder](trash-folder.md#restoring_assets_from_the_trash_folder)
