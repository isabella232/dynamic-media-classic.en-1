---
title: Personal Setup
seo-title: Personal Setup
description: null
seo-description: All users can change settings on the Personal Setup screen of Dynamic Media Classic.
uuid: 875634db-001a-409f-9359-a7106d9a97d5
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WSCAAE9C8A-F172-43a8-B134-6163E7C80218
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: b25969ad-9778-4293-8d0a-5d283624453b
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 43.881-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/setup;/content/help/en/experience-manager/morehelp/setup
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Personal Setup{#personal-setup}

All users can change settings on the Personal Setup screen. To open the Personal Setup screen, click Setup &gt; Personal Setup.

>[!NOTE]
>
>The Personal Setup screen lists which user role you have in the Scene7 Publishing System: Company Administrator, Administrator, or User.

The Personal Setup settings control the default behavior of the Browse Panel, how you receive e-mail, and password settings. Remember to click Save after you change these settings.

**My Account Information**

Identifies your account name, name, user name (e-mail address), and assigned user role.

**Desktop Version**

Click Install Now to install the desktop version of Scene7 Publishing System on your local hard drive. Or, click Reinstall Now to install the desktop version again.

**Illustator Plug-in for Web-to-Print**

On computers running Windows 7 or 8, you must have administrator privileges and log on as an administrator in Windows to install the Adobe Illustrator Plug-in for Web-to-Print. After you install the plug-in, it is available in Adobe Illustrator.

The plug-in is supported for the following Adobe Illustrator versions:

* Adobe Illustrator 18 in Adobe Creative Cloud 2014.
* Adobe Illustrator 17 in Adobe Creative Cloud.
* Adobe Illustrator 16 in Adobe Creative Suite 6.

Supported Adobe Illustrator platforms include the following:

* Apple Mac OS X 10.7 or greater.
* Windows 8, 32-bit and 64-bit.
* Windows 7, 32-bit and 64-bit.
* Windows XP, 32-bit and 64-bit (for Adobe Illustrator 16 in Adobe Creative Suite 6 only).

See also [Template Publishing](/#template_publishing).

**To install the plug-in on your local hard drive**

1. On the Personal Setup page in Scene7 Publishing System, under Illustrator Plug-in for Web-to-Print, click **Download Now** to download the **Illustrator Plug-in for Web-to-Print.zip** file. 
1. Uncompress the ZIP file to a temporary folder.

   A readme file is included at the root of the unzipped file to provide you with additional information about the plug-in.

1. Depending on your installed operating system, do one of the following:

    * **Windows**

    <table border="1" cellpadding="4" cellspacing="0" frame="border" id="WSac64270ea1b22722-107e390916129c79406-7fee" rules="all" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e1563" valign="top" width="NaN%"><p>If you are running</p></th> 
   <th class="cellrowborder" id="d19e1566" valign="top" width="NaN%"><p>Do this</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e1563 " valign="top" width="NaN%"><p>Adobe Illustrator 18 in Adobe Creative Cloud 2014</p></td> 
   <td class="cellrowborder" headers="d19e1566 " valign="top" width="NaN%"> 
    <ol> 
     <li><p>From the root of the unzipped folder, click <strong>CC-2014</strong>.</p></li> 
     <li><p>Depending on the bit version of Adobe Illustrator that you are using, click <strong>win32</strong> or <strong>win64</strong>.</p></li> 
     <li><p>Click <strong>libraries</strong> &amp;gt; <strong>flame</strong>, and then copy <i>aflame.dll</i> to Adobe Illustrator's executable folder. For example, <span class="kbd">C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows</span>.</p><p><i><strong>note</strong>: This example path is for the 64-bit location; the 32-bit location may fall under <span class="kbd">Program Files (x86)</span> instead.</i></p></li> 
     <li><p>Return to the same <strong>libraries</strong> folder, click <strong>flamingo</strong>, and then copy <i>aflamingo.dll</i> to the same Adobe Illustrator executable folder that you used in the previous step.</p></li> 
     <li><p>Return to the <strong>win32</strong> or <strong>win64</strong> folder that you selected in step 2, and then copy <i>AdobeS7FXGFileFormat.aip</i> to Adobe Illustrator's plug-ins folder. For example, <span class="kbd">C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats</span>.</p><p><i><strong>note</strong>: This example path is for the 64-bit location; the 32-bit location may fall under <span class="kbd">Program Files (x86)</span> instead.</i></p></li> 
    </ol></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e1563 " valign="top" width="NaN%"><p>Adobe Illustrator 17 in Adobe Creative Cloud</p></td> 
   <td class="cellrowborder" headers="d19e1566 " valign="top" width="NaN%"> 
    <ol> 
     <li><p>From the root of the unzipped folder, click <strong>CC</strong>.</p></li> 
     <li><p>Depending on the bit version of Adobe Illustrator that you are using, click <strong>win32</strong> or <strong>win64</strong>.</p></li> 
     <li><p>Copy <i>AdobeS7FXGFileFormat.aip</i> to Adobe Illustrator's plug-ins folder. For example, <span class="kbd">C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats</span>.</p><p><i><strong>note</strong>: This example path is for the 64-bit location; the 32-bit location may fall under <span class="kbd">Program Files (x86)</span> instead.</i></p></li> 
    </ol></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e1563 " valign="top" width="NaN%"><p>Adobe Illustrator 16 in Adobe Creative Suite 6</p></td> 
   <td class="cellrowborder" headers="d19e1566 " valign="top" width="NaN%"> 
    <ol> 
     <li><p>From the root of the unzipped folder, click <strong>6.0</strong>.</p></li> 
     <li><p>Depending on the bit version of Adobe Illustrator that you are using, click <strong>win32</strong> or <strong>win64</strong>.</p></li> 
     <li><p>Copy <i>AdobeS7FXGFileFormat.aip</i> to Adobe Illustrator's plug-ins folder. For example, <span class="kbd">C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats</span>.</p><p><i><strong>note</strong>: This example path is for the 64-bit location; the 32-bit location may fall under <span class="kbd">Program Files (x86)</span> instead.</i></p></li> 
    </ol></td> 
  </tr> 
 </tbody> 
</table>

    * **Mac**

    <table border="1" cellpadding="4" cellspacing="0" frame="border" id="WSac64270ea1b22722-107e390916129c79406-7fe1" rules="all" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e1724" valign="top" width="NaN%"><p>If you are running</p></th> 
   <th class="cellrowborder" id="d19e1727" valign="top" width="NaN%"><p>Do this</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e1724 " valign="top" width="NaN%"><p>Adobe Illustrator 18 in Adobe Creative Cloud 2014</p></td> 
   <td class="cellrowborder" headers="d19e1727 " valign="top" width="NaN%"> 
    <ol> 
     <li><p>From the root of the unzipped folder, click <strong>CC-2014</strong> &amp;gt; <strong>mac64</strong>.</p></li> 
     <li><p>Click <strong>libraries</strong> &amp;gt; <strong>flame</strong>, and then copy the <i>aflame.framework</i> folder to Adobe Illustrator package contents folder. For example, <span class="kbd">/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/</span>.</p><p>(To open Adobe Illustrator’s package contents folder, right-click on the <strong>Adobe illustrator CC 2014</strong> icon and click <strong>Show Package Contents</strong> from context menu)..</p></li> 
     <li><p>Return to the same <strong>libraries</strong> folder, click <strong>flamingo</strong>, and then copy the <i>aflamingo.framework</i> folder to the same Adobe Illustrator package contents folder that you used in the previous step.</p></li> 
     <li><p>Return to the <strong>mac64</strong> folder that you selected in step 1, and then copy the <i>AdobeS7FXGFileFormat.aip</i> folder to Adobe Illustrator’s plug-in folder. For example, <span class="kbd">/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/</span>.</p></li> 
    </ol></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e1724 " valign="top" width="NaN%"><p>Adobe Illustrator 17 in Adobe Creative Cloud</p></td> 
   <td class="cellrowborder" headers="d19e1727 " valign="top" width="NaN%"> 
    <ol> 
     <li><p>From the root of the unzipped folder, click <strong>CC</strong> &amp;gt; <strong>mac64</strong>.</p></li> 
     <li><p>Copy the <i>AdobeS7FXGFileFormat.aip</i> folder to Adobe Illustrator’s plug-in folder. For example, <span class="kbd">/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/</span>.</p></li> 
    </ol></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e1724 " valign="top" width="NaN%"><p>Adobe Illustrator 16 in Adobe Creative Suite 6</p></td> 
   <td class="cellrowborder" headers="d19e1727 " valign="top" width="NaN%"> 
    <ol> 
     <li><p>From the root of the unzipped folder, click <strong>6.0</strong> &amp;gt; <strong>mac64</strong>.</p></li> 
     <li><p>Copy the <i>AdobeS7FXGFileFormat.aip</i> folder to Adobe Illustrator’s plug-in folder. For example, <span class="kbd">/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/</span>.</p></li> 
    </ol></td> 
  </tr> 
 </tbody> 
</table>

The plug-in is now available for you to use in Adobe Illustrator.

**Browser**

**Thumbnail Size** Determines the default size of thumbnail images in Grid view in the Browse Panel.

**Default Asset Library View** Determines whether the assets in the Asset Library for build sets appear as thumbnails or by name. If you are working with large quantities of assets in the Asset Library, you can view the assets by name. For example, if you are building a large eCatalog with many PDF files, you can view the assets by name to make the list shorter.

**Default Browse Sort Order** Determines the order in which assets appear by default in the Browse Panel. Choose a sort criterion on the menu and whether you want an ascending or descending sort.

**Default Browse Location** Lets you set the browse location to the default, the last folder browsed, or to a specific location that you navigate to and identify. You can also set the browse location to sort the files and folders in ascending or descending order.

**Default Browse View** Determines whether Grid view or List view is the default view you see when you first open the Browse Panel.

**Splash Screen Display** Determines whether you see any splash screens, including the Welcome splash screen.

**Show ToolTips** Determines whether tool tips appear when you move the pointer over buttons, menus, and navigation links. Tool tips describe on-screen items.

**Checkerboard Background** Displays a checkerboard layer behind images, letting you easily see the transparent areas of an image that has an alpha channel.

**Show File Size** Displays the file size of an asset when you are browsing.

**Confirm When Leaving SPS** Displays a confirmation window before you exit Scene7 Publishing System.

**Include UDFs in Search** Deselected (default) to improve system performance for most metadata searches that you run.

If most of your metadata searches benefit from including user-defined fields, you can select this option to turn it on. As an alternative, use Advanced Search to give you a more directed and faster search experience than including user-defined fields.

See [Conducting an advanced search](searching-assets.md#conducting_an_advanced_search).

See also [User-Defined Fields](application-setup.md#user_defined_fields).

**Basic Search Type** Choose a default search type, Contains or Starts With.

**Show Media Portal Features** Select this option to access Media Portal features, such as Media Cart.

**Show Command Feedback** Show command requests to the server.

**Show Dialog During Export** Displays a dialog box when you perform an export. If you deselect this option, you can still go to the Jobs page to retrieve the results of your export.

**Email**

**Email Options** Choose how you want Scene7 to inform you by e-mail when upload and publish jobs are completed. You can receive job completion notices only if warnings or errors occurred.

**Email Scope** Determines whether you receive all job e-mail for your company or only e-mail about upload and publish jobs you initiate.

**Email Types** Determines whether you are informed when upload jobs and publish jobs are completed.

**Language**

**Preferred Language** Determines the language for the interface.

**Password**

**New Password** Enter a new, valid password. Your password must meet the following requirements:

* Be between 8-25 characters long
* Contain at least one lowercase letter
* Contain at least one uppercase letter
* Contain at least one number
* Contain at least one of the following special characters: #$&-_:{}

**Re-Type Password** Re-enter the new password to confirm that you are entering it correctly.

**Password Expiration** Determines whether your password expires after 72 days as a security measure. If you select Yes, you are asked to create a new password after 72 days.
