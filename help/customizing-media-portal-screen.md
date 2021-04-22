---
title: Customizing the Media Portal screen
description: Learn how to customize the Media Portal screen.
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Administrator,Business Practitioner
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
---
# Customizing the Media Portal screen{#customizing-the-media-portal-screen}

The Media Portal style settings allow you to brand the Media Portal screen with your company logo and colors. Use the style settings to put your company branding on Media Portal.

To access the style settings, choose **[!UICONTROL Setup]** > **[!UICONTROL Media Portal Setup]** > **[!UICONTROL Style Settings]**. Be sure you click **[!UICONTROL Save]** to save your settings after you make them. You can click **[!UICONTROL Restore]** to bring back the default settings. As you make your choices, the Preview panel shows you what your choices look like.

* **Logo** - Click **[!UICONTROL Browse]** and choose a graphic in the Select Logo Image window.

* **Application** - Create a gradient color blend by making choices on the Background Gradient Colors menus.

* **Tree** - Choose a rollover color (the color that appears when you move the pointer over an item) and selection color (the color that appears when you select an item).

* **Accordion** - Choose background colors, a border style, and rollover and selected colors for the accordion that appears on the right side of the screen in Details view.

* **Accordion Header** - Choose whether to make text in the accordion header boldface.

* **Datagrid** - Choose colors for the header row in data grids.

* **Alert** - Choose a background color for alert message boxes.

* **Progress Bar** - Choose a color for the bar that indicates the progress of uploads and downloads.

For Media Portal users to see the style settings that you chose, they must append `?company=(company name)` to the URL with which they access Media Portal. For example, to see style settings, Media Portal users who access the PortalCo company at the following:

`https://s7sps1.scene7.com/MediaPortal`

Use the following URL instead:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

Including the company name in the URL enables Media Portal to recognize which company a user wants to access and apply the company’s style settings accordingly.

You can learn more about communicating URL changes to Media Portal users, and setting up a Welcome e-mail message so new users receive the correct Media Portal URL.

See [Set up the Welcome e-mail message for Media Portal users](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
