---
title: Pushing offer sets to Adobe Target Classic
seo-title: Pushing offer sets to Adobe Target Classic
description: null
seo-description: Learn how to push offer sets to Adobe Target Classic.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
index: y
internal: n
snippet: y
---

# Pushing offer sets to Adobe Target Classic{#pushing-offer-sets-to-adobe-target-classic}

After you create or edit an offer set, push it to Target Classic by following these steps:

1. In the Target Classic Offer Set screen, click the Push Offers button. 
1. Enter your login credentials.
1. Click the Login button.

During the transfer to Target Classic, the prefix S7_ is attached automatically to the start of offer names. This prefix is attached to ensure that you can easily find Scene7 offers in the Target Classic offer list. For example, the offer appears as S7_&lt;name of offer set&gt;_&lt;offer name&gt;.

SPS pushes into Target Classic widget offers. You can use Widget offers to host your own offer content outside Target Classic. Widget offers are similar to a standard offer hosted outside Target Classic. They allow Target Classic to deploy offer content that is stored on your server, allowing for more sophisticated and dynamic usage. Widget offers retrieve content from a URL, caching and serving that content for approximately two hours. Widget offers provide some dynamic content generation capabilities that other offers outside Target Classic do not. If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. These parameters can be used by a service available at the Widget offer URL to return content outside Target Classic that uses product or order information from your mboxes. The Widget offer is also accessible through the API to programmatically create offers outside Target Classic.
