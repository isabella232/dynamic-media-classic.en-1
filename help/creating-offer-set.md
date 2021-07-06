---
title: Creating an offer set
description: Learn how to create an offer set.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
---
# Creating an offer set{#creating-an-offer-set}

You can create any of the following types of offer sets:

* Video
* Parameterized template
* Image

For templates, click **[!UICONTROL Add and Preview]**, then set the parameters you choose. The other offer set types do not include parameters, but you can still customize them by clicking **[!UICONTROL Preview]** and changing the available presets.

Dynamic Media Classic offers tools for editing as well as creating offer sets.

>[!NOTE]
>
>Before you create an offer set, be sure you publish all assets that you intend to use for the set to Dynamic Media Classic. See [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

## Types of offer sets {#types-of-offer-sets}

Create an offer set from the following types of offer sets:

* **Images** - You can assemble images for an offer set. Each image includes a different offer in the set.

* **Image template** - You can parameterize image templates in Dynamic Media Classic with the Build > Template Basics command. Through parameters, components of the template — the text in text frames, the different images — can be swapped out and customized. For an offer set, you can use template parameters to create variations on the same image in your offer set, for example. For information about creating and parameterizing image templates, see Creating template parameters.

* **Video** - You can assemble video for an offer set. Each video is a different offer in the set.

## Creating an offer set with a parameterized template {#creating-an-offer-set-with-a-parameterized-template}

When you create an Offer Set, the **[!UICONTROL Publish after save]** option affects the set and set members in the following ways:

|“Publish after save” option selected before saving?|State of set after saving|State of set members after saving|
|--- |--- |--- |
|Yes|Published|Published|
|No|Unpublished|Set members retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To create an offer set with a parameterized template:**

1. Select the template or banner.
1. Click **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

   The Test&Target Offer Set page lists offers in the offer set. The first item on the list is the object. 

1. Select the object and click **[!UICONTROL Add & Preview]**.

   The left side of the page lists parameters in the template and their values.

1. Change parameter values to create the offer. For example, enter different text in a text field, change the size of a layer, swap one image for another, or choose a different viewer preset.
1. Click **[!UICONTROL **Save]** or **[!UICONTROL Save As**]** to save the offer as part of the offer set.

   The Test&Target Offer Set page lists the offers you created.

1. Repeat steps 3 through 5 to create more offers for the set.
1. When you finish, near the lower-right corner of the page, ensure that **[!UICONTROL Publish after save*]** is selected (default).
1. Click **[!UICONTROL Close]**, enter a name for the offer set, and then click **[!UICONTROL Save]**.

Before you close the Test&Target Offer Set page, push the offer set to Adobe Target Standard/Premium. See [Pushing offer sets to Test&Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Creating an offer set with images or videos {#creating-an-offer-set-with-images-or-videos}

When you create an Offer Set, the **[!UICONTROL Publish after save]** option affects the set and set members in the following ways:

|**[!UICONTROL Publish after save]** option selected before saving?|State of set after saving|State of set members after saving|
|--- |--- |--- |
|Yes|Published|Published|
|No|Unpublished|Set members retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To create an offer set with images or videos:**

1. Assemble images or videos for the offer set. Start in the Test&Target Offer Set screen or in the Grid View or List View and use one of the following methods:

   * **Test&Target Offer Set screen** - Click **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**. Drag images or videos onto the screen. To create varying sizes of videos or images, drag in multiple copies of the image or video and set each size individually.

   * **Grid view or List view** - Select the images or videos, and then click **[!UICONTROL Build]** > **[!UICONTROL Test&Target Offer Set]**.

1. Optionally, select an image or video and click **[!UICONTROL Preview]**. On the Preview Offers page, you can change the size and look of the image or video you selected. Or, you can change all images or videos in the offer set.

    * Choose a Preset to change the look and size of the image or video.
    * To apply the preset you chose to all the offers in the offer set, click the **[!UICONTROL Select Presets to All]** check box.

   Click **[!UICONTROL Save]** to save your changes to the image or video offer. Then click **[!UICONTROL Close]** to return to the Test&Target Offer Set page.

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **[!UICONTROL Publish after save]** is selected (default).
1. Click **[!UICONTROL Save]** and enter a name for the offer set, and click **[!UICONTROL Save]**.

Before closing the Test&Target Offer Set page, push the offer set to Adobe Target Standard/Premium. See [Pushing offer sets to Test&Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Editing an Offer Set {#editing-an-offer-set}

Whether you edit a published set or an unpublished set, the **[!UICONTROL Publish after save]** option affects the set and set members in the following ways:

|Set already published?|**[!UICONTROL Publish after save]** option selected before saving your edit?|State of set after saving|State of set members after saving|
|--- |--- |--- |--- |
|Yes|Yes|Published|Published|
|Yes|No|Published|Existing set members retain their published state. Any new set members that you added during your edit retain their published or unpublished state.|
|No|Yes|Published|Published|
|No|No|Unpublished|Existing set members and any new set members that you added during your edit retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To edit an Offer Set:**

1. To edit an offer set, display the offer set in Grid view or List view, and then click its **[!UICONTROL Edit]** rollover button.
1. In the Test&Target Offer Set page, do any of the following:

    * **Removing an offer** - Select the offer, and then click **[!UICONTROL Delete]** to remove an offer from the set.
    * **Adding an offer** - How you add an offer depends on the type of offer set you are working with:
      * **Templates** - Click **[!UICONTROL Add & Preview]**, and on the Add & Preview Offers page, create another offer.
      * **Images and videos** - Drag an image or video onto the Test&Target Offer Set page.

    >[!NOTE]
    >
    >You cannot delete an offer set that is associated with a campaign. To delete an offer set associated with a campaign, sign in to Adobe Target Standard/Premium and remove the campaign associations first. Even after unassociating from a campaign, the asset can only be deleted from Dynamic Media Classic, requiring a sign in to Adobe Target Standard/Premium, and not from within Adobe Target Standard/Premium.

1. When you finish editing, near the lower-right corner of the page, ensure that **[!UICONTROL Publish after save]** is selected (default).
1. Click **[!UICONTROL Save]**, select a storage folder, enter a name for the set, and then click **[!UICONTROL Save]**.

## Deleting an Offer Set {#deleting-an-offer-set}

When you delete an Offer Set, the set itself is moved to the Trash. However, the members (or “children”) within that set are not affected; instead, they each retain their existing published or unpublished state.

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To delete an Offer Set:**

1. In the Grid View, List View, or Details View, select one or more Offer Sets.
1. On the Global Navigation Bar, click **[!UICONTROL File]** > **[!UICONTROL Delete]** > **Delete**.

>[!MORELIKETHIS]
>
>* [Creating template parameters](creating-template-parameters.md#creating_template_parameters)
