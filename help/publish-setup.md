---
title: Publish Setup
seo-title: Publish Setup
description: null
seo-description: The Publish Setup screen settings determine how assets are delivered by default from Dynamic Media Classic servers to web sites or applications.
uuid: 196f25c8-abf5-4c5d-8f6f-bc70007a0301
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: cba59093-28b6-4490-b838-d942b72ad1ec

---

# Publish Setup {#publish-setup}

The Publish Setup screen settings determine how assets are delivered by default from Dynamic Media Classic servers to web sites or applications. If no setting is specified, the Dynamic Media Classic server delivers an asset according to a default setting on a Publish Setup screen. For example, a request to deliver an image that does not include a resolution attribute yields an image with the Default Object Resolution setting on the Image Server screen.

Administrators can change the default settings on the Image Server, Image Renderer, and Vignette screens to establish default settings for delivering assets from servers.

To open the Publish Setup screens, click Setup > Application Setup > Publish Setup.

>[!NOTE]
>
>The Publish Setup screens are for use by experienced web site developers and programmers. Dynamic Media Classic assumes that users who change settings on these screens are familiar with Dynamic Media Classic, HTTP protocol standards and conventions, and basic imaging technology.

## Image Server {#image-server}

The Image Server screen establishes default settings for delivering images from image servers. Settings are available in these five categories (see the Image Server screen itself for detailed descriptions of the settings).

Change these settings only with the assistance of a Dynamic Media Classic support person.

**Catalog Management** These settings determine how Dynamic Media Classic and the catalog interact. Unlike most web servers, Dynamic Media Image Server URL calls go to a manifest-or catalog-file rather than an image file proper. The catalog file (not to be confused with an eCatalog) contains a list of all content published to the image server along with the path to each image. If you have a Digimarc ID, enter your user information in the Digimarc User Info section.

**Request Attributes** These settings impose limits on images that can be delivered from the server. For example, the *maximum* **[!UICONTROL Reply Image Size Limit]** is **[!UICONTROL Width]** 5000 and **[!UICONTROL Height]** 5000.

**Default Request Attributes** These settings pertain to the default appearance of images.

**Common Thumbnail Attributes** These settings pertain to the default appearance and alignment of thumbnail images.

**Defaults for Catalog Fields** These settings pertain to the resolution and default thumbnail type of images.

**Color Management Attributes** These settings determine which ICC color profiles are used.

**Compatibility Attributes** This setting enables leading and trailing paragraphs in text layers to be treated as they were in version 3.6 for backwards compatibility.

**Localization Support** These settings let you manage multiple locale attributes. It also lets you specify a locale map string so you can define which languages you want to support for the various tooltips in Viewers.

For example, if you are a multi-national brand that sells in different countries, you can ensure that each country has their own locale-specific Viewer. To accomplish this functionality, you specify a locale map string. Then you edit the tooltip text in a Viewer’s preset by adding the translated text strings for the language you want.

>[!NOTE]
> To set up Localization Support options, [use the Admin Console to create a support case.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) In your support case, request setup help.

