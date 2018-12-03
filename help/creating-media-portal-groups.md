---
title: Creating and managing Media Portal groups
seo-title: Creating and managing Media Portal groups
description: null
seo-description: Learn how to create and manage Media Portal groups.
uuid: d7b7e80b-5876-4c03-9ce2-74be4d98f5fa
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WSb6fcde95647ddd92-d5fb6c21265839fcb3-7ff1,scene7/using/WSb6fcde95647ddd92-d5fb6c21265839fcb3-7ff0,scene7/using/WSb6fcde95647ddd92-d5fb6c21265839fcb3-7fef,scene7/using/WSb6fcde95647ddd92-d5fb6c21265839fcb3-7fee,scene7/using/WSef8d5860223939e2-557af6f112e791b6a73-8000,scene7/using/WSb6fcde95647ddd92-d5fb6c21265839fcb3-7fed
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: c545512d-4c8b-4d5e-a8a6-d8e9c5acb4bc
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 42.771-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/media_portal;/content/help/en/experience-manager/morehelp/media_portal
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Creating and managing Media Portal groups{#creating-and-managing-media-portal-groups}

*Groups* are designed to help you administer Media Portal users. To access an asset, a user must be a member of at least one group that has permission to access that asset. When you add a user, you assign the user to one or more groups. In so doing, you grant the user access to folders to which the group has been assigned. You can also choose which Image Presets are available to a group.

## Using groups to restrict access to folders, assets, and Image Presets {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

To grant access permission at different levels, you create groups. For each group, you assign read, write, and delete permissions to different folders and assets in folders. As well, you decide which Image Presets are available to the group. You then assign users to groups. A user can be a member of more than one group. The group concept gives you the flexibility to assign access to limited sets of the total content.

If you don’t specifically grant a group permission to an asset or folder, that asset or folder inherits the permissions you assigned to its parent folder (the folder above it in the folder hierarchy). Grant permissions to a parent folder if you want to make sure that all its child folders inherit the same permissions.

>[!NOTE]
>
>Users can belong to more than one group. When a user belongs to two groups with different access permissions to a folder, the user is granted the highest access.

## Adding a group {#adding-a-group}

1. Click **Setup** &gt; **Media Portal Setup** &gt; **Groups**.
1. Click **Add**. 
1. In the Add Group dialog box, enter a name for the group in the Group Name box, and then click **Add Group**.
1. If you want, you can select the boxes next to the names of users to add users to the new group.
1. If you want to specify access permissions at this time, click the **Asset Access Permissions** tab, and then specify the options you want.

   See [Establish asset access permissions for a group](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. If you want to choose which Image Presets are available to the group, click the **Image Preset Access Permissions** tab, and select Image Presets that the group can use.

   See [Choose Image Preset access permissions for a group](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Click **Close**.

## Establishing asset access permissions for a group {#establishing-asset-access-permissions-for-a-group}

1. Click **Setup** &gt; **Media Portal Setup** &gt; **Groups**.
1. On the Groups list page, do one of the following:

    * To add a group and specify permissions, click **Add**. In the Add Group dialog box, enter a name for the group, click **Add Group**, and add users to the group.
    * To edit a group’s permissions, select the group, and then click **Edit**.

1. In the Add Group or Edit group dialog box, click the **Asset Access Permissions** tab. The right side of the tab offers boxes for establishing read, write, and delete permissions for folders and assets. You can expand and collapse folders and subfolders in the left pane.
1. To assign rights to folders or individual assets, select the folder in the left pane. The folder contents appear in the right pane. Then assign rights for the group by selecting the boxes for the corresponding files or folders in the right pane.

   This table maps different tasks to read, write, and delete permissions.

<table cellpadding="4" cellspacing="0"> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e9191" valign="top" width="NaN%"><p>Task</p></th> 
   <th class="cellrowborder" id="d19e9194" valign="top" width="NaN%"><p>Read</p></th> 
   <th class="cellrowborder" id="d19e9197" valign="top" width="NaN%"><p>Write</p></th> 
   <th class="cellrowborder" id="d19e9200" valign="top" width="NaN%"><p>Delete</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e9191 " valign="top" width="NaN%"><p>Browse folders and files</p></td> 
   <td class="cellrowborder" headers="d19e9194 " valign="top" width="NaN%"><p><strong>X</strong></p></td> 
   <td class="cellrowborder" headers="d19e9197 " valign="top" width="NaN%"><p></p></td> 
   <td class="cellrowborder" headers="d19e9200 " valign="top" width="NaN%"><p></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e9191 " valign="top" width="NaN%"><p>Edit files (crop, sharpen, adjust)</p></td> 
   <td class="cellrowborder" headers="d19e9194 " valign="top" width="NaN%"><p></p></td> 
   <td class="cellrowborder" headers="d19e9197 " valign="top" width="NaN%"><p><strong>X</strong></p></td> 
   <td class="cellrowborder" headers="d19e9200 " valign="top" width="NaN%"><p></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e9191 " valign="top" width="NaN%"><p>Change filenames</p></td> 
   <td class="cellrowborder" headers="d19e9194 " valign="top" width="NaN%"><p></p></td> 
   <td class="cellrowborder" headers="d19e9197 " valign="top" width="NaN%"><p><strong>X</strong></p></td> 
   <td class="cellrowborder" headers="d19e9200 " valign="top" width="NaN%"><p></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e9191 " valign="top" width="NaN%"><p>Move files to different folders</p></td> 
   <td class="cellrowborder" headers="d19e9194 " valign="top" width="NaN%"><p></p></td> 
   <td class="cellrowborder" headers="d19e9197 " valign="top" width="NaN%"><p><strong>X</strong></p></td> 
   <td class="cellrowborder" headers="d19e9200 " valign="top" width="NaN%"><p></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e9191 " valign="top" width="NaN%"><p>Rename files</p></td> 
   <td class="cellrowborder" headers="d19e9194 " valign="top" width="NaN%"><p></p></td> 
   <td class="cellrowborder" headers="d19e9197 " valign="top" width="NaN%"><p><strong>X</strong></p></td> 
   <td class="cellrowborder" headers="d19e9200 " valign="top" width="NaN%"><p></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e9191 " valign="top" width="NaN%"><p>Delete files</p></td> 
   <td class="cellrowborder" headers="d19e9194 " valign="top" width="NaN%"><p></p></td> 
   <td class="cellrowborder" headers="d19e9197 " valign="top" width="NaN%"><p></p></td> 
   <td class="cellrowborder" headers="d19e9200 " valign="top" width="NaN%"><p><strong>X</strong></p></td> 
  </tr> 
 </tbody> 
</table>

1. Click **Close**.

>[!NOTE]
>
>Access rights are established when you select a box. When you assign rights to a folder, its subfolders and all files within it are given the same rights as the parent folder. However, you can specify different rights for individual subfolders and asset files.

## Choosing Image Preset access permissions for a group {#choosing-image-preset-access-permissions-for-a-group}

Choose Image Preset access permissions for a group if you want to specify which Image Presets are available to group members when they export assets with Media Portal.

See also [Specifying export options available to Media Portal users](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

1. Click **Setup** &gt; **Media Portal Setup** &gt; **Groups**.
1. On the Groups list page, do one of the following:

    * To add a group and specify which Image Presets are available to it, click **Add**. In the Add Group dialog box, enter a name for the group, click **Add Group**, and add users to the group.
    * To edit a group’s Image Preset options, select the group, and then click **Edit**.

1. In the Add Group or Edit group dialog box, click the **Image Preset Access Permissions** tab. 
1. Select or deselect Image Presets to specify which presets are available to Media Portal users when they export assets.
1. Click **Close**.

## Edit and delete groups {#edit-and-delete-groups}

1. Click **Setup** &gt; **Media Portal Setup** &gt; **Groups**.
1. On the Group List page, select a group and edit or delete it.

   **Editing a group** Click Edit, and then choose options in the Edit Group dialog box.

   **Deleting a group** Click Delete.

