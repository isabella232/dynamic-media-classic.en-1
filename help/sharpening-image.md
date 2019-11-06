---
title: Sharpening an image
seo-title: Sharpening an image
description: null
seo-description: Learn how to sharpen an image.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409

---

# Sharpening an image {#sharpening-an-image}

Sharpening is an image-manipulation technique for making the outlines of a digital image look more distinct. Sharpening increases the contrast between edge pixels and emphasizes the transition between dark and light areas. Sharpening increases local contrast and brings out fine detail. There is no strict formula for correctly sharpening all images. Too little sharpening can make for a soft image, but over-sharpening adds halos, artifacts, and noise.

Dynamic Media Classic highly recommends using Image Presets for all images. This ensures a uniform size, and sharpening is enforced on any image called with an Image Preset. Furthermore, you can edit and change an Image Preset’s sharpening parameters quite easily. The next time you publish, all images called with that preset are given the new values.

Dynamic Media Classic also recommends adding sharpening to Viewer Presets, and then calling a viewer with that preset. This ensures that images within your viewers are crisp and appealing.

However, whether you use Image Presets and Viewer Presets, or some alternate method of sharpening, the bottom line is that you should sharpen your images. If you do not, your images (and website) might look soft and fuzzy.

>[!NOTE]
>
>The Sharpen commands override Image Preset settings, including their sharpening effects. An Image Preset governs the size and formatting with which images are delivered from Dynamic Media Image Servers. Dynamic Media Classic highly recommends using Image Presets to deliver all images to make sure that images are delivered at a uniform size and sharpening. After the sharpening settings of an individual image have been changed, however, Image Preset sharpening settings no longer apply to the image. It is delivered without Image Preset sharpening settings.

It is often necessary to sharpen images. Dynamic Media Classic SPS and Image Servers offer several sharpening options. It is important to understand what sharpening does to an image and how much sharpening you need. Most images need some sharpening but the amount required depends upon the image.

Image sharpening increases the contrast of pixels to create the effect of accentuating edges. Humans perceive this enhanced edge contrast as sharpness. Although it is easy to enhance an image by running sharpening filters on an image, it is also easy to over-sharpen an image.

Over sharpening an image creates a halo effect, or banding of the edge’s lines.

There are best practices you can follow to optimize the sharpening of your images in Scene7 Publishing System and on Dynamic Media Image Server.

See [Best practices for sharpening images in Scene7 Publishing System and on Dynamic Media Image Server](/help/assets/s7_sharpening_images.pdf).

**To sharpen an image**

To sharpen an image, click its rollover **Edit** button and choose Sharpen, or open it in the Browse Panel in Detail view, then click **Sharpen**. The Sharpness Editor screen opens with sharpening commands. Choose commands and click **Save**.

>[!NOTE]
>
>Before sharpening an image, you can select the Apply Preset menu and choose an Image Preset to see what its sharpening effects are. The sharpening effects of an Image Preset may be suitable for your image. The Apply Preset menu is located on the bottom of the Sharpness Editor screen.

**Sharpening options**

The following table shows the Image Server sharpening options.

|Name|URL Protocol|Values|Example|
|--- |--- |--- |--- |
|Simple Sharpening|op_sharpen|`0 | 1`|op_sharpen=1|
|Resample Mode|resMode|`bilin | bicub | sharp2 | trilin`<br><br>bilin: Selects standard bi-linear interpolation. Fastest resampling method; some aliasing artifacts may be noticeable.<br>bicub: Selects bi-cubic interpolation. More CPU-intensive than bilin, but yields sharper images with less noticeable aliasing artifacts.<br><br>sharp2: Selects a modified Lanczos Window function as an interpolation algorithm. May produce slightly sharper results than bi-cubic at a higher CPU cost.<br><br>trilin: Selects a modified trilinear interpolation, which uses both higher and lower resolutions, if available. Recommended only when aliasing is an issue. Reduces JPEG sizes due to reduced high frequency data.|resMode=sharp2|
|Unsharp Mask|op_usm|amount, radius, threshold, monochrome<br><br>amount: filter strength factor (real 0…5)<br><br>radius: filter kernel radius in pixels (real 0…250) <br><br>threshold: filter threshold level (int 0…255)<br><br>monochrome: set to 0 to unsharp-mask each color component separately, set to 1 to unsharp-mask image brightness (intensity)|op_usm=1,1,10,0|

