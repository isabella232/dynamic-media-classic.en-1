---
title: "Quick Start: Template Basics"
description: An introduction and Quick Start to Template Basics to help you get up and running quickly in Adobe Dynamic Media Classic.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
---
# Quick Start: Template Basics{#quick-start-template-basics}

Template Basics are dynamically created and addressable layered image files like layered files in image-editing applications such as Adobe Photoshop. Unlike a static file containing layers, such as a PSD file, a template can include parameters. Through parameters, the different aspects of the image can be addressed and customized.

A template can contain any number of image layers and text layers. You can convert a static file containing layers, such as a layered PSD file, into a template, and create templates in Adobe Dynamic Media Classic. You can create text layers in templates using fonts that you uploaded into Adobe Dynamic Media Classic. After you add text to a template, you can format it by changing its justification, fonts, font size, and color.

Using the Parameters page, you can convert any aspect of a template to an addressable parameter. In so doing, you can change which layered image to use or what text value to use in your template. Parameters are passed with the URL string, allowing you to change any parameter to dynamically customize the reply image generated from the image server.

This Quick Start is designed to get up and running quickly with Template Basics.

## 1. Upload the files

Start by uploading the PSD file or image file for your template. Adobe Dynamic Media Classic supports many image file formats in addition to PSD, but lossless TIFF and PNG images are recommended for templates because they allow for transparency.

If you are using a PSD file to build your template, select **[!UICONTROL Create Template]** on the **[!UICONTROL Upload Job Options]** dialog box when you upload the PSD file. Also choose a **[!UICONTROL Layer Naming]** option so Adobe Dynamic Media Classic knows how to name PSD layers when they are uploaded to Adobe Dynamic Media Classic.

If you are using image files, you can crop the images and also create a mask from clipping paths in the images as you upload them.

On the Global Navigation bar, select **[!UICONTROL Upload]** to upload a PSD file or other image files from your computer to a folder on Adobe Dynamic Media Classic. See [Upload template files](uploading-template-files.md#uploading_template_files).

## 2. Create a template

To create a template from a PSD file, select **[!UICONTROL Create Template]** when you upload the file. To create a template from images, on the Global Navigation bar, go to **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**, enter a width and height measurement for the canvas. Near the upper-right corner of the page, select either **[!UICONTROL Designer]** or **[!UICONTROL Developer]**, and drag images onto the Template page. You can also select the images *before* you go to **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. The Template page offers tools for:

* Adding image layers. To add a layer, drag an image into the Template page.
* Adding text layers. Select the **[!UICONTROL Text tool]** icon. Drag the pointer to create a box for the text layer; then format the text with tools on the Text page.
* Changing the size and position of layers.
* Changing the order of layers.
* Applying shadow and glow effects to image and text layers.

See [Create a template](creating-template.md#creating_a_template).

## 3. Create template parameters

The next step is to parameterize the properties on layers to determine which layer properties are included in the URL string. Parameters allow you to use templates with maximum flexibility. After you make a layer property into a parameter, you can change it dynamically.

To parameterize a layer, open the template in the Template page, and then select **[!UICONTROL Parameters]** next to a layer name. On the Parameters page, select the option next to each parameter you want to add. See [Create template parameters](creating-template-parameters.md#creating_template_parameters).

## 4. Publish templates

Publishing your template places it on Dynamic Media Image Servers so that it can be dynamically delivered to your web site or application. Publishing also activates the URL to call the template from Dynamic Media Image Servers to your web site or application.

Be sure to publish all images associated with your template.

To publish a template, mark it for publish and on the Global Navigation bar, select **[!UICONTROL Publish]**. Then select **[!UICONTROL Submit Publish]**. See [Publish templates](publishing-templates.md#publishing_templates).

## 5. Link a template to a web page

Dynamic Media Classic creates URLs for templates, and activates the URLs when you publish templates to Dynamic Media Image Servers. You can copy these URL strings from the Template Preview page.

Select your template in the Browse Panel, and then select **[!UICONTROL Preview]** to open the Template Preview page. Choose an Image Preset for delivering your template, and then select **[!UICONTROL Copy URL]**. After you copy the URL from the Preview page, you can use it in your web site or application. See [Link a template to a web page](linking-template-web-page.md#linking_a_template_to_a_web_page).
