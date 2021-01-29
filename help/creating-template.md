---
title: Creating a template
description: Learn how to create a template in Dynamic Media Classic.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648

---

# Creating a template {#creating-a-template}

To create a template, click Build > Template Basics. Select either Designer or Developer. On this page, you can add image and text layers. You can also reorder layers, change the size and position of layers, and apply shadow and glow effects to images and text.

>[!NOTE]
>
>If you edit a template created in an earlier version of Dynamic Media Classic, you may receive the a prompt upon saving asking “Do you want to add a canvas layer?” Choose No to avoid adding a new base layer. If you accidentally choose Yes, delete the “&allowCanvasPrompt” and “&layer=0” modifiers in the URL and press Enter or Return.

## Creating the initial template {#creating-the-initial-template}

When you create a template set, the **Publish after save** option affects the set and set members in the following ways:

|“Publish after save” option selected before saving?|State of set after saving|State of set members after saving|
|--- |--- |--- |
|Yes|Published|Published|
|No|Unpublished|Set members retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

You can create a template from an existing template. Open the template, click **Save As**, and enter a new name in the Save As dialog box.

**To create the initial Temple Set**

1. To create your template use one of the following methods:

   **Select the PSD or images first** In the Browse Panel, select the PSD file or images you want for your template, click Build > Template Basics.

   **Start from the Template screen** Click Build > Template Basics. Select either Designer or Developer.

1. In the Enter Canvas Size dialog box, enter width and height measurements for your template.
1. Select a folder in the Asset Library and drag the PSD file or images you want for your template onto the Template screen.
1. When you are finished, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Save**.
1. Select a folder for storing your template, enter a name for the template, and click **Submit**.

   Dynamic Media Classic shrinks images if necessary to fit them on the canvas, the area on the Template screen for defining your template.

## Editing a Template Set {#editing-a-template-set}

Depending on whether you edit a published set or an unpublished template set, the **Publish after save** option affects the set and set members in the following ways:

|Set already published?|“Publish after save” option selected before saving your edit?|State of set after saving|State of set members after saving|
|--- |--- |--- |--- |
|Yes|Yes|Published|Published|
|Yes|No|Published|Existing set members retain their published state.Any new set members that you added during your edit retain their published or unpublished state.|
|No|Yes|Published|Published|
|No|No|Unpublished|Existing set members and any new set members that you added during your edit retain their published or unpublished state.|

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To edit a Template Set**

1. In the Grid view, browse to an Template Set, and then below the image, click **Edit**.
1. Make changes to the template as necessary.
1. When you are finished editing, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Save**, select a storage folder, enter a name for the set, and then click **Save**.

## Deleting a Template {#deleting-a-template}

When you delete a Template set, the set itself is moved to the Trash. However, the members (or “children”) within that set are not affected; instead, they each retain their existing published or unpublished state.