Select the Sharpening menu and choose an option:

**None** Disables sharpening.

**Sharpen** Runs a simple sharpening pass on the file after it is resized. This is similar to the “Sharpen” filter in Photoshop and does support any user parameters. Normally, you would use this filter or Unsharp Mask but not both. As a best practice, this method is not recommended, but it can help compensate for blurriness. (URL: op_sharpen)

**Unsharp Mask** Allows you to fine-tune a sharpening filter effect on the final downsampled image. You can control intensity of effect, radius of the effect (measured in pixels) and a threshold of contrast that will be ignored. This effect uses the same options as Photoshop’s “Unsharp Mask” filter. (URL: op_usm)

Choose these options to fine-tune sharpening with Unsharp Mask:

**Amount** Controls the amount of contrast applied to edge pixels. The default is 0.0. For high-resolution images, you can increase it to as high as 5.0. Think of Amount as a measure of filter intensity. Be aware that the Amount setting in Dynamic Media Classic is not the same as the Amount setting in Photoshop. Photoshop uses an amount in the range of 1% to 500%, whereas Dynamic Media Classic scales from 0.0 to 5.0. (5.0 is roughly equivalent to 500% in Photoshop, 0.9 is similar to 90%, and so on.)

**Radius** Determines the number of pixels surrounding the edge pixels that affect the sharpening. The effect runs on all pixels in the image and radiates in all directions.

The best radius value depends on the size of the image. A low value sharpens only the edge pixels. A high value sharpens a wider band of pixels.

For example, to get a similar sharpening effect for a 2000 x 2000 pixel image and 500x 500 pixel image, you might set a radius value of two pixels on the 2000 x 2000 pixel image. Then, set a radius value of one pixel on the 500 x 500 pixel image (a larger value for an image with more pixels).

**Threshold** Determines the range of contrast to ignore when the unsharp mask filter is applied. This option determines how different the sharpened pixels must be from the surrounding area before they are considered edge pixels and are sharpened.

Threshold uses a value from 0-255, which is the number of brightness steps in a grayscale image. 0=black, 128=50% gray and 255=white. For example, a threshold value of 12 ignores slight variations is skin tone brightness, so as not to add noise, while still adding edge contrast to contrasty areas, such as where eyelashes meet skin.

As an example, suppose you have a photo of someone’s face. The Unsharp Mask affects the parts of the image with the most contrast and the smooth skin itself. Even the smoothest skin exhibits subtle changes in brightness values. If you do not use a threshold value, the filter accentuates these subtle changes in skin pixels, creating a noisy effect (probably undesirable) while also increasing the contrast on the eyelashes, enhancing sharpness (probably desirable). To avoid this issue, use a threshold value that tells the filter to ignore pixels that do not change contrast dramatically, like smooth skin. To avoid introducing noise or posterization--in images with flesh tones, for example--try experimenting with Threshold values between 2 and 20. The default Threshold value of 0 sharpens all pixels in the image.

**Apply To** Choose Each Color to apply sharpening separately to each color component; choose Brightness to apply to sharpening to image brightness areas.

**Resampling**

Select the Resampling menu and choose an option. These options sharpen the image when it is downsampled:

**None** Turns off resampling.

**Bilinear** The fastest resampling method; some aliasing artifacts are noticeable.

**Bicubic** Increases CPU usage on the Image Server, but yields sharper images with less noticeable aliasing artifacts.

**Sharpen2** May produce slightly sharper results than the Bicubic option, but at even higher CPU cost on the Image Server.

**Trilinear** Uses both higher and lower resolutions if available; recommended only when aliasing is an issue. This method reduces JPEG size due to reduced high-frequency data.

