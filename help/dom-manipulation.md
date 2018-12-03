---
title: DOM manipulation
seo-title: DOM manipulation
description: null
seo-description: Learn about DOM manipulation.
uuid: e365e2ee-7938-4dc4-ad08-4cea4d1a83b9
contentOwner: admin
cq-gepid: scene7/using/WSef8d5860223939e2112ef46712a72891a2f-8000,scene7/using/WSef8d5860223939e22d03bf5d12a728ee296-8000,scene7/using/WSef8d5860223939e22d03bf5d12a728ee296-7fff,scene7/using/WSef8d5860223939e22d03bf5d12a728ee296-7ffe,scene7/using/WSB1AA35CE-C162-4ea2-A582-B9F310F744E8,scene7/using/WS1B5175F5-659C-44f5-8B42-90EDAE6ECFA1,scene7/using/WS3DB6D046-15D9-465b-903E-4D99002F84E9,scene7/using/WSef8d5860223939e2-141e2c7712f1259bb1b-7ffc
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_publishing
discoiquuid: 8b5b5632-4f05-4383-9992-dd27a441bde5
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 43.251-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/template_publishing;/content/help/en/experience-manager/morehelp/template_publishing
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# DOM manipulation{#dom-manipulation}

DOM (document object model) manipulation is a technique for editing a design file by directly manipulating its XML code. DOM manipulation gives you more control over variable design elements, including changing their content and appearance; you can even create new elements on an as-needed basis.

Scene7 lets you manipulate the DOM of a Scene7 FXG template by way of URL commands after the template is published. Design elements in the FXG template are manipulated by passing commands through the URL. In this way, you can dynamically manipulate and add attributes to graphics.

To use DOM manipulation, you create s7:elementIDs in your Illustrator file before converting it to a Scene7 FXG file and uploading it to SPS.

>[!NOTE]
>
>When using DOM manipulation commands, all values passed in must be URL-encoded.

>[!NOTE]
>
>Illustrator Plug-in for Web-to-Print (for converting Illustrator files) converts to FXG 2.0. For information about this specification, see [www.adobe.com/go/learn_s7_fxg2_en](http://www.adobe.com/go/learn_s7_fxg2_en).

## Creating s7:elementIDs in Illustrator files {#creating-s-elementids-in-illustrator-files}

To use DOM manipulation with a design created in Illustrator, create s7:elementIDs in your Illustrator design. Creating s7:elementIDs enables design elements to be modified with URL commands after the template is published.

### Creating s7:elementIDs for DOM manipulation of text {#creating-s-elementids-for-dom-manipulation-of-text}

To create an s7:elementID for DOM manipulation of a text object, open the Layers panel in Illustrator. Then, on the text layer that holds variable text, name the layer with a s7:elementID. To do so, enter the letters `id` (for identification), a colon ( `:`), and a name. Following are examples of s7:elementID text layer names:

`id:BirthdayBoyName`

`id:DateofBirth`

`id:EnterFirstNameHer`

### Creating s7:elementIDs for DOM manipulation of objects {#creating-s-elementids-for-dom-manipulation-of-objects}

Create s7:elementIDs for objects when you want end users to be able to change the attributes of objects. Objects can constitute entire text frames, graphics, and images. A color background is an example of an object element ID. As the seasons change, the end user can swap out the background color of a poster to make the poster appropriate to the season.

Before you create an s7:element ID for an object in Illustrator, create a separate layer for the object.

Follow these steps to create an s7:elementID for an object in Illustrator:

1. Select the object.
1. Click **Windows** &gt; **Layers**.
1. In the Layers panel, name the object layer with an s7:elementID. To do so, enter the letters `id` (for identification), a colon ( `:`), and description to identify the element. Following are examples of s7:elementID object layer names:

   `id:BackgroundColor`

   `id:RotationPercentage`

   `id:JacketJPG`

## Publish FXG templates {#publish-fxg-templates}

Publishing your FXG template places it on the Scene7 servers, where it is available to your web site and application. During the publishing process, the Scene7 Publishing System activates the URLs you need for your web site or application.

>[!NOTE]
>
>To use your FXG template, publish all content that went into making it, including fonts and images. If you don’t include all required files, an error message appears when you publish.

### Mark FXG templates for publish {#mark-fxg-templates-for-publish}

Templates and all their support files must be marked for publish for them to be placed on Scene7 Image Servers.

1. In the Browse Panel, select the FXG template along with any graphics, images, and fonts used.
1. Click **Mark For Publish**.

### Publish your FXG template {#publish-your-fxg-template}

1. On the Global Navigation bar, click **Publish**.
1. Select a When option, and optionally enter a name for the publish job.
1. Click **Start Publish**.

### Text overflow indicator display {#text-overflow-indicator-display}

A *text overflow indicator* shows when text exceeds the space allocated for it in a text frame (or in the last text frame in the case of threaded text). The indicator is a red box with a plus sign in it. Text overflow indicators on SPS are always enabled.

Text overflow indicators are controlled with the `markOverflowingTextFrame` modifier. Use the modifier as follows:

<table cellpadding="4" cellspacing="0"> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e21772" valign="top" width="NaN%"><p>Modifier/Values</p></th> 
   <th class="cellrowborder" id="d19e21775" valign="top" width="NaN%"><p>Description</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e21772 " valign="top" width="NaN%"><p><span class="code">markOverflowingTextFrame</span>=0,1</p></td> 
   <td class="cellrowborder" headers="d19e21775 " valign="top" width="NaN%"><p>The 1 value makes text flow indicators appear. Default is 0. (Although the default is 0, text overflow indicators in SPS are always enabled.) Note that the <span class="code">markOverflowingTextFrame</span> modifier is case-sensitive.</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORE_LIKE_THIS]
>
>* [Defining variability: Parameterization versus DOM manipulation](defining-variability-parameterization-versus-dom.md#defining_variability_parameterization_versus_dom_manipulation)
>* [Publishing](publishing-files.md#publishing_files)
