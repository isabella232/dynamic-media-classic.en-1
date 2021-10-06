---
title: Adobe Dynamic Media Classic program overview
description: An overview of the Adobe Dynamic Media Classic program and its entire workflow process.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
---
# Adobe Dynamic Media Classic program overview{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic is an integrated, rich media management, publishing, and serving environment. Rich media can be delivered to all marketing and selling channels, including the web, print material, e-mail campaigns, web portals, desktops, and devices.

See also [Platform overview](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) training video.

## Workflow process {#workflow-process}

The key Adobe Dynamic Media Classic workflow steps are:

* **Upload and manage your assets** - Upload your media assets to Adobe Dynamic Media Classic. You can organize, browse, and search for assets on the system. You can also apply metadata to assets.

* **Create rich media** - Create different configurations of your assets such as eCatalogs, Image Sets, Spin Sets, Swatch Sets, Mixed Media Sets, basic Templates, and FXG Templates.

* **Publish and administer** - Publish assets to the Adobe Dynamic Media Classic SaaS network. Monitor the status of assets when they are published. Administer user rights and maintain security.

* **Serve** - Deliver media from Adobe Dynamic Media Classic SaaS network to web pages, applications, and mobile devices; the media are performance-optimized and are delivered with CDN caching. Adobe Dynamic Media Classic provides you with a URL for each asset. After you publish the asset, the URL becomes active.

![The Adobe Dynamic Media Classic workflow process](/help/assets/gs_workflow.png)

## Single master images and single URL calls {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic is fundamentally different from other systems because you can use Adobe Dynamic Media Classic to deliver media dynamically from single master assets and URL calls.

The URL strings you generate with Adobe Dynamic Media Classic include instructions that tell the server how to display the asset when it is delivered. For example, the same master image can be delivered in different sizes, formats, weights, colors, and zoom views. As part of building and publishing media assets with Adobe Dynamic Media Classic, you visually configure the effects. In so doing, you create the URL calls that correctly tell the server how to present your master asset to applications.

![Adobe Dynamic Media Classic can deliver the same master image to different mediums in different sizes and formats.](/help/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic ensures that consistent, quality experiences are delivered to any screen, regardless of size or bandwidth.*

## Content caching {#content-caching}

The images that Adobe Dynamic Media Classic generates dynamically are cache-friendly; usually, they are JPEG images with unique URL calls that identify them. The images are delivered on the content delivery network (CDN), a system of servers that are networked together on the Internet to deliver content faster. The images are distributed from servers located globally, and then to computers. When implementing a caching mechanism using any CDN vendor, you simply change the server name to point to the CDN-enabled Dynamic Media Image Server. All Adobe Dynamic Media Classic editions include bundled CDN caching.
