---
title: Creating and managing Media Portal groups
seo-title: Creating and managing Media Portal groups
description: null
seo-description: Learn how to create and manage Media Portal groups.
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98

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

    |Task|Read|Write|Delete|
    |--- |--- |--- |--- |
    |Browse folders and files|X|||
    |Edit files (crop, sharpen, adjust)||X||
    |Change filenames||X||
    |Move files to different folders||X||
    |Rename files||X||
    |Delete files|||X|

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

