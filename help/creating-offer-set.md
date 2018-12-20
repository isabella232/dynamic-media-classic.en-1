---
title: Creating an offer set
seo-title: Creating an offer set
description: null
seo-description: Learn how to create an offer set.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
index: y
internal: n
snippet: y
---

# Creating an offer set{#creating-an-offer-set}

You can create any of the following types of offer sets:

* Video
* Parameterized template
* Image

For templates, click **Add and Preview**, then set the parameters you choose. The other offer set types do not include parameters, but you can still customize them by clicking **Preview** and changing the available presets.

Scene7 offers tools for editing as well as creating offer sets.

>[!NOTE]
>
>Before you create an offer set, be sure you publish all assets that you intend to use for the set to Scene7 Publishing System. See [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

## Types of offer sets {#types-of-offer-sets}

Create an offer set from the following types of offer sets:

**Images** You can assemble images for an offer set. Each image includes a different offer in the set.

**Image template** You can parameterize image templates in Scene7 with the Build > Template Basics command. Through parameters, components of the template — the text in text frames, the different images — can be swapped out and customized. For an offer set, you can use template parameters to create variations on the same image in your offer set, for example. For information about creating and parameterizing image templates, see Creating template parameters.

**Video** You can assemble video for an offer set. Each video is a different offer in the set.

## Creating an offer set with a parameterized template {#creating-an-offer-set-with-a-parameterized-template}

When you create an Offer Set, the **Publish after save** option affects the set and set members in the following ways:

<table border="1" cellpadding="4" cellspacing="0" frame="border" rules="all" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e27297" valign="top" width="NaN%"><p>“Publish after save” option selected before saving?</p></th> 
   <th class="cellrowborder" id="d19e27300" valign="top" width="NaN%"><p>State of set after saving</p></th> 
   <th class="cellrowborder" id="d19e27303" valign="top" width="NaN%"><p>State of set members after saving</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e27297 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e27300 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e27303 " valign="top" width="NaN%"><p>Published</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e27297 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e27300 " valign="top" width="NaN%"><p>Unpublished</p></td> 
   <td class="cellrowborder" headers="d19e27303 " valign="top" width="NaN%"><p>Set members retain their published or unpublished state.</p></td> 
  </tr> 
 </tbody> 
</table>

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To create an offer set with a parameterized template**

1. Select the template or banner.
1. Click **Build** &gt; **Target Classic Offer Set**.

   The Target Classic Offer Set page lists offers in the offer set. The first item on the list is the object. 

1. Select the object and click **Add & Preview**.

   The left side of the page lists parameters in the template and their values.

1. Change parameter values to create the offer. For example, enter different text in a text field, change the size of a layer, swap one image for another, or choose a different viewer preset.
1. Click **Save** or **Save As** to save the offer as part of the offer set.

   The Target Classic Offer Set page lists the offers you created.

1. Repeat steps 3 through 5 to create more offers for the set.
1. When you finish, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Close**, enter a name for the offer set, and then click **Save**.

Before you close the Target Classic Offer Set page, push the offer set to Target Classic. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Creating an offer set with images or videos {#creating-an-offer-set-with-images-or-videos}

When you create an Offer Set, the **Publish after save** option affects the set and set members in the following ways:

<table> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e27421" valign="top" width="NaN%"><p>“Publish after save” option selected before saving?</p></th> 
   <th class="cellrowborder" id="d19e27424" valign="top" width="NaN%"><p>State of set after saving</p></th> 
   <th class="cellrowborder" id="d19e27427" valign="top" width="NaN%"><p>State of set members after saving</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e27421 " valign="top" width="NaN%"><p>Yes</p></td> 
   <td class="cellrowborder" headers="d19e27424 " valign="top" width="NaN%"><p>Published</p></td> 
   <td class="cellrowborder" headers="d19e27427 " valign="top" width="NaN%"><p>Published</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e27421 " valign="top" width="NaN%"><p>No</p></td> 
   <td class="cellrowborder" headers="d19e27424 " valign="top" width="NaN%"><p>Unpublished</p></td> 
   <td class="cellrowborder" headers="d19e27427 " valign="top" width="NaN%"><p>Set members retain their published or unpublished state.</p></td> 
  </tr> 
 </tbody> 
</table>

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To create an offer set with images or videos**

1. Assemble images or videos for the offer set. Start in the Target Classic Offer Set screen or in the Grid View or List View and use one of the following methods:

   **Target Classic Offer Set screen** Click Build > Target Classic Offer Set. Drag images or videos onto the screen. To create varying sizes of videos or images, drag in multiple copies of the image or video and set each size individually.

   **Grid or List view** Select the images or videos, and then click Build > Target Classic Offer Set.

1. Optionally, select an image or video and click **Preview**. On the Preview Offers page, you can change the size and look of the image or video you selected. Or, you can change all images or videos in the offer set.

    * Choose a Preset to change the look and size of the image or video.
    * Click the Select Presets to All check box to apply the preset you chose to all the offers in the offer set.

   Click **Save** to save your changes to the image or video offer. Then click **Close** to return to the Target Classic Offer Set page.

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **Publish after save** is selected (default).
1. Click **Save** and enter a name for the offer set, and click **Save**.

Before closing the Target Classic Offer Set page, push the offer set to Target Classic. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Editing an Offer Set {#editing-an-offer-set}

Depending on whether you edit a published set or an unpublished set, the **Publish after save** option affects the set and set members in the following ways:

|Set already published?|“Publish after save” option selected before saving your edit?|State of set after saving|State of set members after saving|
|--- |--- |--- |--- |
|Yes|Yes|Published|Published|
|Yes|No|Published|Existing set members retain their published state.Any new set members that you added during your edit retain their published or unpublished state.|
|No|Yes|Published|Published|
|No|No|Unpublished|Existing set members and any new set members that you added during your edit retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To edit an Offer Set**

1. To edit an offer set, display the offer set in Grid view or List view, and then click its **Edit** rollover button.
1. In the Target Classic Offer Set page, do any of the following:

   **Removing an offer**

   Select the offer, and then click **Delete** to remove an offer from the set.

   **Adding an offer**

   How you add an offer depends on the type of offer set you are working with:

    * Templates: Click **Add & Preview**, and on the Add & Preview Offers page, create another offer.
    * Images and videos: Drag an image or video onto the Target Classic Offer Set page.

   ***Note**: You cannot delete an offer set that is associated with a campaign. To delete an offer set associated with a campaign, log on to Target Classic and remove the campaign associations first. Even after un-associating from a campaign, the asset can only be deleted from Scene7 Publishing System, requiring a login to Target Classic, and not from within Target Classic.*

1. When you finish editing, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Save**, select a storage folder, enter a name for the set, and then click **Save**.

## Deleting an Offer Set {#deleting-an-offer-set}

When you delete an Offer Set, the set itself is moved to the Trash. However, the members (or “children”) within that set are not affected; instead, they each retain their existing published or unpublished state.

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To delete an Offer Set**

1. In the Grid View, List View, or Details View, select one or more Offer Sets.
1. On the Global Navigation Bar, click **File** &gt; **Delete** &gt; **Delete**.

>[!MORE_LIKE_THIS]
>
>* [Creating template parameters](creating-template-parameters.md#creating_template_parameters)