For more information about setting up **Localization Support**, see [Considerations when setting up localization of assets](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Considerations when setting up localization of assets {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>If you want to set up Localization Support options in Dynamic Media Classic, such as the Locale Map field, [use the Admin Console to create a support case.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) In your support case, request setup help.

A common way to use Dynamic Media Classic is to manage the product imagery on e-Commerce websites. International businesses face the challenge that assets for similar products look different from country to country. Usually the differences are for a very few part of the overall media. Addressing such differences by copying all assets for each of the countries and over-write just the differences is a tremendous effort and contradicts the single master asset metaphor. Such differences for assets can endure, from country-specific videos with different audio tracks, to subtle but important differences in a power cord that is used with the product. Dynamic Media Classic uses a basic lookup mechanism. You define an order of asset suffixes in which the Image Server is looking, starting from the required locale.

**How assets are localized**

The locale for an IS (Image Serving) request is identified with the following IS/IR (Image Rendering) command:

`locale=`

This command accepts a locale id (locId) string which is not case-sensitive. The locale id is typically a 2-6 character string composed of letters and “_”.

IS supports arbitrary printable ASCII strings.The `locale=` command has a global scope, meaning that it is applied to the entire request, including all nested IS and IR requests, referenced templates, and image layers. Multiple locales per request, such as a different locale for each layer, is not supported. However, it is conceivable to allow explicit overrides in nested requests.

If `locale=` is not specified, `attribute::DefaultLocale` is passed to the translation engines. Limited input validation is applied to the `locale=` value. Empty `locale=` values are permitted. Because `locale=` has a global scope, `attribute::DefaultLocale` is provided by the main catalog for the entire request.

Some of the benefits of using `locale=` and `attribute::DefaultLocale` include the following:

* Share contents for multiple locales.
* Access locale-specific contents using generic ids.
* Allow flexibility around naming conventions and the management of locale-specific contents, such as locale prefix versus suffix, or locale-specific contents in a separate catalog.
* Support direct access to locale-specific versions.
* Aggregate objects, such as image sets, may contain generic references to potentially locale-specific contents.
* Supports all contents managed by catalogs that may need localization, including images, image sets, vignettes, materials, and viewer configuration records.
* Minimize changes to the IPS database and IS manifest mechanisms.
* Support for static contents such as videos and skins will be added when RFC IS-63 is implemented.
* The default locale is configurable.

**Application scenarios**

|Application|Scenario|
|--- |--- |
|Viewer localization|After static content catalogs are implemented, localization is controlled entirely with the locale= parameter, appended to all requests that are made to IS. Configuration records, skins, splash screens, and so on, can have locale-specific variants or not. The correct contents is provided by IS without the viewer needing to know which contents is localized and what its IDs are.|
|Images and video|Multi-national companies often have a mix of generic and locale-specific contents. With this mechanism, a reference to an image or video can be generic, and IS serves up the locale-specific contents if it is available.|
|Image sets and Media sets|The entire image set can be different for some locales--such as when an eCatalog is completely different--with the translation from a generic to a locale-specific image set handled by the viewer.More commonly, individual IDs in a generic set may refer to localized contents. For example, most photos of an appliance can be the same in all languages, except the photo of the control panel. IS automatically translate IDs, so there is no need to generate locale-specific image sets.|

**Implementing asset localization**

Dynamic Media Classic and Image Serving have an interface that allows for the localizations of images and static content.

Without localization, an Image Server URL looks like the following:

`https://server/is/image/company/image`

With localization, an Image Server URL adds the `locale=` parameter to the path, as in the following:

`https://server/is/image/company/image?locale=de_DE`

On receipt of the http call by the Image Server, the `locale=` parameter is parsed through the localeMap field found in **Setup** > **Application Setup** > **Publish Setup** > **Image Server** > **Localization Support** group.

The Locale Map field contains a list of entries that are separated using the pipe symbol (|).

Each entry consists of a comma-separated list of values. The first value is the search value that is passed by the `locale=` parameter. The remaining values are suffix/replacement values that are subsequently tried until one results in an existing image.

Whether a suffix value or a replacement value is applied depends on the Global Locale setting in **Setup** > **Application Setup** > **Publish Setup** > **Image Server** > **Localization Support** group.

>[!NOTE]
>
>The Global Locale setting is currently only possible when you set it through the API, not within the Dynamic Media Classic interface.

**Suffix example**

|URL|localeMap IDs|Result|
|--- |--- |--- |
|`https://server/is/image/company/image?locale=de_DE`|`de_DE,_DE,|fr_FR,_FR,`|Notice that there is no GlobalLocale defined. The locale parameter de_DE is matched against the first entry in the localeMap. The first corresponding value _DE is added as a suffix to the asset image_DE and an attempt is made to find it on the Image Server. If it is found on the server, it is returned. Otherwise, the second value “” is used as a suffix, resulting in the image itself being returned.|

**Replacement example**

|URL|GlobalLocale and localeMap IDs|Result|
|--- |--- |--- |
|`https://server/is/image/company/image-main-01?locale=de_DE`|`GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main`|In the replacement example above, GlobalLocale is set to main. The locale parameter de_DE is matched against the first entry in the localeMap. The GlobalLocale substring is found and replaced with the first corresponding value de in the localeMap: image-de-01. If it is found on the Image Server, it is returned. If not, the second value is replaced, resulting in image-main-01.|

If no locale is defined in the URL, the Image Server takes the DefaultLocale, if it is defined, and applies it to the URL.

If an unknown or empty locale parameter is supplied with `locale=`, then the localeMap is scanned for the empty value “starting with,”. It is important to configure this to have a default locale applied for unknown locales.

**About the defaultImage**

The Image Server tries the options for the requested locale, one after the other. If no match is found, the locale options are applied to the defaultImage, and the matching version is returned. Therefore, either each locale should include an option for the image without localization, or localized defaultImage versions should be made available in Dynamic Media Classic.

**Scenarios for finding the localeMap**

Suppose you want to support the following locales:

`en, en_us, en_uk, de, de_at, de_de, fr`

You map these locales to the suffixes `_E`, `_G`, and `_F`, for English, German, and French, respectively. For all examples, the generic input image ID is `myImg`.

*Standard behavior for finding the localeMap*

The locale IDs are mapped to their corresponding suffixes. If no locale-specific ID is found in the catalog, the generic ID is tried. Note the empty locSuffix values which map to the generic ID.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

|locale=|Output IDs to search|
|--- |--- |
|en,en_us, en_uk|myImg_E, myImg|
|de,de_de,de_at|myImg_D, myImg|
|fr|myImg_F, myImg|
|All others|-|

*Finding the localeMap when the locale is unknown*

You can map unknown locales to specific IDs or to generic IDs. For our example, you can map unknown locales to the English IDs, or if they do not exist, to the generic IDs.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

|locale=|Output IDs to search|
|--- |--- |
|de,de_de,de_at|myImg_D,myImg|
|fr|myImg_F,myImg|
|All others|myImg_E,myImg|

You could also have a dedicated locSuffix, such as U, just for unknown locales, and force to the default image if no `_U` exists, as in the following:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Or, you can map directly to the generic ID, as in the following:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*Finding the localeMap using a multi-tiered lookup*

It is often desirable to group locales, such as European, Middle Eastern, and North American, to address regional standards, such as skin exposure. You can achieve this effect using a multi-tiered lookup.

For this example, suppose you want to support collections for Western and Middle Eastern use. Both collections are based on the generic image collection, and both add or modify some images. Both collections are then further refined for specific locales, such as `m1, m2` for two middle-eastern variants, and `w1, w2,` and `w3` for three Western locales, except that images are shared for `w1` and `w3`. Unknown locales are mapped only to the generic collection and do not have access to locale-specific images. The following is what the map would look like:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

|locale=|Output IDs to search|
|--- |--- |
|w1, w3|myImg-W, myImg|
|w2|myImg-W2, myImg-W, myImg|
|m1|myImg-M1, myImg-M, myImg|
|m2|myImg-M2, myImg-M, myImg|
|All others|mylmg|

*Finding the localeMap by searching for specific IDs*

Some image naming conventions may not support generic image IDs. The generic IDs from the request must be mapped to a specific ID in the catalog. However, there may be instances where the exact specific ID is not known.

Using the first example as a basis, images for all languages may have the suffixes `_1`, `_2`, or `_3`. Images that are specific to French locales may have the suffixes `_22` or `_23` suffix. And images that are specific to German locales may have the suffixes `_470` or `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

|locale=|Output IDs to search|
|--- |--- |
|fr|myImg_22, myImg_23, myImg_1, myImg_2, myImg_3|
|de, de_at, de_de|myImg_470, myImg_480, myImg_1, myImg_2,myImg_3|
|All others|myImg_1, myImg_2, myImg_3|

**Important considerations when implementing localization support**

* Localization is limited to ID-based asset calls and cannot be used on path-based asset calls. Therefore, when calling videos with locale, it must be called as company/assetID; no full path to the video. This means that you cannot use rtmp with localization because that method is for use with path-based video calls only.
* You cannot use a Mixed Media Set that contains a single video when localeMap is active, otherwise the call to the contents of the set fails. To work around this issue you can add a single video to an Adaptive Video Set. Then, add the Adaptive Video Set to a Mixed Media Set.
* Certain requests are not localized, such as requests for the contents of an Adaptive Video Set. Therefore, if you intend to use Adaptive Video Sets with localization, you should place the Adaptive Video Set within a Mixed Media Set. Then, call the set into a Mixed Media viewer with the `locale=` parameter.

## Image Renderer {#image-renderer}

The Image Renderer screen establishes default settings for delivering Image Sets from image rendering servers. Settings are available in these five categories (see the Image Server screen itself for detailed descriptions of the settings):

**Catalog Management** These settings determine how Dynamic Media Classic and the catalog file interact. Dynamic Media Classic Render Server URL calls are made to the catalog, which in turn calls to deliver images from the server. Change these settings only with the assistance of a Dynamic Media Classic support person.

**Session Attributes** These settings establish error parameters, the URL for relative image URLs, and whether object overlapping is permitted.

**Default Material Attributes** These settings establish default resolution and sharpening settings for images.

**Response Image Attributes** These settings pertain to the default appearance of images.

**Color Management Attributes** These settings pertain to the default color settings of images.

## Vignette {#vignette}

The Vignette screen offers settings for establishing the default appearance of vignettes (see the screen itself for detailed descriptions of options).
