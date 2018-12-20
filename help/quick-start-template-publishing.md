---
title: "Quick Start: Template publishing"
seo-title: "Quick Start: Template publishing"
description: null
seo-description: An introduction and Quick Start to Template publishing to help you get up and running quickly.
uuid: 101b6211-2421-4565-8635-944315a5c512
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 03671fc1-ce3b-4fae-ad1f-53c99abcabde
index: y
internal: n
snippet: y
---

# Quick Start: Template publishing{#quick-start-template-publishing}

Adobe Scene7 Web-to-Print lets you create professionally branded print content that is easy for your customers, clients, and staff to customize and personalize. You can maintain corporate content and brand identity throughout the publishing process. End users can customize the print content — but only the part of the content that you allow them to customize. Personalized stationary, business cards, posters, greeting cards, labels, checks, gifts, clothing, calendars, scrapbooks, and photo albums are examples of customized print products that you can deliver. Corporations can maintain a common brand identity in their signage that can be customized for different regions, franchises, stores, and branch offices.

You start by designing a template in Adobe Illustrator. The template carefully defines what is constant and what is variable — the variable components being the ones that can be customized. For example, after text in an Illustrator file is parameterized, end users can enter text of their own. Similarly, a background color, after it is parameterized as a variable component, can be swapped for a different background color.

Scene7 offers two Template Publishing workflows, one for basic use cases and one for advanced use cases. Basic use cases entail creating a design in Adobe Illustrator, uploading it to Scene7, and defining variable elements with parameters in SPS. Advanced use cases require a more comprehensive definition of variability. Advanced use cases entail creating variable elements in Adobe Illustrator, uploading the file to Scene7, and directly manipulating those elements on a XML-level with URL calls. This scenario is called *`*DOM manipulation*`*.

>[!NOTE]
>
>For more information about Scene7 web-to-print workflows, template creation, parameterization, DOM manipulation, and more, see the Web-to-Print Workflow Guide here: [www.adobe.com/go/learn_s7_webtoprint_en](https://www.adobe.com/go/learn_s7_webtoprint_en) . Download the Zip file to your local hard drive and extract its contents (the Scene7 Web-To-PrintWorkflow Tutorial document and tutorial assets).

**Quick Start**

This Quick Start describes the basic workflow for using Illustrator files to create high-quality, customizable print products.

**1. Design your Illustrator file for Template Publishing**

In Illustrator, design your template. If you want to use the advanced, DOM manipulation method to customize your template, define s7:elementIDs for variable elements in Illustrator.

See [Create the initial template in Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator) and [DOM manipulation](dom-manipulation.md#dom_manipulation).

**2. Convert your template to Scene7 FXG and upload it to Scene7 Publishing System**

Adobe Creative Cloud users can use the Adobe Illustrator Plug-in for Web-to-Print. This plug-in converts templates to Scene7 FXG. If a template contains fonts, corresponding font files must be uploaded to the Scene7 Publishing System before uploading the FXG file.

See [Upload files for Template Publishing](upload-files-template-publishing.md#upload_files_for_template_publishing).

**3. View, define, or refine parameters in Scene7**

In the Template Publishing Preview and Build screens, you can define and refine variable elements via parameters, preview the results, and test the results. In these screens, you can:

* Create and modify parameters.
* Specify default values for parameter properties and attributes. 
* Click Copy URL to copy the preview URL to the Clipboard and preview the result in a browser window.

See [Parameterizing a template in Scene7](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7).

**4. Publish the FXG template**

After you finish defining and testing parameters and attributes, publish the file. Publishing your FXG template places it on the Scene7 Image Servers and activates the URL.

Be sure to publish all images and fonts associated with your FXG template.

See [Publish FXG templates](dom-manipulation.md#publish_fxg_templates).

**5. Obtain the URL**

Via its URL, the template is now ready to be embedded in your web site for end users to personalize variable content.

See [Linking an FXG template to a web page](linking-fxg-template-web-page.md#linking_an_fxg_template_to_a_web_page).
