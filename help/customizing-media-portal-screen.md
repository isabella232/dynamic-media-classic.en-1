---
title: Customizing the Media Portal screen
seo-title: Customizing the Media Portal screen
description: null
seo-description: Learn how to customize the Media Portal screen.
uuid: de59825c-3de2-41bc-a277-2c653197bb33
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WSef8d5860223939e266034dbf12ac11b4c6d-8000
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 9d8a29c2-7d56-4fd6-a657-457c28d69dea
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 43.101-0400
lr-lastmodifiedby: admin
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Customizing the Media Portal screen{#customizing-the-media-portal-screen}

The Media Portal style settings allow you to brand the Media Portal screen with your company logo and colors. Use the style settings to put your company stamp on Media Portal.

To access the style settings, choose **Setup** &gt; **Media Portal Setup** &gt; **Style Settings**. Be sure you click **Save** to save your settings after you make them. You can click **Restore** to bring back the default settings. As you make your choices, the Preview panel shows you what your choices look like.

**Logo** Click Browse and choose a graphic in the Select Logo Image window.

**Application** Create a gradient color blend by making choices on the Background Gradient Colors menus.

**Tree** Choose a rollover color (the color that appears when you move the pointer over an item) and selection color (the color that appears when you select an item).

**Accordion** Choose background colors, a border style, and rollover and selected colors for the accordion that appears on the right side of the screen in Details view.

**Accordion Header** Choose whether to make text in the accordion header boldface.

**Datagrid** Choose colors for the header row in data grids.

**Alert** Choose a background color for alert message boxes.

**Progress Bar** Choose a color for the bar that indicates the progress of uploads and downloads.

For Media Portal users to see the style settings you choose, they must append `?company=(company name)` to the URL with which they access Media Portal. For example, to see style settings, Media Portal users who access the PortalCo company at the following:

`http://s7sps1.scene7.com/MediaPortal`

would use the following URL instead:

`http://s7sps1.scene7.com/MediaPortal?company=PortalCo`

Including the company name in the URL enables Media Portal to recognize which company a user wants to access and apply the company’s style settings accordingly.

You can learn more about communicating URL changes to Media Portal users, and setting up a Welcome e-mail message so new users receive the correct Media Portal URL.

See [Email Communications](#UnresolvedLink-sc7_setup_se.xml#WS874C2EDC-7FFA-4449-ACDD-FFD8AFF40E6F) and [Set up the Welcome e-mail message for Media Portal users](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).
