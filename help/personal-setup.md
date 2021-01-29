---
title: Personal Setup
description: All users can change settings on the Personal Setup screen of Dynamic Media Classic.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c

---

# Personal Setup {#personal-setup}

All users can change settings on the Personal Setup screen. To open the Personal Setup screen, click Setup > Personal Setup.

>[!NOTE]
>
>The Personal Setup screen lists which user role you have in Dynamic Media Classic: Company Administrator, Administrator, or User.

The Personal Setup settings control the default behavior of the Browse Panel, how you receive e-mail, and password settings. Remember to click Save after you change these settings.

## My Account Information

Identifies your account name, name, user name (e-mail address), and assigned user role.

### Desktop Version

Click Install Now to install the desktop version of Dynamic Media Classic on your local hard drive. Or, click Reinstall Now to install the desktop version again.

## To install the plug-in on your local hard drive

1. On the Personal Setup page in Dynamic Media Classic, under Illustrator Plug-in for Web-to-Print, click **Download Now** to download the **Illustrator Plug-in for Web-to-Print.zip** file. 
1. Uncompress the ZIP file to a temporary folder.

   A readme file is included at the root of the unzipped file to provide you with additional information about the plug-in.

1. Depending on your installed operating system, do one of the following:

### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li>Click libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, click flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014 > mac64.</li><li>Click libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-click on the Adobe illustrator CC 2014 icon and click Show Package Contents from context menu).</li><li>Return to the same libraries folder, click `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator.

### Browser

* **Thumbnail Size**
  * Determines the default size of thumbnail images in Grid view in the Browse Panel.
* **Default Asset Library View**
  * Determines whether the assets in the Asset Library for build sets appear as thumbnails or by name. If you are working with large quantities of assets in the Asset Library, you can view the assets by name. For example, if you are building a large eCatalog with many PDF files, you can view the assets by name to make the list shorter.
* **Default Browse Sort Order**
  * Determines the order in which assets appear by default in the Browse Panel. Choose a sort criterion on the menu and whether you want an ascending or descending sort.
* **Default Browse Location**
  * Lets you set the browse location to the default, the last folder browsed, or to a specific location that you navigate to and identify. You can also set the browse location to sort the files and folders in ascending or descending order.
* **Default Browse View** 
  * Determines whether Grid view or List view is the default view you see when you first open the Browse Panel.
* **Splash Screen Display**
  * Determines whether you see any splash screens, including the Welcome splash screen.
* **Show ToolTips**
  * Determines whether tool tips appear when you move the pointer over buttons, menus, and navigation links. Tool tips describe on-screen items.
* **Checkerboard Background**
  * Displays a checkerboard layer behind images, letting you easily see the transparent areas of an image that has an alpha channel.
* **Show File Size**
  * Displays the file size of an asset when you are browsing.
* **Include UDFs in Search**
  * Deselected (default) to improve system performance for most metadata searches that you run.

If most of your metadata searches benefit from including user-defined fields, you can select this option to turn it on. As an alternative, use Advanced Search to give you a more directed and faster search experience than including user-defined fields.

See [Conducting an advanced search](searching-assets.md#conducting_an_advanced_search).

See also [User-Defined Fields](application-setup.md#user_defined_fields).

* **Basic Search Type**
  * Choose a default search type, Contains or Starts With.
* **Show Media Portal Features**
  * Select this option to access Media Portal features, such as Media Cart.
* **Show Command Feedback**
  * Show command requests to the server.
* **Show Dialog During Export**
  * Displays a dialog box when you perform an export. If you deselect this option, you can still go to the Jobs page to retrieve the results of your export.

## Email

* **Email Options**
  * Choose how you want Dynamic Media Classic to inform you by e-mail when upload and publish jobs are completed. You can receive job completion notices only if warnings or errors occurred.
* **Email Scope**
  * Determines whether you receive all job e-mail for your company or only e-mail about upload and publish jobs you initiate.
* **Email Types**
  * Determines whether you are informed when upload jobs and publish jobs are completed.
* **Language**
* **Preferred Language**
  * Determines the language for the interface.
* **Password**
* **New Password**
  * Enter a new, valid password. Your password must meet the following requirements:
    * Be between 8-25 characters long
    * Contain at least one lowercase letter
    * Contain at least one uppercase letter
    * Contain at least one number
    * Contain at least one of the following special characters: #$&-_:{}
* **Re-Type Password**
  * Re-enter the new password to confirm that you are entering it correctly.
* **Password Expiration**
  * Determines whether your password expires after 72 days as a security measure. If you select Yes, you are asked to create a new password after 72 days.
