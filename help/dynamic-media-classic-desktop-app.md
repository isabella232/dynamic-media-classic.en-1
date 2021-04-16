---
title: Adobe Dynamic Media Classic desktop app - Now available
description: Learn more about Dynamic Media Classic desktop application.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
---
# Now available: Adobe Dynamic Media Classic desktop app {#dynamic-media-classic-desktop-app}

Dynamic Media Classic users now have access to a new desktop app experience that no longer relies on Adobe Flash technology in the browser.

This new app is now available for Windows® and macOS.

>[!IMPORTANT]
>
>Adobe recommends that you install the new Adobe Dynamic Media Classic desktop app by October 1, 2020. Doing so will ensure you have a smooth transition before Adobe Flash Player is deprecated on December 31, 2020. After that date, you cannot log on to the browser version of Adobe Dynamic Media Classic user interface, labeled as Dynamic Media Classic in the product.

See the FAQ for the [New Dynamic Media Classic sign in experience now available.](/help/new-ui-2020.md)

## System requirements for Adobe Dynamic Media Classic desktop app {#system-requirements-dmc-app}

Adobe Dynamic Media Classic desktop app is compatible with the following operating systems:

* macOS 10.10 or newer.
* Windows® 7 or newer.

>[!NOTE]
>
>Upgrade notification within the Dynamic Media Classic desktop application is not generated for *minor* releases. Customers who benefit from fixes in a minor release can upgrade.

## Fixes in the minor release (20.21.2) {#minor-release}

* Known limitation in 20.21.1 of Server dropdown being empty.
* In **[!UICONTROL Upload Job Options]**, Layer naming default value under **[!UICONTROL Photoshop Options]**, is now **[!UICONTROL Photoshop and Layer Name]**. Layers in the PSD file are uploaded as separate images.
  * The earlier default of **[!UICONTROL Layer name]**, named the images after their layer name or layer number in the PSD file. The layer number was used if the layer names in the PSD file were default Photoshop layer names.
  * The new default of **[!UICONTROL Photoshop and Layer Name]**, names the images after the PSD file followed by the layer name or layer number. The layer number is used if the layer names in the PSD file are default Photoshop layer names.
  * Given that layer images in Dynamic Media Classic now have unique names, no updates to existing PSD or Templates will happen (which shared layer names in the original PSD files).
* Broken thumbnails of assets.

## Fixes in the latest version (20.21.1) {#latest-fixes-desktop-app}

* Sign in issues due to timeout resulting in the following message: *This user may be assigned to the group or groups without permission. Contact your administrator.*
* Viewer presets get duplicated with each incorrect password attempt.
* Desktop application becoming unresponsive due to many assets in the root folder. (Fixed on Windows®; working as desired on macOS.)

## Fixes in the previous version (20.20.2) {#previous-version-fixes-desktop-app}

* No limitation on the number of files that you can upload through the desktop app user interface for both macOS and Windows®.
* No need to sign out of the desktop app to switch between companies.
* Ctrl+V for paste operation now works on Windows®.
* In the future, when a new version of the desktop app is released, users will be notified within the desktop app itself.

## Download and install the latest Adobe Dynamic Media Classic desktop app on macOS or Windows® {#installation-dmc-app}

See also:

* [Download and silent install the latest Adobe Dynamic Media Classic desktop app on Mac](#install-silent-mac-dmc-app)
* [Download and silent install the latest Adobe Dynamic Media Classic desktop app on Windows®](#install-silent-windows-dmc-app)

1. Uninstall any older Dynamic Media Classic desktop app versions on your system.

1. Download the latest installer for Adobe Dynamic Media Classic desktop app.

    * The latest version (20.21.2) is available at the following:

        * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)

    * The previous version (20.21.1) is available at the following:

        * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.dmg)
        * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.exe)

<!--         * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Do one of the following based on the installer you downloaded.

    * **For macOS** - In the **[!UICONTROL Drag & drop to install]** dialog box, drag **[!UICONTROL Adobe Dynamic Media Classic]** and drop it onto **[!UICONTROL Applications]**.

        ![Drag and drop install on macOS](/help/assets/dragondrop-install1.png)

    * In the **[!UICONTROL Applications]** folder, tap the Adobe Dynamic Media Classic icon.
    * In the dialog box, tap **[!UICONTROL Open]** to open the Adobe Dynamic Media Classic desktop app.

        ![Open downloaded app](/help/assets/open-dmclassicapp1.png)

    * **For Windows** - Run the installer binary and follow the on-screen instructions to install the desktop app.

