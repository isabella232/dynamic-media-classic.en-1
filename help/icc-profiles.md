---
title: ICC profiles
seo-title: ICC profiles
description: null
seo-description: Learn about ICC profiles.
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0

---

# ICC profiles{#icc-profiles}

An ICC (International Color Consortium) profile is a file that describes how to correctly convert image files from one color space to another. ICC profiles help you to get the correct colors for your images. For example, to correctly display images designed for printing on a computer monitor, you can choose an ICC profile. This profile converts the image to a different color space and makes sure that the colors display correctly online.

In the Scene7 Publishing System, you can choose an ICC profile to convert images to a different color space when you upload the images. All standard Photoshop ICC profiles are available by default on SPS. To see the names of color profiles on the Upload screen, select the Color Profile menu. Then choose Custom From &gt; To, and choose an ICC profile name on the Converted From and Converted To menus. See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload).

As well as using the default ICC profiles, you can upload other ICC profiles to SPS and make them available for color space conversion. Switch to Detail view in the Browse Panel to investigate the profile class, color space type, and PCS type of an ICC profile.

## Uploading ICC profiles {#uploading-icc-profiles}

Upload ICC profiles with the same techniques you use to upload files. You can store ICC profiles in any SPS folder. See [Uploading your files](uploading-files.md#uploading_your_files).

## Examining an ICC profile {#examining-an-icc-profile}

To examine an ICC profile, select it in the Browse Panel and display it in Detail view. Detail view provides this information about ICC profiles:

**Profile Class** The ICC (International Color Consortium) defines each class to cover a type of application. For example, Input profiles apply to devices such as digital cameras and scanners, and Output profiles apply to printers.

**Color Space Type** This number is the "input" color space of the profile, as defined by the ICC. The color space type defines the number of components of the color space and the interpretation of those components. For example, RGB is a color space with three components: red, green, and blue. The color space type does not define the particular color characteristics of the space (for example, the chromaticities of the primaries).

**PCS Type** This PCS type is the "output" color space of the profile—its profile connection space. For example, a color profile can convert RGB to the PCS, which then converts it to CMYK.

For an input, display, or output profile useful for tagging colors or images, the PCS type is either XYZ or Lab. Interpret this profile as the corresponding specific color space defined in the ICC specification.
