---
title: Adding and managing Media Portal users
seo-title: Adding and managing Media Portal users
description: null
seo-description: Learn how to add and manage Media Portal users
uuid: e40f86a9-56de-48e3-b413-e8757dbc5767
contentOwner: admin
cq-gepid: scene7/using/WSef8d5860223939e226c748d312aabac1f5a-8000,scene7/using/WSef8d5860223939e252d11c5b12edf45786c-8000,scene7/using/WSef8d5860223939e2-7aa8671412aabadfa84-8000,scene7/using/WSb6fcde95647ddd9254e7cbca126676e8056-8000,scene7/using/WSb6fcde95647ddd9254e7cbca126676e8056-7fff,scene7/using/WSb6fcde95647ddd9254e7cbca126676e8056-7ffe,scene7/using/WSb6fcde95647ddd92-6b01d19712659abee1c-8000,scene7/using/WS56d35d2f221c8d0e550b9d62126b5177c73-8000,scene7/using/WSef8d5860223939e2-7834b07d12ac0dad496-8000
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 84f73b1d-2084-4b23-89da-72020ac776b0
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 42.006-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/media_portal;/content/help/en/experience-manager/morehelp/media_portal
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Adding and managing Media Portal users{#adding-and-managing-media-portal-users}

As an administrator, you can add and manage users, decide whether they can change passwords, edit user information, and upload user lists. These tasks are accomplished on the User Administration screen. To access this screen, click **Setup** &gt; **Application Setup** &gt; **Administration Setup** &gt; **User Administration**.

>[!NOTE]
>
>Before you add users, set up groups for administering them. Media Portal does not let you add a user without assigning the user to one or more groups. For more information, see [Creating and managing Media Portal groups](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Handling Media Portal passwords {#handling-media-portal-passwords}

Media Portal users, contributors, and contributor-users are sent a Welcome e-mail message with a password when you sign them up. Administrators can decide whether Media Portal users can change this password.

1. Click **Setup** &gt; **Media Portal Setup** &gt; **General Settings**.
1. On the General Settings page, select or deselect **Allow Media Portal user to change Password**. 
1. Click **Save**.

>[!NOTE]
>
>Media Portal users who are allowed to change passwords can do so by clicking **Setup** &gt; **Personal Setup** and changing passwords on the Personal Setup screen.

## Adding a Media Portal user {#adding-a-media-portal-user}

1. Click **Setup** &gt; **Application Setup** &gt; **Administration Setup** &gt; **User Administation**.
1. On the User Administration page, click **Add**.
1. In the Add User dialog box, in the User Info panel, enter the First Name, Last Name, and Email address of the user, and then click **Next**.
1. In the Company/Role panel, in the Companies drop-down list, select a company or companies for the user.
1. In the Role list, select a Media Portal role, and then click **Next**.

   See [Media Portal user roles](media-portal-user-roles.md#media_portal_user_roles).

1. In the Access Groups panel, select one or more groups.

   See [Creating and managing Media Portal groups](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Optional) Click **Email Settings** to choose e-mail settings different from the default settings.

   See [Set up the Welcome e-mail message for Media Portal users](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Click **Add User**.

After you add a user, Media Portal sends the user a Welcome e-mail message. The message includes a temporary password and the Media Portal URL.

## Uploading a Media Portal user list {#uploading-a-media-portal-user-list}

If you have numerous users to add, you can upload a user list. The users are added automatically to the currently selected account.

Create the user list as a CSV (comma-separated values) file containing the user information. After the list is uploaded, the users in the list are automatically added to the account with their specified group assignments. A Welcome e-mail is sent to each new user, including a link to Media Portal and a temporary password.

### Creating the CSV file {#creating-the-csv-file}

Create a CSV file (filename.csv) that conforms to the following format and fields. The first row of the file must contain the column headings listed in this table; you can order these columns as desired. All columns are required.

<table cellpadding="4" cellspacing="0"> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e9550" valign="top" width="NaN%"><p>Column name</p></th> 
   <th class="cellrowborder" id="d19e9553" valign="top" width="NaN%"><p>Description</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e9550 " valign="top" width="NaN%"><p>First Name</p></td> 
   <td class="cellrowborder" headers="d19e9553 " valign="top" width="NaN%"><p>The first name.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e9550 " valign="top" width="NaN%"><p>Last Name</p></td> 
   <td class="cellrowborder" headers="d19e9553 " valign="top" width="NaN%"><p>The last name.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e9550 " valign="top" width="NaN%"><p>Email</p></td> 
   <td class="cellrowborder" headers="d19e9553 " valign="top" width="NaN%"><p>A valid e-mail address.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e9550 " valign="top" width="NaN%"><p>Password</p></td> 
   <td class="cellrowborder" headers="d19e9553 " valign="top" width="NaN%"><p>A case-sensitive password string.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e9550 " valign="top" width="NaN%"><p>User Role</p></td> 
   <td class="cellrowborder" headers="d19e9553 " valign="top" width="NaN%"><p>MediaPortalAdmin</p><p>MediaPortalUser</p><p>MediaPortalContributor</p><p>MediaPortalContributorUser</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e9550 " valign="top" width="NaN%"><p>Groups</p></td> 
   <td class="cellrowborder" headers="d19e9553 " valign="top" width="NaN%"><p>List of one or more account group assignments for each user, separated by commas. You specify the group by prefixing the account name, separated by forward slash (/). For example, PortalCo/IT, where PortalCo is the account and IT is the group within the PortalCo account.</p></td> 
  </tr> 
 </tbody> 
</table>

The following sample spreadsheet demonstrates how to lay out a CSV file:

<table cellpadding="4" cellspacing="0"> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e9617" valign="top" width="NaN%"><p>First Name</p></th> 
   <th class="cellrowborder" id="d19e9620" valign="top" width="NaN%"><p>Last Name</p></th> 
   <th class="cellrowborder" id="d19e9623" valign="top" width="NaN%"><p>Email</p></th> 
   <th class="cellrowborder" id="d19e9626" valign="top" width="NaN%"><p>Password</p></th> 
   <th class="cellrowborder" id="d19e9629" valign="top" width="NaN%"><p>User Role</p></th> 
   <th class="cellrowborder" id="d19e9632" valign="top" width="NaN%"><p>Groups</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e9617 " valign="top" width="NaN%"><p>Peter</p></td> 
   <td class="cellrowborder" headers="d19e9620 " valign="top" width="NaN%"><p>Peterson</p></td> 
   <td class="cellrowborder" headers="d19e9623 " valign="top" width="NaN%"><p>petep@company.com</p></td> 
   <td class="cellrowborder" headers="d19e9626 " valign="top" width="NaN%"><p>welcome</p></td> 
   <td class="cellrowborder" headers="d19e9629 " valign="top" width="NaN%"><p>MediaPortalAdmin</p></td> 
   <td class="cellrowborder" headers="d19e9632 " valign="top" width="NaN%"><p>PortalCo/IT,PortalCo/Admin</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e9617 " valign="top" width="NaN%"><p>Kevin</p></td> 
   <td class="cellrowborder" headers="d19e9620 " valign="top" width="NaN%"><p>Marks</p></td> 
   <td class="cellrowborder" headers="d19e9623 " valign="top" width="NaN%"><p>kevinm@myco.com</p></td> 
   <td class="cellrowborder" headers="d19e9626 " valign="top" width="NaN%"><p>welcome</p></td> 
   <td class="cellrowborder" headers="d19e9629 " valign="top" width="NaN%"><p>MediaPortalUser</p></td> 
   <td class="cellrowborder" headers="d19e9632 " valign="top" width="NaN%"><p>PortalCo/MktgGroup, PortalCo/test</p></td> 
  </tr> 
 </tbody> 
</table>

### Uploading the CSV file {#uploading-the-csv-file}

1. Open the User Administration Setup screen.
1. Click **Upload User List**.
1. In the Select File to Upload dialog box, select the CSV file, and then click **Open**.

Each user in the list is automatically added to the groups specified. A Welcome e-mail message is sent to each.

>[!NOTE]
>
>If the CSV file was not formatted correctly, the following error message appears: “An error occurred while processing the uploaded CSV file. Check the file contents for valid data.” In addition, if the CSV contains an existing IP or IPS user, the user is not added to the User List.

## Generating a selectable list of Media Portal users {#generating-a-selectable-list-of-media-portal-users}

You can display the names and e-mail addresses of Media Portal users in a pop-up window. This list is useful if you want to cut and paste user names and addresses for use outside Media Portal.

1. Click **Setup** &gt; **Application Setup** &gt; **Administration Setup** &gt; **User Administration**.
1. In the **By User Role** drop-down list, choose the name of a Media Portal user role, and click **Refresh** to display the names of one class of Media Portal user.
1. Click **Popup List** to open the pop-up window. You can copy and paste this list.

## Setting up the Welcome e-mail message for Media Portal users {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

You can send a Welcome e-mail when you add new Media Portal users, contributors, and contributor-users. You can configure this e-mail message or tell Scene7 not to send it.

1. Choose **Setup** &gt; **Application Setup** &gt; **Administration Setup** &gt; **User Administration**.
1. In the User Administration Setup screen, click **Email Settings**.
1. In the Email Settings dialog box, specify any of the following settings:

   **Send Email** Deselect this option if you don’t want to inform new users by e-mail that you have signed them up.

   **Default Password** Enter a temporary password for new users, or leave the field empty to have Scene7 generate random passwords. Users are asked to change passwords the first time they log in.

   **Replacement URL** Enter a URL different from the default if your users access Scene7 through a different URL.

## Other user management tasks {#other-user-management-tasks}

Starting on the User Administration Setup screen, you can also do these tasks:

**Filter and sort the user list** Filter the list of Media Portal users to locate users. See Filter and sort the user list.

**Delete users** Delete a user from the list. See Delete a user.

**Activate and deactivate users** Suspend a user from accessing folders. See Activate and deactivate users.

**Edit user information** Enter up-to-date information about a user. See Edit user information.

**Create user-defined fields** Create custom, user-defined metadata fields to help organize assets in the Scene7 Publishing System. The fields can also be activated or deactivated, as necessary.

See [User-Defined Fields](application-setup.md#user_defined_fields).