1. When you open the application, the new Adobe Dynamic Media Classic Sign in page is displayed:

    ![Dynamic Media Classic sign in](/help/assets/dmclassic-login1.png)

1. To sign in to the Adobe Dynamic Media Classic desktop app, use the same credentials that you used to log on to Dynamic Media Classic in the browser.

    For the **[!UICONTROL Server]** to use, see the following mapping for the production environment:

    | Browser URL | Desktop app server name |
    |---|---|
    | https://s7sps1.scene7.com/ | NA (North America) production |
    | https://s7sps3.scene7.com/ | EMEA (Europe, Middle East, and Africa) production |
    | https://s7sps5.scene7.com/ | APAC (Asia-Pacific) production |

1. Following sign in, notice the familiar browser user interface experience. You can continue your day to day Dynamic Media Classic activity as usual on the desktop app.

## Download and *silent* install the latest Adobe Dynamic Media Classic desktop app on macOS {#install-silent-mac-dmc-app}

See also:

* [Download and install the latest Adobe Dynamic Media Classic desktop app on Mac or Windows®](#installation-dmc-app)
* [Download and silent install the latest Adobe Dynamic Media Classic desktop app on Windows®](#install-silent-windows-dmc-app)

To download and *silent* install the latest version of Adobe Dynamic Media Classic desktop app on macOS:

1. Uninstall any older Dynamic Media Classic desktop app versions on your system.

1. Download the latest installer for Adobe Dynamic Media Classic desktop app for macOS.

    * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)

1. Mount the downloaded Disk Image (.DMG) to a mountpoint location using the following command:

    `hdiutil attach adobe-dynamic-media-classic-20.21.2.dmg -mountpoint <mount_point_path>`

1. Copy the .APP file to **[!UICONTROL Applications]** using the following command:

    `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. When you open the application, the new Adobe Dynamic Media Classic Sign in page is displayed:

    ![Dynamic Media Classic sign in](/help/assets/dmclassic-login1.png)

1. To sign in to the Adobe Dynamic Media Classic desktop app, use the same credentials that you used to log on to Dynamic Media Classic in the browser.

    For the **[!UICONTROL Server]** to use, see the following mapping for the production environment:

    | Browser URL | Desktop app server name |
    |---|---|
    | https://s7sps1.scene7.com/ | NA (North America) production |
    | https://s7sps3.scene7.com/ | EMEA (Europe, Middle East, and Africa) production |
    | https://s7sps5.scene7.com/ | APAC (Asia-Pacific) production |

## Download and *silent* install the latest Adobe Dynamic Media Classic desktop app on Windows® {#install-silent-windows-dmc-app}

The command that you use is for a basic MSI silent installation. However, the Dynamic Media Classic desktop app installer is an InstallScript MSI installer created using InstallShield. When you run the installer in record mode, any user interaction is recorded in a response file. This response file is then used for a silent installation as described in [Running Installations in Silent Mode.](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

See also:

* [Download and install the latest Adobe Dynamic Media Classic desktop app on Mac or Windows®](#installation-dmc-app)
* [Download and silent install the latest Adobe Dynamic Media Classic desktop app on macOS](#install-silent-mac-dmc-app)

To download and *silent* install the latest version of Adobe Dynamic Media Classic desktop app on Windows®:

1. Uninstall any older Dynamic Media Classic desktop app versions on your system.

1. Download the latest installer for Adobe Dynamic Media Classic desktop app.

    * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)

1. Run the installer in record mode using the following command:

    `adobe-dynamic-media-classic-20.21.2.exe /r /f1"C:\Setup.iss"`

1. In the GUI installer window, follow the steps to install so that interactions/inputs, like install location, get recorded in `Setup.iss` file.

1. Copy the created `Setup.iss` file and `adobe-dynamic-media-classic-20.21.2.exe` to other computer.

1. Run the following command for a silent installation:

    `adobe-dynamic-media-classic-20.21.2.exe /s /f1"C:\Setup.iss"`

    Details about command-line parameters are available at [Setup.exe and Update.exe Command-Line Parameters.](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. When you open the application, the new Adobe Dynamic Media Classic Sign in page is displayed:

    ![Dynamic Media Classic sign in](/help/assets/dmclassic-login1.png)

1. To sign in to the Adobe Dynamic Media Classic desktop app, use the same credentials that you used to log on to Dynamic Media Classic in the browser.

    For the **[!UICONTROL Server]** to use, see the following mapping for the production environment:

    | Browser URL | Desktop app server name |
    |---|---|
    | https://s7sps1.scene7.com/ | NA (North America) production |
    | https://s7sps3.scene7.com/ | EMEA (Europe, Middle East, and Africa) production |
    | https://s7sps5.scene7.com/ | APAC (Asia-Pacific) production |


## Video walk-through on using Dynamic Media Classic Desktop App {#dmc-app-video-walk-through}

Watch a [video walk-through on using Dynamic Media Classic Desktop App](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (Length: 2 minutes 36 seconds). 

## Clearing the image cache and asset cache on your computer using the desktop app {#clear-cache}

1. In the Dynamic Media Classic desktop app, near the upper-right corner, tap **[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**.
1. On the **[!UICONTROL Personal Setup]** page, under the **[!UICONTROL Desktop]** heading, do any of the following:
    * To remove all Adobe Dynamic Media cached image files from your computer, tap **[!UICONTROL Clear Image Cache]**, then tap **[!UICONTROL OK]**.
    * To remove all Adobe Dynamic Media cached asset files from your computer, tap **[!UICONTROL Clear Asset Cache]**, then tap **[!UICONTROL OK]**.
1. In the lower-right corner of the page, tap **[!UICONTROL Close]**.

### Clearing the image cache and asset cache manually

Besides clearing the image and asset cache using the desktop app, you can manually clear the cache directly from the file system.

1. Based on your operating system, navigate to the following:

    * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
    * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Known limitation in Dynamic Media Classic 20.21.1

* The **[!UICONTROL Server]** drop-down list is empty after updating to Dynamic Media Classic desktop app 20.21.1 - Scenario: You install and sign in to Dynamic Media Classic 20.20.1 or 20.20.2, then close the application. Then you update to Dynamic Media Classic 20.21.1. When you attempt to sign in, the **[!UICONTROL Server]** drop-down list in the **[!UICONTROL Sign in to your account]** dialog box is empty. To work around this issue, you must [manually clear the cache](#clear-cache) (see steps above).

## Known limitations in Dynamic Media Classic 20.20.1 (fixed in 20.20.2)

**_Applies to Windows® only - Is there a limitation on the number of files that can be uploaded through the desktop app UI?_**<br>Yes, a maximum of 150 files can be uploaded at a time by way of the desktop app UI.

**_Applies to Windows® and macOS - How do I switch between companies?_**<br>To switch between companies, do the following:

* In the Dynamic Media Classic app, select the new company from the company drop-down list.
* When the pop-up window appears, tap **[!UICONTROL OK]** to sign out and close the app.

    ![To use the new company, restart the app](/help/assets/dmclassic-new-company1.png)

* Restart Dynamic Media Classic, then sign in as usual to work with the new company.

## Tips and Tricks

**_I am unable to see Media Cart panel on the landing page of Dynamic Media Classic._**<br>In Dynamic Media Classic, tap **[!UICONTROL Setup > Personal Setup]**. In the Browser section, make sure **[!UICONTROL Show MediaPortal Features]** is selected (checked). Tap **[!UICONTROL Save > Close]**.

**_Publish state (green indicator) of an asset is not reflected correctly._**<br>In the browser user interface, a relogin to the UI was required to see the correct publish state of assets. In the desktop app, Adobe has introduced a **[!UICONTROL Refresh]** icon in the toolbar, to the right of the **[!UICONTROL Select None]** button. Tap the **[!UICONTROL Refresh]** icon to see the latest status of all the assets on the given page. No relogin required as with the browser UI.

![Refresh icon](/help/assets/refresh-icon1.png)
*Refresh icon*
 
**_I don't see batch set presets working in the desktop app._**<br>Tap **[!UICONTROL Upload > Job Options > Batch Set Presets]**. Ensure the relevant **[!UICONTROL Batch Set Preset]** is enabled. Click **[!UICONTROL Save and Submit upload]**.
