---
title: Personal Setup
description: All users can change settings on the Personal Setup screen of Adobe Dynamic Media Classic.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
---
# Personal Setup {#personal-setup}

All users can change settings on the Personal Setup screen. To open the Personal Setup screen, go to **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.

>[!NOTE]
>
>The Personal Setup screen lists which user role you have in Adobe Dynamic Media Classic: Company Administrator, Administrator, or User.

The Personal Setup settings control the default behavior of the Browse Panel, how you receive e-mail, and password settings. Remember to select **[!UICONTROL Save]** after you change these settings.

## My Account Information

Identifies your account name, name, user name (e-mail address), and assigned user role.

## Desktop

* **Clear Image Cache** - Removes all Adobe Dynamic Media cached image files from your computer.
* **Clear Asset Cache** - Removes all Adobe Dynamic Media caches asset files from your computer.

Besides clearing the image and asset cache using the desktop app, you can manually clear the cache directly from the file system. Based on your operating system, navigate to the following:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**To install Adobe Dynamic Media Creative Suite Extension:**

1. In Adobe Dynamic Media Classic, on the toolbar, go to **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**, under Creative Suite Extension, select **[!UICONTROL Download Now]** to download the `s7csxs.zxp` file. 
1. Select the **[!UICONTROL Installation]** and **[!UICONTROL System Requirements]** links for additional information about the extension.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li>Select libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, select flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Browser

* **[!UICONTROL Thumbnail Size]** - Determines the default size of thumbnail images in Grid View in the Browse Panel.
* **[!UICONTROL Default Asset Library View]** - Determines whether the assets in the Asset Library for build sets appear as thumbnails or by name. If you are working with large quantities of assets in the Asset Library, you can view the assets by name. For example, if you are building a large eCatalog with many PDF files, you can view the assets by name to make the list shorter.
* **[!UICONTROL Default Browse Sort Order]** - Determines the order in which assets appear by default in the Browse Panel. Choose a sort criterion on the menu and whether you want an ascending or descending sort.
* **[!UICONTROL Default Browse Location]** - Lets you set the browse location to the default, the last folder browsed, or to a specific location that you navigate to and identify. You can also set the browse location to sort the files and folders in ascending or descending order.
* **[!UICONTROL Default Browse View]** - Determines whether Grid View or List View is the default view you see when you first open the Browse panel.
* **[!UICONTROL Splash Screen Display]** - Determines whether you see any splash screens, including the Welcome splash screen.
* **[!UICONTROL Show ToolTips]** - Determines whether tooltips appear when you move the pointer over buttons, menus, and navigation links. Tooltips describe on-screen user interface items.
* **[!UICONTROL Checkerboard Background]** - Displays a checkerboard layer behind images, letting you easily see the transparent areas of an image that has an alpha channel.
* **[!UICONTROL Show File Size]** - Displays the file size of an asset when you are browsing.
* **[!UICONTROL Include UDFs in Search]** - To improve system performance for most metadata searches that you run, deselected (default).

  If most of your metadata searches benefit from including user-defined fields, you can select this option to turn it on. As an alternative, use Advanced Search to give you a more directed and faster search experience than including user-defined fields.

  See [Conducting an advanced search](searching-assets.md#conducting_an_advanced_search).

  See also [User-Defined Fields](application-setup.md#user_defined_fields).

* **[!UICONTROL Basic Search Type]** - You can select from two options: **[!UICONTROL Contains]** searches the full string for the specified value; **[!UICONTROL StartsWith]** searches from the beginning of the string and returns results faster than **[!UICONTROL Contains]**. Either option overrides the default that is set in **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Application General Settings]** by the Administrator.
* **[!UICONTROL Show Command Feedback]** - Select to turn the display of command requests to the server on; deselect to turn off.
* **[!UICONTROL Show Dialog During Export]** - Select to show a pop-up dialog box during an export. If you deselect (turn off) this option, you can still go to the Jobs page to retrieve the results of your export.

## Email

* **[!UICONTROL Email Options]** - Choose how you want Adobe Dynamic Media Classic to inform you by e-mail when upload and publish jobs are completed. You can receive job completion notices only if warnings or errors occurred.
* **[!UICONTROL Email Scope]** - Determines whether you receive all job e-mail for your company or only e-mail about upload and publish jobs you initiate.
* **[!UICONTROL Email Types]** - Determines whether you are informed when upload jobs and publish jobs are completed.

## Language

* **[!UICONTROL Preferred Language]** - Determines the language you want to use for the interface.

## Password

* **[!UICONTROL Current Password]** - Enter the password your present password.
* **[!UICONTROL New Password]** - Enter a new, valid password. Your password must meet the following requirements:
  * Be between 8-25 characters long.
  * Contain at least one lowercase letter.
  * Contain at least one uppercase letter.
  * Contain at least one number.
  * Contain at least one of the following special characters: `# $ & - _ : { }`
* **[!UICONTROL Re-Type Password]** - Reenter the new password to confirm that you are entering it correctly.
* **[!UICONTROL Password Expiration]** - Determines whether your password expires after 72 days as a security measure. If you select Yes, you are asked to create a password after 72 days.
