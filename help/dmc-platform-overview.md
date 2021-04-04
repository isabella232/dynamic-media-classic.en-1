---
title: Adobe Dynamic Media Classic platform overview
description: An overview of the Dynamic Media Classic platform and workflow process.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
---
# Adobe Dynamic Media Classic platform overview{#adobe-scene-platform-overview}

Dynamic Media Classic is an integrated, rich media management, publishing, and serving environment. Rich media can be delivered to all marketing and selling channels, including the web, print material, e-mail campaigns, web portals, desktops, and devices.

## Workflow process {#workflow-process}

The key Dynamic Media Classic workflow steps are:

* **Upload and manage your assets**
Upload your media assets to Dynamic Media Classic. You can organize, browse, and search for assets on the system. You can also apply metadata to assets.

* **Create rich media**
Create different configurations of your assets such as eCatalogs, Image Sets, Spin Sets, Swatch Sets, Mixed Media Sets, basic Templates, and FXG Templates. For more information, see About rich media.

* **Publish and administer**
Publish assets to the Dynamic Media Classic Saas network, as well as monitor the status of assets when they are published, administer user rights, and maintain security.

* **Serve**
Deliver media from Dynamic Media Classic SaaS network to web pages, applications, and mobile devices; the media are performance-optimized and are delivered with CDN caching. Dynamic Media Classic provides you with a URL for each asset. After you publish the asset, the URL becomes active.

![The Dynamic Media Classic workflow process](/help/assets/gs_workflow.png) 

## Single master images and single URL calls {#single-master-images-and-single-url-calls}

Dynamic Media Classic is fundamentally different from other systems because you can use Dynamic Media Classic to deliver media dynamically from single master assets and URL calls.

The URL strings you generate with Dynamic Media Classic include instructions that tell the server how to display the asset when it is delivered. For example, the same master image can be delivered in different sizes, formats, weights, colors, and zoom views. As part of building and publishing media assets with Dynamic Media Classic, you visually configure the effects. In so doing, you create the URL calls that correctly tell the server how to present your master asset to applications.

![Dynamic Media Classic can deliver the same master image to different mediums in different sizes and formats.](/help/assets/gs_dynamic_publishing.png) 

## Content caching {#content-caching}

The images that Dynamic Media Classic generates dynamically are cache-friendly; in most cases, they are JPEG images with unique URL calls that identify them. The images are delivered on the content delivery network (CDN), a system of servers that are networked together on the Internet to deliver content faster. The images are distributed from servers located globally, and then to computers. When implementing a caching mechanism using any CDN vendor, you simply change the server name to point to the CDN-enabled Dynamic Media Image Server. All Dynamic Media Classic editions include bundled CDN caching.
