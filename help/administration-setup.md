---
title: Administration Setup
description: Learn how to setup the administration area of Dynamic Media Classic.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
feature: Dynamic Media Classic
role: Administrator
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
---
<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Administration Setup{#administration-setup}

The Administration Setup screens are for administering Dynamic Media Classic users. Use these screens to enable users to work in Dynamic Media Classic and to communicate by e-mail with users.

1. To access Administration Setup options, click **Setup** > **Personal Setup** > **Administration Setup**.

## User Administration {#user-administration}

All Dynamic Media Classic users are assigned a role that determines their privileges and access rights to features in Dynamic Media Classic. Administrators determine the different roles and responsibilities for the companies to which they are assigned.

Typically, Dynamic Media Classic configures the first set of companies and assigns a company administrator. The company administrator then sets up and administers Dynamic Media Classic users.

Dynamic Media Classic supports several user roles. These roles can access companies set up for the Dynamic Media Classic:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic User** Can access companies to which they have been assigned; cannot perform any administrative duties.

**Adobe Dynamic Media Classic Company Admin** Can view and administer only their own companies. A Company Administrator can also perform all administration functions, including adding administrators and users. A Company Administrator can add a user to the DMC company admin accounts. (This role is the default user role.)

After you add a user, Dynamic Media Classic sends the user a Welcome e-mail message. The message includes a password and the Dynamic Media Classic URL.

### Adding a user or administrator {#adding-a-user-or-administrator}

1. Click Setup > Application Setup > Administration Setup >User Administration.
1. Click Add.
1. Enter the name and email address of the user or administrator that you want to add, then click Next.

   >[!NOTE]
   >
   >The apostrophe character (‘) is not allowed in email addresses.

1. Choose a Role option to assign a role to the user.

   See [Dynamic Media Classic user roles and privileges](administration-setup.md#user_administration).

1. Select a company name to add a user to a company.
1. If you want to add the user to a group (if you are adding a Media Portal user or contributor), click Next and add the user.
1. Click Save to complete the user setup.

   After saving, a prompt asks if you want to add a user to another company. Click Add if you want to add the user to a company.

   All new users are given a randomly generated password; users are required to change passwords the first time they sign in to the Dynamic Media Classic desktop application.

   New users are sent a Welcome e-mail after you add them. The e-mail provides a temporary password and explains how to sign in to Dynamic Media Classic.

   If the user does not receive the welcome email, have them go the Dynamic Media Classic sign in page (https://s7sps1.scene7.com), and click Forgot My Password. The password is reset and a new email is sent. If the user does not receive the email and it is not in their Junk folder, contact Technical Support.

   When adding new Media Portal users, you can also go to Setup > Application Setup > User Administration, then click Upload User List and select a .csv file containing no more than 500 users.

### Deleting a user {#deleting-a-user}

You can delete users from Dynamic Media Classic by making them invalid. Invalid users are removed from the system and all accounts.

1. Click **Setup** > **Application Setup** > **Administration Setup** > **User Administration**.
1. Select a user from the list, and then click **Edit**.
1. Deselect Valid.
1. Click **Save**.

### Activating or deactivating users {#activating-or-deactivating-users}

Users who have been deactivated no longer have permission to enter the account listed at the top of the Select Accounts To Access menu.

1. Click **Setup** > **Application Setup** > **Administration Setup** > **User Administration**.
1. In the user list, select or deselect the Active option next to the name of the user.

### Editing user information {#editing-user-information}

The user information that you can edit depends on your role as an administrator and the assigned role of the user whose information you want to edit. Options that are dimmed (unavailable) are not editable.

1. Go to **Setup** > **Application Setup** > **Administration Setup** > **User Administration**.
1. Select the user and click **Edit**.
1. Select the entry in the table that shows the company you are trying to modify permissions or access for, then click the Manage Company link.
1. Select the user role.
1. If you want to change the user’s group membership (if you are editing or adding a Media Portal user or contributor), click Next and edit the group membership.
1. Click **Save**.

### Filtering and sorting the user list {#filtering-and-sorting-the-user-list}

You can filter and sort the user list to locate users. All users in all accounts you administer appear in the Users list, regardless of the account selected in the Select Account To Access menu.

You can use the following user list filtering techniques:

* **Filter by group** - Select the By Group menu and choose an option to narrow the list to users in a group.

* **Filter by user role** - Select the By User Role menu and choose an option to narrow the list to users or administrators of different types.

* **Filter by field name** - Select the Enable Filter By Field option. Then select the By Field Name menu, choose a column for filtering the list, and select the Filter Character menu and choose a letter. The list is filtered on one of the columns by the letter you chose. Deselect the Enable Filter By Field option to see the full list.

* **Filter out invalid users** - Deselect the Include Invalid option. The search results display only users who are in the system. Invalid users have been deleted from the system and the accounts you administer.

* **Sort by column heading** - Click a heading to sort all users by their status, alphabetically by first name, last name, or email, by user role, or by valid/invalid status.

If you have many users, you can limit the size of the list by selecting the Max List Size menu and choosing a number.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to a Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to a Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Click **Manage Organizations**.
1. Click **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Click **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, click **Solutions** > **Experience Manager**. Under the Dynamic Media Classic card, click **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Bandwidth & Storage {#bandwidth-storage}

Dynamic Media Classic Administrators can generate bandwidth, storage, and other types of reports for the companies they administer. These reports are available on the Bandwidth & Storage screen.

To open this screen, click Setup > Personal Setup. Expand Administration Setup, and then click Bandwidth & Storage.

### Types of reports {#types-of-reports}

The following table describes reports that you can generate from the Bandwidth & Storage screen:

|Report|Information|Use|
|:--- |:--- |:--- |
|Bandwidth|Bandwidth use by company|Track bandwidth usage by company over specific date ranges to determine traffic patterns.|
|Storage|Storage usage|Track the amount of data uploaded by company.|
|Image Content|The number of image requests by type|Track the number of requests and volume for different image types.|
|Domain|The number of URL requests by domain|Track image usage based on the domain of the image request for a specific company. (Dynamic Media Classic can provide more than one domain per account. For more information, contact Technical Support.)|
|Video Streaming|Bandwidth usage for streaming video|Track streaming video usage by company over specific date ranges to determine traffic patterns.|
|Video Content|Playing time of different videos|Determine which are the most viewed and least viewed videos.|

The Image Content report provides information about requests for the following image types:

* **Image Request** - Requests for images.

* **Thumbnail Request** - Requests for swatch or alternate images in viewers.

* **Mask Request** - Requests to images returning gray-scale masks.

* **Viewer Tile Request** - Image requests loaded by a viewer.

* **Vnt Object Request** - Image rendering requests that return an image with specified objects in the requested vignettes.

* **Vnt Info Request** - Image rendering requests that return information concerning the requested vignettes.

>[!NOTE]
>
>The Video Streaming report applies to streaming videos only. It doesn’t track the viewing of progressive videos.

### Generating a report {#generating-a-report}

To generate a bandwidth, storage, image content, domain, video streaming, or video content report:

1. Choose Setup > Personal Setup.
1. Expand Administration Setup, and then click Bandwidth & Storage.
1. Click a tab: Bandwidth, Storage, Image Content, Domain, Video Streaming, or Video Content.

   See [Types of reports](administration-setup.md#types_of_reports).

### Viewing data in different ways {#viewing-data-in-different-ways}

After you generate a report on the Bandwidth & Storage page, you can choose options for viewing information. You can choose how information is presented, view information in a chart or data grid, and specify a time period for capturing information. In Data view, you can also sort information and rearrange columns.

* **Viewing data in a chart or data grid** - Click the Chart View option to view data in a chart; click the Data View option to view data in a data grid.

* **Choosing a report presentation type** - On the Report Type menu, choose Summary, Daily, or monthly to organize data in summary form, by day, or by month. Not all reports provide this option.

* **Specifying a time period** - Choose options to define a time period for your report, and then click Update after you define a time period:

* **Pre-defined time period** - On the Pre-defined Report menu, choose an option. For example, choose Last Month to capture data from the previous month.

* **Custom time period** - On the Pre-defined Report menu, choose Custom. Then choose a date on the Start Month (or Start Date) menu and a date on the # of Months (or # or Days) menu. For Domain and Video Content Reports, you can choose a specific start and end date for capturing report information.

* **Sorting data (Data view only)** - To sort information on a column, click the column’s heading. Click again to sort in descending order.

* **Rearranging columns (Data view only)** - To move a column to a different location on the data grid, drag its heading.

### Exporting and printing reports {#exporting-and-printing-reports}

After you generate a report, you can export its data for use in spreadsheets and other applications. You can also print reports.

* **Exporting report data** - In Data view, sort, and arrange the data as necessary. Then open the Export menu and choose a format: Tab Delimited, Comma Separated, or HTML Formatted. The data is copied to the Clipboard in the format you chose. You can now paste the data into a spreadsheet or application.

* **Printing a report** - Click **[!UICONTROL Print]**, choose the options you want in the Print dialog box, and then click **[!UICONTROL OK]**.

## Image Errors {#image-errors}

Dynamic Media Classic Administrators can generate Image Error reports. An Image Error report provides a list of the 20 most frequent image errors, for the past 24 hours, for the company you are currently logged in to. Follow these steps to generate an Image Error report:

1. Click Setup > Personal Setup.
1. Expand Administration Setup, and then click Image Errors.
1. (Optional) Do any of the following:

    * Click a heading to sort errors by the heading information. By default, errors are sorted by number of occurrences, highest to lowest.
    * Move the cursor over the Response field for an error to see the specific error message.
    * Move the cursor over the URL field or the Referrer field to see the link to the image or referrer web page.
    * Click **[!UICONTROL URL Copy URL]** to copy the link to the actual image. You can paste this link in a browser window to go to the image and investigate the error.
    * Click **[!UICONTROL Referrer Copy URL]** to copy the link to the referrer web page.

Errors displayed are for the company you are currently logged in to. Each error includes the following information:

* **Image ID** - ID for the offending image.

* **Time** - The time range of the first time the error was reported to the last time the error was reported, within the last 24 hours.

* **Count** - The number of errors reported on the image.

* **Response** - The specific error message. Errors are either 4xx or 5xx.

* **URLs** - Lists the URL to the image on Dynamic Media Classic.

* **Referrer** - Specifies the URL for the web site where the initial request came from. The referrer can be any web site that has a link to the image.

The URL and Referrer columns have Copy URL associated with them to simplify testing.
