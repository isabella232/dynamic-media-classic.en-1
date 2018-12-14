---
title: Linking a Spin Set to a web page
seo-title: Linking a Spin Set to a web page
description: null
seo-description: Learn how to link a Spin Set to a web page.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
index: y
internal: n
snippet: y
---

# Linking a Spin Set to a web page{#linking-a-spin-set-to-a-web-page}

Web sites and applications access Scene7 Image Server content, including Spin Sets, by way of URL strings or embedded code. These URL strings are activated during the publishing process. To place the URL string or embed code for your Spin Set in your web pages and applications, you copy it from the Scene7 Publishing System.

>[!NOTE]
>
>The URL is not active until you publish the asset.

## Copying a Spin Set URL {#copying-a-spin-set-url}

1. In the Asset Browse panel, in the Show drop-down list, click **Spin Set**.
1. in the Asset Library panel on the left side, navigate to the asset folder that contains the Spin Set whose embed code you want to copy.
1. Above the Asset Browse panel, on the right side of the toolbar, do one of the following:

    * Click **Grid View**. In the Asset Browse panel, double-click a single asset to open it in Detail View. In the URLs and Embed Code panel on the right, click **Copy URL** to the right of the viewer you want.
    * Click **Grid View**. In the Asset Browse panel, select a single asset, and then below the thumbnail image, click **Preview** &gt; **Viewer List**.

      In the Viewer List page, under the Actions column of the table, click **Copy URL**.
    
    * Click **List View**. In the Asset Browse panel, select a single asset, and then to the right of the thumbnail image, click **Preview** &gt; **Viewer List**.

      In the Viewer List page, under the Actions column of the table, click **Copy URL**.
    
    * Click **Grid View**, **List View**, or **Detail View**. On the same toolbar, click **Preview** &gt; **Viewer List**.

      In the Viewer List page, under the Actions column of the table, click **Copy URL**.

## Adding Spin Set URLs to your web page {#adding-spin-set-urls-to-your-web-page}

Spin Sets are deployed like all zoom viewers, by way of a dynamic page (ASP or JSP) that displays the Spin Set in a zoom window. The URL call to the Scene7 platform follows the same protocol on the zoom viewer. However, the Viewer Preset name depends on the Preset that your administrator defined as the default Spin Set Viewer Preset. For example, the following non-live, URL syntax example includes a Preset name called `viewer.jsp` and the SKU parameter is now the Spin Set name:

```as3
http://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

In this URL syntax example (the link is not live), notice a SKU number ( `sku=backpack_spin`). The string after `sku=` is the Spin Set name ( `backpack spin`).

## Copying the embed code of a Spin Set viewer {#copying-the-embed-code-of-a-spin-set-viewer}

Using the Embed Code feature lets you review the viewer code for the selected Spin Set. You can also copy the code to the clipboard so you can paste it in your web pages for deployment of the viewer. Editing of the code is not permitted in the Embed Code dialog box.

**To copy the embed code of a Spin Set viewer**

1. In the Asset Browse panel, in the Show drop-down list, click **Spin Set**.
1. in the Asset Library panel on the left side, navigate to the asset folder that contains the Spin Set whose embed code you want to copy.
1. Above the Asset Browse panel, on the right side of the toolbar, do one of the following:

    * Click **Grid View**. In the Asset Browse panel, double-click a single asset to open it in Detail View. In the URLs and Embed Code panel on the right, click **Embed Code** to the right of the viewer you want.
    * Click **Grid View**. In the Asset Browse panel, select a single asset, and then below the thumbnail image, click **Preview** &gt; **Viewer List**.

      In the Viewer List page, under the Actions column of the table, click **Embed Code**.
    
    * Click **List View**. In the Asset Browse panel, select a single asset, and then to the right of the thumbnail image, click **Preview** &gt; **Viewer List**.

      In the Viewer List page, under the Actions column of the table, click **Embed Code**.
    
    * Click **Grid View**, **List View**, or **Detail View**. On the same toolbar, click **Preview** &gt; **Viewer List**.

      In the Viewer List page, under the Actions column of the table, click **Embed Code**.

1. In the Embed Code dialog box, click **Copy to Clipboard**.

   Editing the code is not permitted in the Embed Code dialog box.

1. Click Close.