See also [Manually publishing assets](publishing-files.md#manually_publishing_assets) and [Manually unpublishing assets](publishing-files.md#manually_unpublishing_assets).

**To delete a Template**

1. In the Grid View, List View, or Details View, select one or more Templates.
1. On the Global Navigation Bar, click **File** > **Delete** > **Delete**.

## Understanding the Template screen {#understanding-the-template-screen}

The Template screen offers tools for manipulating and parameterizing layers.

Use these tools on the Template screen to create templates:

**Pan tool** Allows you to select layers, move them around the canvas, resize them, or rotate them.

**Text tool** Creates a text layer. Drag on the canvas to create a text layer, and then enter the text in the layer. See Create a text layer.

**Preview button** Opens the Preview screen and shows the template in a Zoom Viewer. You see what the template looks like to users on your web site or application.

**Parameter Summary button** Opens the Parameter Summary screen. You can see the name of each layer in a template, and on each layer, the names of parameters that have been activated.

**Text Editor v4.3 and Text Editor v4.2** You can choose to use the latest and most fully featured text editor, Text Editor v4.3, or the previous text editor, Text Editor v4.2. When creating new templates, Text Editor v4.3 is selected by default. When editing older templates, Text Editor v4.2 is selected by default. Text Editor v4.3 does not currently support word wrap, so when editing older templates that use word wrap, use Text Editor v4.2 to keep the template’s fidelity fully intact. If your older template does not use word wrap, you can choose Text Editor v4.3 to take advantage of the many new features it offers such as Increase Margins, Decrease Margins, Set Text In All Caps, and Copy Fit Text.

***note**: Text Editor v4.2 will eventually be removed as an option in Dynamic Media Classic, so it is recommended that you use Text Editor 4.3 when possible. The Word Wrap option will be incorporated into a future release of the Text Editor.*

**Designer and Developer** Select the option that best describes your role.

**Canvas** Defines the total available area, in pixels, for defining your template. The default size is 300 x 300 pixels. Layers are placed on the canvas.

**Layers list** Lists the name of layers in the template. To select a layer, select its name in the Layers list. The Layers list offers tools for adding effects to layers, deleting layers, reordering layers, and parameterizing layers. See Working with layers.

**Layer Properties area** Offers tools for changing the background color, opacity, size, and position of a layer, as well as the background color, opacity, and size of the canvas. You can also adjust shadow and glow effects. See Working with layers.

## Creating image layers {#creating-image-layers}

1. Drag the image from the Asset Library to the canvas.

   The ID name of the image appears in the Layers list.

>[!NOTE]
>
>If necessary, Dynamic Media Classic shrinks images to make them fit in the canvas when you create an image layer.

## Creating a text layer {#creating-a-text-layer}

1. Click the Text tool.
1. Drag to create a text box on the canvas or on an image. 
1. In the Text screen that opens, add text by doing any of the following on the Preview tab:

    * Type text in the text box. Choose Copy Fit Text to make the text fit n the text box.
    * Paste text from the Clipboard into the text box.

1. Click Apply, and then close the Text screen.

### Format text {#format-text}

Follow these steps to format text in a text layer:

1. In the Layers list, double-click the name of the text box with text you want to edit. The Text Editor opens.
1. In the text box, select the text you want to format. You can select all the text, portions of the text, as well as individual characters.
1. Specify any of these formatting options, and then click Apply.

   **Font** Choose a font on the Font menu. If a font you want does not appear on the menu, you can upload it into the Dynamic Media Classic. See Fonts.

   **Font Size** Choose a font size from the menu, type a specific size in the box, or click the up or down arrows to increase or decrease the size by two points.

   **Color** Click to choose a color for text.

   **Bold, Italic, or Underline** Select the text, and then click the icon for the type of formatting you want to apply to the text.

   **All Caps, Superscript, or Subscript** Select the text, and then click the icon for the type of formatting you want to apply to the text.

   **Alignment** Choose an Alignment button to left-align, center, or right-align text in the text layer.

   **Tracking** Type or select a numeric value by which to adjust the amount of space between words.

   **Kerning** Type or select a numeric value by which to adjust the amount of space between characters.

   **Line Spacing** Type or select a numeric value by which to adjust the amount of space between lines.

   **Baseline Shift** Type or select a numeric value by which to move a selected character up or down relative to the baseline of the surrounding text. This option is especially useful when you’re hand-setting fractions or adjusting the position of inline graphics.

>[!NOTE]
>
>Click Undo to reverse your last action. Click Redo if you change your mind about reversing an action after you click Undo.

### Format paragraphs {#format-paragraphs}

1. In the Layers list, double-click the name of the text box with text you want to edit. The Text Editor opens.
1. Select the paragraph you want to format. 
1. Specify any of these formatting options, and then click Apply.

   **Alignment** Click to specify the type of alignment: align left, align center, align right, or justify.

   **End of Paragraph Justification** Click to specify the type of justification for the last line in the paragraph: last line aligns left; last line aligns center; and last line aligns right.

   **Line Spacing** Type or select a numeric value by which to adjust the amount of space between all the lines in the paragraph.

   **Indent All** Click to increase the amount the text is indented.

   **Remove Indent** Click to decrease the amount the text is indented.

   **Indent First Line** Specify the amount by which you want to indent the first line of text.

   **Space Before Paragraph** Specify the amount of space you want to appear above the first line of text in the paragraph.

   **Space After Paragraph** Specify the amount of space you want to appear below the last line of text in the paragraph.

   **Vertical Align** Select where you want the text to appear vertically within the text box: Top, Middle, Bottom.

   **Text Direction** Select the direction in which you want the text to display: Right-To-Left or Left-To-Right.

### Adjust text layer properties {#adjust-text-layer-properties}

1. In the Template Basics screen, select the text box you want to adjust.
1. In the Layer Properties panel, select any of the following:

   **Shrink Text (Text Editor v4.2 only)** Select to shrink the text to fit within the text box.

   **Word Wrap (Text Editor v4.2 only)** Select a wrap option to specify if or how the text wraps:

   **Wrap** Wraps the text to fit into a text box that is too small horizontally.

   **No Wrap** Does not wrap the text when the text box is too small horizontally, and instead, cuts off a portion of the text.

   **NB Wrap** (Nonbreaking wrap) Wraps text to fit into a textbox, and does not break words.

   **Position** Specifies the location of the text box on the canvas.

   **Padding** Adds margins or crops the layer rectangle. Specify the number of pixels to add or remove for Left, Top, Bottom, and Right. Enter positive numbers to add a margin; enter negative numbers to crop.

### View and edit text source code {#view-and-edit-text-source-code}

The information provided in Source tab of the Text Editor is for your reference. Edit the text only if you are familiar with editing source code.

1. In the Layers list, double-click the name of the text box with text you want to edit. The Text Editor opens.
1. Click the Source tab in the Text Editor to reveal the source code for the text.
1. View or edit the text as desired.

   Changes remain intact if you switch back and forth between Preview and Source view. 

1. Click Apply to render the edits.

## Working with layers {#working-with-layers}

Use the Layers list and Layer Properties area to work with layers. You can reorder layers, change their size and position, rotate layers, and determine the background color, foreground color, opacity, and blend mode of a layer.

You can also change the size of the canvas, choose its background color, and change its opacity setting.

### Reordering layers {#reordering-layers}

Changing layer order can effect appearance, especially when transparency or overprinting is involved. Be sure to preview the outcome before committing your changes.

1. Use one of these techniques to reorder the layers in a template:

    * Select a layer in the Layers list. Then click the Up or Down button as many times as necessary to place it in the correct position in the list.
    * Drag a layer up or down in the Layers list.

### Changing the size and position of layers and the canvas {#changing-the-size-and-position-of-layers-and-the-canvas}

Layers must be small enough to fit on the canvas. You can change the size of a layer or the canvas manually or by entering size measurements. You can change the position of a layer manually or by entering offset measurements. You can also rotate a layer.

>[!NOTE]
>
>Dynamic Media Classic recommends creating an Image Preset that is the exact size of your template. Matching the Image Preset size to the template size ensures that the final output size and sharpening options for the template are set correctly. After you’ve created this Image Preset, you can choose it from the Apply Preset menu on the Template Preview screen. The screen shows you what the image looks like when it is delivered from the server. See [Setting up Image Presets](setting-image-presets.md#setting_up_image_presets).

**Changing the size of a layer**

To change the size of a layer or the canvas, select the layer or canvas on the Layers list and use one of these techniques:

**Manually changing size** Select and drag a corner of the layer or canvas. With text layers, you can also drag a side of the layer. Hold down the Shift key as you drag to change size but maintain the aspect ratio (the shape).

**Entering layer size measurements** Enter pixel measurements in the W (Width) and H (Height) text boxes in the Layer Properties area.

Beside changing the size of a layer, you can pad it. To do so, enter a Padding measurement in the Left, Right, Top, and Bottom box of the Layer Properties area. Padding adds a margin to the current layer to offset it from the perimeter of its base layer. Padding is useful if you add a drop shadow or outer glow effect and you want to make the effect more visible. Padding increases the size of a layer and displays its background color in the extended, padded area. The base layer repositions itself relative to the new size of the layer. For example, if the current layer is centered on the base layer, extending the left side of the layer moves it further to the right of the base layer.

**Changing the position of a layer**

To change the position of a layer on the canvas, select its name in the Layers list and use one of these techniques:

**Manually&#xA;changing position** Move the pointer near to but not over a layer boundary, and when you see the four-headed arrow cursor, click and start dragging.

**Entering position offset measurements** Enter X and Y offset measurements in the X and Y text boxes. These measurements represent the x, y offset of the anchor point in pixels.

**Rotating a layer**

The Rotate box lists the angle to which the layer was rotated. To rotate a layer, select its name in the Layers list and use one of these techniques:

**Manually rotating** Move the cursor near to but not over a corner of the layer. When you see the rotation cursor, drag the corner of the layer. Hold down the Shift key as you drag to rotate by 15-degree increments.

**Entering a degree measurement** Enter the number of degrees to rotate the layer. Rotation is clockwise; to rotate in a counterclockwise fashion, enter a negative number.

**Hiding a layer or a layer effect**

You can hide a layer or layer effect by clicking the eye icon next to a layer name or effect name. Hidden layers do not appear in previews or output. The layer information is not deleted from the URL. Instead, “hide=1” is added to the URL to note that the layer is currently hidden from view. For example:

layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode

layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode

### Determining the background color, opacity, and blend mode {#determining-the-background-color-opacity-and-blend-mode}

To choose a background color, opacity, and blend mode for a layer or the canvas, select the layer or canvas and use these techniques:

**Foreground color** Click the Foreground Color button and choose a color swatch to change the color of the shadow or glow. You can also enter a color-value parameter in the box. The background color applies only to layers that use transparency. For example, it applies to a partially transparent layer in a price tag or the background of a text field. Layers that consist of a PSD, TIFF or PNG image with transparency turned on can have transparent backgrounds.

**Background color** Click the Background Color button and choose a color swatch to change the color of the padded areas.

**Opacity** Drag the Opacity slider to make any layer translucent so that part of the underlying image shows through. The 100-percent setting is completely opaque; the 0 setting is transparent.

**Blend mode** Choose an option to simulate one of the blend modes available in Photoshop. The options are Normal, Dissolve, Lighten, Darken, Multiply, and Screen. These options are available for layers, not the canvas.

## Using shadow and glow effects on layers {#using-shadow-and-glow-effects-on-layers}

You can apply a shadow or glow to a layer. The shadow or glow is applied to the perimeter of the layer and extends inward or outward, depending on the shadow or glow option you choose. If your template originated with a PSD file with shadow and glow effects, you can adjust these effects in Dynamic Media Classic.

After you apply a shadow or glow effect, you can adjust its size, color, opacity, and position in the Layer Properties area of the Template screen.

### Applying a shadow or glow effect to a layer {#applying-a-shadow-or-glow-effect-to-a-layer}

To apply a shadow or glow effect:

1. Select a layer in the Layers list.
1. Select the Add Effect menu and choose an option:

   **Drop Shadow** Applies a shadow to the bottom and right side of the layer.

   **Inner Shadow** Applies a shadow effect inside all edges of the layer.

   **Outer Glow** Applies a glow effect around all edges of the layer.

   **Inner Glow** Applies a glow effect inside all edges of the layer.

An effect name appears on the Layers list after you apply an effect. To delete an effect, select its name on the Layers list and then select the Delete button.

>[!NOTE]
>
>You sometimes can’t see the effect of a drop shadow or outer glow if the underlying layer is not large enough to display it. If you can’t see the shadow or glow, consider adding Padding values to the layer or reordering the layer. See [Changing the size and position of layers and the canvas](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas)and [Reordering layers](creating-template.md#reordering_layers).

### Adjusting a shadow or glow effect {#adjusting-a-shadow-or-glow-effect}

To adjust a shadow or glow effect, start by selecting its name in the Layers list. Then change its settings in the Layer Properties area of the Template screen:

**Color** Select the Color button and choose a color swatch to change the color of the shadow or glow. You can also enter a color-value parameter in the box.

**Opacity** Drag the slider to determine how intense the effect is. Less opaque effects are more transparent.

**Blend Mode** Choose an option to simulate one of the blend modes available in Photoshop. The options are Normal, Dissolve, Lighten, Darken, Multiply, and Screen.

**Size** Enter measurements in the X and Y box to enlarge or shrink the shadow effect. Size options are only available for inner shadows and drop shadows.

**Grow** Drag the slider to extend the effect inward or outward.

**Blur** Drag the slider to control feathering at the edges of the effect. Effects with more blur are more feathered.

## Masking layers {#masking-layers}

The Layers list offers a Mask button that specifies how the mask or alpha channel of a layer is used. Using the Mask button, you can apply the effect of a background layer to a particular layer or the entire parent layer in your template. Select a layer in the Layers list and select the Mask button to cycle through these states:

* The background of the layer is opaque.
* The layer content is inverted and the background of the layer is filled with solid black. 
* The background of the layer is filled with solid black.

