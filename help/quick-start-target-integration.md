---
title: "Quick Start: Adobe Target Standard/Premium integration"
description: An introduction and Quick Start to Adobe Target Standard/Premium to help you get up and running quickly with Adobe Target Standard/Premium integration techniques in Adobe Dynamic Media Classic.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
---
# Quick Start: Adobe Target Standard/Premium integration{#quick-start-target-integration}

 Adobe Target Standard/Premium puts control directly in the hands of marketers to quickly and continually run multiple A/B and multivariate tests, measure effectiveness, and increase relevance of online content through segmentation, targeting, and Automated Personalization.

Adobe Dynamic Media Classic lets you create offers and offer sets for Adobe Target Standard/Premium campaigns. For example, you can create an offer set with three variations of the same rich media asset. Then you can have Adobe Target Standard/Premium determine which asset provides better conversion lift. You can create offers and offer sets from a Basic Template or from individual images. After the offer set is pushed or saved to Adobe Target Standard/Premium, where the offers are associated with mboxes and experiences, Adobe Target Standard/Premium can run campaigns. These campaigns determine which variation of a website is likely to perform best for click-throughs and conversion.

For greater customization of dynamic Adobe Dynamic Media Classic content, use Adobe Target Standard/Premium HTML offers. See the [Adobe Target Standard/Premium product documentation](https://experienceleague.adobe.com/docs/target.html) for more information.

>[!NOTE]
>
>A valid Adobe Target Standard/Premium account is required to use Adobe Target Standard/Premium with Adobe Dynamic Media Classic.

This Quick Start is designed to get you up and running quickly with Adobe Target Standard/Premium HTML offer sets. Follow steps 1 through 3. After each step is a cross-reference to a topic heading where you can find more information.

## 1. Enter your Adobe Target Standard/Premium URL in the Application General Settings page

Adobe Dynamic Media Classic needs your Adobe Target Standard/Premium URL to integrate with Adobe Target Standard/Premium. Copy the portion of your Adobe Target Standard/Premium URL up to and including `.com`, and enter it in the Adobe Dynamic Media Classic **[!UICONTROL Application General Settings]** page, in the **[!UICONTROL Servers]** group, **[!UICONTROL Test&Target Server Name]** text field. See [Integrate Adobe Dynamic Media Classic with Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Create the offer set

Use a parameterized template or images to create an offer set. You create HTML offer sets on the Test&Target Offer Set page. To open this page, select your template or images, then on the Global Navigation bar, go to **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

To create an offer with a template, select **[!UICONTROL Add & Preview]**. On the Add & Preview page, change parameter values.

To create an offer with images, drag images into the Test&Target Offer Set page. Select **[!UICONTROL Preview]** and choose an Image Preset for an image or all the images in the offer set.

Save the offer set after you create it.

See [Create an offer set](creating-offer-set.md#creating_an_offer_set).

## 3. Push the offer set to Adobe Target Standard/Premium

In the Test&Target Offer Set page, select **[!UICONTROL Push Offers]**, and enter your login credentials in the Test&Target Login dialog box. See [Push offer sets to Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