**Sharpening and image presets**

You could mix all three sharpening effects to achieve your final result. However, this is not recommended. Dynamic Media Classic recommends you save your sharpening effects as part of an Image Preset.Image Presets allow you to package the most often used image modifiers to create a dynamically resized image in a small text string. An Image Preset contains values for the file format (usually JPEG for the web), pixel count and image sharpening. Instead of appending the URL with each image modifier needed to create a specific type of image size, you create a named Image Preset, such as “thumbnail,” configure the thumbnail Image Preset with the appropriate size, file format, and sharpening options, and then call the image using the Image Preset name. Image Presets shorten the length of the overall URL.These two URLs produce the same 350x350 JPEG image with sharpening:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Image Presets can be changed and updated at any time. You will see the results of a change to an Image Preset after you publish and after the cache for the URL clears.

If you use one preset for every image in a size category, any Company Administrator can update the definition of that Image Preset, republish, and affect every image using that format, without changing any web code. As a best practice, use one Image Preset per unique size on your site. To add an image preset, go to Setup &gt; Application Settings &gt; Image Presets. Then, Add or Edit an existing preset. The only required field is the name of the preset itself. However, you should include some level of sharpening in every preset.

**JPG Quality**

The JPG Quality options control the JPG compression level:

**JPG Quality** Select this option if you want to control compression levels and chrominance downsampling.

**Slider** Determines the JPG compression level. This setting affects both file size and image quality. The JPG quality scale is 1-100.

**Enable JPG Chrominance Downsampling** Because the eye is less sensitive to high-frequency color information than high-frequency luminance, JPEG images divide image information into luminance and color components. When a JPEG image is compressed, the luminance component is left at full resolution, while the color components are downsampled by averaging together groups of pixels. Downsampling reduces the data volume by one half or one third with almost no impact on perceived quality. Downsampling is not applicable to grayscale images. This technique reduces the amount of compression useful for images with high contrast (for example, images with overlaid text).

**Setting company-wide sharpening options**

If you do not use an Image Preset or pass specific Image Server sharpening protocols along the URL string, then your image is not sharpened when it is downsampled. However, you may set default sharpening values if this occurs and then any image will always have some sharpening.

To set your company’s default sharpening options, go to Setup &gt; Application Setup &gt; Publish Setup &gt; Image Server. If you set the Default Resampling Mode to Sharp2, it will always sharpen the image when downsampling.

**Adding sharpening to viewer presets**

Unless you add sharpening image modifiers to the preset, the small initial load image can look soft because it is downsampled to fit into the viewer window without being sharpened.

In SPS, Viewer Presets (like Image Presets) allow you to centralize many options into one location, including choice of skin and viewer options (such as including a Print button or controlling the speed of the zoom animation). Viewer Presets are found in the same section as Image Presets, under Setup &gt; Application Settings &gt; Viewer Presets.

The Modifiers option is found under the Core Settings section of all eCatalog, Spin, and Custom Zoom Viewer Presets. By adding the URL sharpening commands to the Modifiers box, you add sharpening every time that viewer is called with that viewer preset.

To call the Viewer Preset, use the config= command on the viewer URL. Here is an example of calling an Image Set (shoes) with a Viewer Preset (FantasticoZoom2009):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2009`

The preset here sharpens and changes the default skin of the viewer.

**Creating image-specific overrides**

The last, and least recommended, sharpening method is to create sharpening overrides on an image-by-image basis. This overrides the sharpening in an Image Preset with its own specific values. However, this overrides all other sharpening methods at any size. The best use case for this method is if some of your images are not high resolution, and the values in the Image Presets are too high for these small images. In this case, some per-image sharpening might be needed.

In SPS, select any image, go to the Detail View (by double-clicking or pressing the Detail View button), and click Sharpen. Change any parameter, then click Save. This tells the Image Server to use these sharpening parameters rather than any command you call in the URL, such as a sharpening modifier or Image Preset. You must publish to see the changes take effect.
