---
title: Create template parameters
description: Learn how to create template parameters in Adobe Dynamic Media Classic.
uuid: d17168a8-4776-4761-b022-8258d5997604
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: d263f041-5a0d-4c4f-9266-aeff51a5a7e2
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
---
# Create template parameters{#creating-template-parameters}

Parameters enable you to use templates with maximum flexibility; they allow you to dynamically customize a template image. You can decide which text and image layers to include in the template, and in each layer, which parameters to display. For example, to draw attention to a product that is on sale, you can create an On Sale text layer. Later, you can remove this layer but still retain the rest of the template image by removing the On Sale parameter.

When you create template parameters, you in effect declare which parts of the template to call in a URL string. A URL constructed with parameters exposes those items in the URL string. With parameters exposed, you can create custom results from the way the template image is dynamically constructed from the Image Server. In this way, you can change a template dynamically because you can call some or all of its parameters in a URL.

In text layer parameters, you can also make the text string a dynamic field linked to values in a database. Being able to link text to a database is useful, for example, in promotions. You can customize template images to make them show client or customer names. You can also link a text layer parameter to a prices database to show the price of an item in a template image.

You can refer to a parameter more than once. Use the combo box for each command in the parameter dialog box to select any parameter that matches that particular command. For example, all size parameters are available for the `size=` command. You can reassign the parameter reference to any parameter already in the combo box, and rename to something not in the combo box. In the latter case, the name must be unique. Otherwise, an error states that the parameter exists. When you delete a parameter reference, the parameter is removed from the URL if it is not referenced anywhere else. When you change the default value for a text parameter, all references to that parameter update. You can see the update in the layer table, in the rendering of the template, and in the URL. When you change a layer attribute by manipulating resize handles or typing in values in the property panel, the parameter value is updated and all references to the parameter update. For example, if you have parameterized the size of two layers using one parameter, both layer sizes update when either of the layer sizes are changed. When you preview a template and change a parameter, all references to that parameter are updated.

See also [Template Basics](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) training video.

## Parameterize a layer {#parameterizing-a-layer}

For each layer in your template, follow these steps to create template parameters:

1. In the Layers list, select the Parameters button next to the name of the layer you want to create parameters for. The Parameters screen opens. It lists the names of each parameter on the layer, its value, and its type.
1. Select the On option beside the name of each parameter you want to include in the template image.
1. Select **[!UICONTROL Close]** to exit the Parameters screen.

>[!NOTE]
>
>You can rename parameters in the Parameters screen. Renaming a parameter makes the parameter easier to identify in URL strings and easier to use as a database value. To rename a parameter, select its **[!UICONTROL On]** option, select its name, and enter a new name in the Name field.

To see a list of the parameters you have created for your template, select the Parameter Summary button on the Template screen. The Parameter Summary screen opens. It lists the name of each layer, and if you have created parameters for a layer, the parameter names and values.

## Create dynamic text parameters {#creating-dynamic-text-parameters}

For text layers, you can also make the text string a dynamic field linked to a database value. Follow these steps:

1. On the Template screen, select the Parameters button next to the name of the text layer for which you want to create dynamic text parameters. The Parameters page opens.
1. Select the **[!UICONTROL On]** option next to the name of the text attribute (textAttr).
1. Select the **[!UICONTROL Text]** tab in the Parameters screen.
1. Select **[!UICONTROL Add Parameter]**. A default parameter name appears. You can replace this name by selecting it and typing over it. The current text string becomes the new name of the parameter. 
1. Select **[!UICONTROL Close]** to close the Parameters page.

To make the parameter name use a database value, append the following string to the Template URL:

```as3
?$_2(parameter name)=(database value)
```

The parameter name is replaced by names in a database field or Java™ code indicating, for example, the current price of an item or a customer name.
