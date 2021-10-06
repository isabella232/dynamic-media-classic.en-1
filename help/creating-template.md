---
title: Create a template
description: Learn how to create a template in Adobe Dynamic Media Classic.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
---
# Create a template {#creating-a-template}

To create a template, go to **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. Select either Designer or Developer. On this page, you can add image and text layers. You can also reorder layers, change the size and position of layers, and apply shadow and glow effects to images and text.

See also [Template Basics](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) training video.

>[!NOTE]
>
>If you edit a template created in an earlier version of Adobe Dynamic Media Classic, a prompt asks you upon saving “Do you want to add a canvas layer?”. Select **[!UICONTROL No]** to avoid adding a base layer. If you accidentally select **[!UICONTROL Yes]**, delete the `&allowCanvasPrompt` and `&layer=0` modifiers in the URL and press **[!UICONTROL Enter]** or **[!UICONTROL Return]**.

## Create the initial template {#creating-the-initial-template}

When you create a template set, the **[!UICONTROL Publish after save]** option affects the set and set members in the following ways:

| **[!UICONTROL Publish after save]** option selected before saving? | State of set after saving | State of set members after saving |
| --- | --- | --- |
| Yes | Published | Published |
| No | Unpublished |Set members retain their published or unpublished state. |

See also [Manually publish assets](publishing-files.md#manually_publishing_assets) and [Manually unpublish assets](publishing-files.md#manually_unpublishing_assets).

You can create a template from an existing template. Open the template, select **[!UICONTROL Save As]**, and enter a new name in the Save As dialog box.

**To create the initial template:**

1. To create your initial template, use one of the following methods:

   * **Select the PSD or images first** - In the Browse Panel, select the PSD file or images you want for your template, go to **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**.

   * **Start from the Template screen** - Go to **[!UICONTROL Build]** > **[!UICONTROL Template Basics]**. Select either Designer or Developer.

1. In the Enter Canvas Size dialog box, enter width and height measurements for your template.
1. Select a folder in the Asset Library and drag the PSD file or images you want for your template onto the Template screen.
1. When you are finished, near the lower-right corner of the page, ensure that **[!UICONTROL Publish after save]** is selected (default).
1. Select **[!UICONTROL Save]**.
1. Select a folder for storing your template, enter a name for the template, and select **[!UICONTROL Submit]**.

   Adobe Dynamic Media Classic shrinks images if necessary to fit them on the canvas, the area on the Template screen for defining your template.

## Edit a template set {#editing-a-template-set}

Whether you edit a published set or an unpublished template set, the **[!UICONTROL Publish after save]** option affects the set and set members in the following ways:

| Set already published? | **[!UICONTROL Publish after save]** option selected before saving your edit? | State of set after saving | State of set members after saving |
| --- | --- | --- | --- |
| Yes | Yes | Published | Published |
| Yes | No | Published | Existing set members retain their published state. Any new set members that you added during your edit retain their published or unpublished state. |
| No | Yes | Published | Published |
| No | No | Unpublished | Existing set members and any new set members that you added during your edit retain their published or unpublished state. |

See also [Manually publish assets](publishing-files.md#manually_publishing_assets) and [Manually unpublish assets](publishing-files.md#manually_unpublishing_assets).

**To edit a template set:**

1. In the Grid View, browse to a Template Set, and then below the image, select **[!UICONTROL Edit]**.
1. Change the template as necessary.
1. When you are finished editing, near the lower-right corner of the page, ensure that **[!UICONTROL Publish after save]** is selected (default).
1. Select **[!UICONTROL Save]**, select a storage folder, enter a name for the set, and then select **[!UICONTROL Save]**.

## Delete a Template {#deleting-a-template}

When you delete a Template set, the set itself is moved to the Trash. However, the members (or “children”) within that set are not affected; instead, they each retain their existing published or unpublished state.

See also [Manually publish assets](publishing-files.md#manually_publishing_assets) and [Manually unpublish assets](publishing-files.md#manually_unpublishing_assets).

**To delete a Template:**

1. In the Grid View, List View, or Details View, select one or more Templates.
1. On the Global Navigation Bar, go to **[!UICONTROL File]** > **[!UICONTROL Delete]** > **[!UICONTROL Delete]**.

## Understand the Template screen {#understanding-the-template-screen}

The Template screen offers tools for manipulating and parameterizing layers.

Use these tools on the Template screen so you can create templates:

* **[!UICONTROL Pan]** - Lets you select layers, move them around the canvas, resize them, or rotate them.

* **[!UICONTROL Text]** - Creates a text layer. Drag on the canvas to create a text layer, and then enter the text in the layer. See [Creating a text layer](#creating-a-text-layer).

* **[!UICONTROL Preview]** - Opens the Preview screen and shows the template in a Zoom Viewer. You see what the template looks like to users on your web site or application.

* **[!UICONTROL Parameter Summary]** Opens the Parameter Summary screen. You can see the name of each layer in a template, and on each layer, the names of parameters that have been activated.

* **[!UICONTROL Text Editor v4.3 and Text Editor v4.2]** - You can choose to use the latest and most fully featured text editor, Text Editor v4.3, or the previous text editor, Text Editor v4.2. When creating templates, Text Editor v4.3 is selected by default. When editing older templates, Text Editor v4.2 is selected by default. Text Editor v4.3 does not currently support word wrap, so when editing older templates that use word wrap, use Text Editor v4.2 to keep the template’s fidelity fully intact. If your older template does not use word wrap, you can choose Text Editor v4.3 to take advantage of the many new features it offers. For example, Increase Margins, Decrease Margins, Set Text In All Caps, and Copy Fit Text.

   >[!NOTE]
   >
   >Text Editor v4.2 is planned for removal as an option in Adobe Dynamic Media Classic, so it is recommended that you use Text Editor 4.3 when possible. The **[!UICONTROL Word Wrap]** option will be incorporated into a future release of the Text Editor.

* **[!UICONTROL Designer and Developer]** - Select the option that best describes your role.

* **[!UICONTROL Canvas]** - Defines the total available area, in pixels, for defining your template. The default size is 300 x 300 pixels. Layers are placed on the canvas.

* **[!UICONTROL Layers list]** - Lists the name of layers in the template. To select a layer, select its name in the Layers list. The Layers list offers tools for adding effects to layers, deleting layers, reordering layers, and parameterizing layers. See [Work with layers](#working-with-layers).

* **[!UICONTROL Layer Properties area]** - Offers tools for changing the background color, opacity, size, and position of a layer, as well as the background color, opacity, and size of the canvas. You can also adjust shadow and glow effects. See [Work with layers](#working-with-layers).

## Create image layers {#creating-image-layers}

1. Drag the image from the Asset Library to the canvas.

   The ID name of the image appears in the Layers list.

   >[!NOTE]
   >
   >If necessary, Adobe Dynamic Media Classic shrinks images to make them fit in the canvas when you create an image layer.

## Create a text layer {#creating-a-text-layer}

1. Select the **[!UICONTROL Text]** tool.
1. Drag to create a text box on the canvas or on an image. 
1. In the Text screen that opens, add text by doing any of the following on the Preview tab:

    * Type text in the text box. Choose Copy Fit Text to make the text fit n the text box.
    * Paste text from the Clipboard into the text box.

1. Select **[!UICONTROL Apply]**, and then close the Text screen.

### Format text {#format-text}

To format text in a text layer, do the following:

1. In the Layers list, double-click the name of the text box with text you want to edit. The Text Editor opens.
1. In the text box of the Text Editor, select the text you want to format. You can select all the text, portions of the text, or individual characters.
1. Specify any of the following formatting options, and then select **[!UICONTROL Apply]**.

   * **[!UICONTROL Font]** - Choose a font on the Font menu. If a font you want does not appear on the menu, you can upload it into the Adobe Dynamic Media Classic. See Fonts.

   * **[!UICONTROL Font Size]** - Choose a font size from the menu, type a specific size in the box, or select the **[!UICONTROL Up]** or **[!UICONTROL Down]** arrows to increase or decrease the size by two points.

   * **[!UICONTROL Color]** - Select to choose a color for text.

   * **[!UICONTROL Bold]**, **[!UICONTROL Italic]**, or **[!UICONTROL Underline]** - Select the text, and then select the icon for the type of formatting you want to apply to the text.

   * **[!UICONTROL All Caps]**, **[!UICONTROL Superscript]**, or **[!UICONTROL Subscript]** - Select the text, and then select the icon for the type of formatting you want to apply to the text.

   * **[!UICONTROL Alignment]** - Choose an Alignment button to left-align, center, or right-align text in the text layer.

   * **[!UICONTROL Tracking]** - Type or select a numeric value by which to adjust the amount of space between words.

   * **[!UICONTROL Kerning]** - Type or select a numeric value by which to adjust the amount of space between characters.

   * **[!UICONTROL Line Spacing]** - Type or select a numeric value by which to adjust the amount of space between lines.

   * **[!UICONTROL Baseline Shift]** - Type or select a numeric value by which to move a selected character up or down relative to the baseline of the surrounding text. This option is especially useful when you’re hand-setting fractions or adjusting the position of inline graphics.

>[!NOTE]
>
>Select **[!UICONTROL Undo]** if you want to reverse your last action. Select **[!UICONTROL Redo]** if you change your mind about reversing an action after you select **[!UICONTROL Undo]**.

### Format paragraphs {#format-paragraphs}

1. In the Layers list, double-click the name of the text box with text you want to edit. The Text Editor opens.
1. Select the paragraph you want to format.
1. Specify any of the following formatting options, and then select **[!UICONTROL Apply]**.

   * **[!UICONTROL Alignment]** - Select to specify the type of alignment: align left, align center, align right, or justify.

   * **[!UICONTROL End of Paragraph Justification]** - Select to specify the type of justification for the last line in the paragraph: last line aligns left; last line aligns center; and last line aligns right.

   * **[!UICONTROL Line Spacing]** - Type or select a numeric value by which to adjust the amount of space between all the lines in the paragraph.

   * **[!UICONTROL Indent All]** - Select to increase the amount the text is indented.

   * **[!UICONTROL Remove Indent]** - Select to decrease the amount the text is indented.

   * **[!UICONTROL Indent First Line]** - Specify the amount by which you want to indent the first line of text.

   * **[!UICONTROL Space Before Paragraph]** - Specify the amount of space you want to appear above the first line of text in the paragraph.

   * **[!UICONTROL Space After Paragraph]** - Specify the amount of space you want to appear below the last line of text in the paragraph.

   * **[!UICONTROL Vertical Align]** - Select where you want the text to appear vertically within the text box: Top, Middle, Bottom.

   * **[!UICONTROL Text Direction]** - Select the direction in which you want the text to display: Right-To-Left or Left-To-Right.

### Adjust text layer properties {#adjust-text-layer-properties}

1. In the Template Basics screen, select the text box you want to adjust.
1. In the Layer Properties panel, select any of the following:

   * **[!UICONTROL Shrink Text (Text Editor v4.2 only)]** - To fit within the text box, select to shrink the text.

   * **[!UICONTROL Word Wrap (Text Editor v4.2 only)]** - To specify if or how the text wraps, select a wrap option:

   * **[!UICONTROL Wrap]** - Wraps the text to fit into a text box that is too small horizontally.

   * **[!UICONTROL No Wrap]** - Does not wrap the text when the text box is too small horizontally, and instead, cuts off a portion of the text.

   * **[!UICONTROL Nonbreaking Wrap]** - Wraps text to fit into a textbox, and does not break words.

   * **[!UICONTROL Position]** - Specifies the location of the text box on the canvas.

   * **[!UICONTROL Padding]** - Adds margins or crops the layer rectangle. Specify the number of pixels that you want to add or remove for Left, Top, Bottom, and Right. Enter positive numbers if you want to add a margin or negative numbers to crop.

### View and edit text source code {#view-and-edit-text-source-code}

The information provided in Source tab of the Text Editor is for your reference. Edit the text only if you are familiar with editing source code.

1. In the Layers list, double-click the name of the text box with text you want to edit. The Text Editor opens.
1. In the Text Editor, to reveal the source code for the text, select the **[!UICONTROL Source]** tab in the Text Editor.
1. View or edit the text as desired.

   Changes remain intact if you switch back and forth between Preview and Source view.

1. Select **[!UICONTROL Apply]** to render the edits.

## Work with layers {#working-with-layers}

Use the Layers list and Layer Properties area to work with layers. You can reorder layers, change their size and position, rotate layers, and determine the background color, foreground color, opacity, and blend mode of a layer.

You can also change the size of the canvas, choose its background color, and change its opacity setting.

### Reorder layers {#reordering-layers}

Changing layer order can affect appearance, especially when transparency or overprinting is involved. Be sure to preview the outcome before committing your changes.

1. Use one of these techniques to reorder the layers in a template:

    * Select a layer in the Layers list. Then select **[!UICONTROL Up]** or **[!UICONTROL Down]** as many times as necessary to place it in the correct position in the list.
    * Drag a layer up or down in the Layers list.

### Change the size and position of layers and the canvas {#changing-the-size-and-position-of-layers-and-the-canvas}

Layers must be small enough to fit on the canvas. You can change the size of a layer or the canvas manually or by entering size measurements. You can change the position of a layer manually or by entering offset measurements. You can also rotate a layer.

>[!NOTE]
>
>Adobe Dynamic Media Classic recommends creating an Image Preset that is the exact size of your template. Matching the Image Preset size to the template size ensures that the final output size and sharpening options for the template are set correctly. After you’ve created this Image Preset, you can choose it from the Apply Preset menu on the Template Preview screen. The screen shows you what the image looks like when it is delivered from the server. See [Set up Image Presets](setting-image-presets.md#setting_up_image_presets).

* **Changing the size of a layer** - To change the size of a layer or the canvas, select the layer or canvas on the Layers list and use one of these techniques:

* **Manually changing size** - Select and drag a corner of the layer or canvas. With text layers, you can also drag a side of the layer. Hold down the Shift key as you drag to change size but maintain the aspect ratio (the shape).

* **Entering layer size measurements** - Enter pixel measurements in the W (Width) and H (Height) text boxes in the Layer Properties area.

Beside changing the size of a layer, you can pad it. To do so, enter a Padding measurement in the Left, Right, Top, and Bottom box of the Layer Properties area. Padding adds a margin to the current layer to offset it from the perimeter of its base layer. Padding is useful if you add a drop shadow or outer glow effect and you want to make the effect more visible. Padding increases the size of a layer and displays its background color in the extended, padded area. The base layer repositions itself relative to the new size of the layer. For example, if the current layer is centered on the base layer, extending the left side of the layer moves it further to the right of the base layer.

* **Changing the position of a layer** - To change the position of a layer on the canvas, select its name in the Layers list and use one of these techniques:

* **Manually changing position** - Move the pointer near to but not over a layer boundary, and when you see the four-headed arrow cursor, select and start dragging.

* **Entering position offset measurements** - Enter X and Y offset measurements in the X and Y text boxes. These measurements represent the x, y offset of the anchor point in pixels.

* **Rotating a layer** - The Rotate box lists the angle to which the layer was rotated. To rotate a layer, select its name in the Layers list and use one of these techniques:

* **Manually rotating** - Move the cursor near to but not over a corner of the layer. When you see the rotation cursor, drag the corner of the layer. Hold down the Shift key as you drag to rotate by 15-degree increments.

* **Entering a degree measurement** - Enter the number of degrees to rotate the layer. Rotation is clockwise; to rotate in a counterclockwise fashion, enter a negative number.

**Hide a layer or a layer effect:**

You can hide a layer or layer effect by selecting the eye icon next to a layer name or effect name. Hidden layers do not appear in previews or output. The layer information is not deleted from the URL. Instead, `hide=1` is added to the URL to note that the layer is hidden from view. For example:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Determine the background color, opacity, and blend mode {#determining-the-background-color-opacity-and-blend-mode}

To choose a background color, opacity, and blend mode for a layer or the canvas, select the layer or canvas and use these techniques:

* **Foreground color** - Select **[!UICONTROL Foreground Color]** and choose a color swatch to change the color of the shadow or glow. You can also enter a color-value parameter in the box. The background color applies only to layers that use transparency. For example, it applies to a partially transparent layer in a price tag or the background of a text field. Layers that consist of a PSD, TIFF or PNG image with transparency turned on can have transparent backgrounds.

* **Background color** - Select **[!UICONTROL Background Color]** and choose a color swatch to change the color of the padded areas.

* **Opacity** - Drag the Opacity slider to make any layer translucent so that part of the underlying image shows through. The 100-percent setting is opaque; 0 is transparent.

* **Blend mode** - To simulate one of the blend modes available in Photoshop, choose an option. The options are Normal, Dissolve, Lighten, Darken, Multiply, and Screen. These options are available for layers, not the canvas.

## Use shadow and glow effects on layers {#using-shadow-and-glow-effects-on-layers}

You can apply a shadow or glow to a layer. The shadow or glow is applied to the perimeter of the layer and extends inward or outward, depending on the shadow or glow option you choose. If your template originated with a PSD file with shadow and glow effects, you can adjust these effects in Adobe Dynamic Media Classic.

After you apply a shadow or glow effect, you can adjust its size, color, opacity, and position in the Layer Properties area of the Template screen.

### Apply a shadow or glow effect to a layer {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Select a layer in the Layers list.
1. Select the Add Effect menu and choose an option:

   * **[!UICONTROL Drop Shadow]** - Applies a shadow to the bottom and right side of the layer.

   * **[!UICONTROL Inner Shadow]** - Applies a shadow effect inside all edges of the layer.

   * **[!UICONTROL Outer Glow]** - Applies a glow effect around all edges of the layer.

   * **[!UICONTROL Inner Glow]** - Applies a glow effect inside all edges of the layer.

An effect name appears on the Layers list after you apply an effect. To delete an effect, select its name on the Layers list and then select **[!UICONTROL Delete]**.

>[!NOTE]
>
>You sometimes cannot see the effect of a drop shadow or outer glow if the underlying layer is not large enough to display it. If you cannot see the shadow or glow, consider adding Padding values to the layer or reordering the layer. See [Changing the size and position of layers and the canvas](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) and [Reordering layers](creating-template.md#reordering_layers).

### Adjust a shadow or glow effect {#adjusting-a-shadow-or-glow-effect}

To adjust a shadow or glow effect, start by selecting its name in the Layers list. Then change its settings in the Layer Properties area of the Template screen:

* **[!UICONTROL Color]** - Select the Color button and choose a color swatch to change the color of the shadow or glow. You can also enter a color-value parameter in the box.

* **[!UICONTROL Opacity]** - Drag the slider to determine how intense the effect is. Less opaque effects are more transparent.

* **[!UICONTROL Blend Mode]** - To simulate one of the blend modes available in Photoshop, choose an option. The options are Normal, Dissolve, Lighten, Darken, Multiply, and Screen.

* **[!UICONTROL Size]** - Enter measurements in the X and Y box to enlarge or shrink the shadow effect. Size options are only available for inner shadows and drop shadows.

* **[!UICONTROL Grow]** - Drag the slider to extend the effect inward or outward.

* **[!UICONTROL Blur]** - Drag the slider to control feathering at the edges of the effect. Effects with more blur are more feathered.

## Mask layers {#masking-layers}

The Layers list offers a Mask button that specifies how the mask or alpha channel of a layer is used. Using the Mask button, you can apply the effect of a background layer to a particular layer or the entire parent layer in your template. Select a layer in the Layers list and select **[!UICONTROL Mask]** to cycle through these states:

* The background of the layer is opaque.
* The layer content is inverted and the background of the layer is filled with solid black. 
* The background of the layer is filled with solid black.
