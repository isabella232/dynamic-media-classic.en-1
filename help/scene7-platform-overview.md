---
title: Adobe Scene7 platform overview
seo-title: Adobe Scene7 platform overview
description: null
seo-description: An overview of the Dynamic Media Classic platform and workflow process.
uuid: 1e8db51e-8e39-4171-93e5-ccff6fcef391
contentOwner: admin
cq-gepid: scene7/using/WS29CDF638-B68B-4388-9BA1-D57ACB751022,scene7/using/WSFE535014-6E03-4e38-AD00-E534C6EBF164,scene7/using/WS817E2169-03F0-41f1-82E4-729332BC45F0,scene7/using/WS5A9FE6A3-B1D8-4f39-BD49-809EDBB36FE8
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: b5b8c1bc-c54d-4a5d-b462-78d691d9a1c4
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 44.436-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/getting_started;/content/help/en/experience-manager/morehelp/getting_started
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Adobe Scene7 platform overview{#adobe-scene-platform-overview}

Scene7 is an integrated, rich media management, publishing, and serving environment. Rich media can be delivered to all marketing and selling channels, including the web, print material, e-mail campaigns, web portals, desktops, and devices.

## Workflow process {#workflow-process}

The key Scene7 workflow steps are:

**Upload and manage your assets** Upload your media assets to SPS. You can organize, browse, and search for assets on the system. You can also apply metadata to assets. If you install Adobe Scene7 Publishing System desktop application, you can upload files and folders by dragging them from your desktop to an upload folder.

**Create rich media** Create different configurations of your assets such as eCatalogs, Image Sets, Spin Sets, Swatch Sets, Mixed Media Sets, basic Templates, and FXG Templates. For more information, see About rich media.

**Publish and administer** Publish assets to the Scene7 Saas network, as well as monitor the status of assets when they are published, administer user rights, and maintain security.

**Serve** Deliver media from Scene7 SaaS network to web pages, applications, and mobile devices; the media are performance-optimized and are delivered with CDN caching. Scene7 provides you with a URL for each asset. After you publish the asset, the URL becomes active.

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Illustrator source file comes from Marketing but the localized files aren’t available.</p> 
<p></p>

 -->

![]() 

## Single master images and single URL calls {#single-master-images-and-single-url-calls}

Scene7 is fundamentally different from other systems because you can use Scene7 to deliver media dynamically from single master assets and URL calls.

The URL strings you generate with Scene7 include instructions that tell the server how to display the asset when it is delivered. For example, the same master image can be delivered in different sizes, formats, weights, colors, and zoom views. As part of building and publishing media assets with Scene7, you visually configure the effects. In so doing, you create the URL calls that correctly tell the server how to present your master asset to applications.

![]() 

## Content caching {#content-caching}

The images that Scene7 generates dynamically are cache-friendly; in most cases, they are JPEG images with unique URL calls that identify them. The images are delivered on the content delivery network (CDN), a system of servers that are networked together on the Internet to deliver content faster. The images are distributed from servers located globally, and then to computers. When implementing a caching mechanism using any CDN vendor, you simply change the server name to point to the CDN-enabled Scene7 Image Server. All Scene7 editions include bundled CDN caching.
