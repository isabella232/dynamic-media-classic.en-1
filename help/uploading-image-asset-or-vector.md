---
title: Uploading an image asset or a vector asset
seo-title: Uploading an image asset or a vector asset
description: null
seo-description: Learn how to upload an image asset or a vector asset.
uuid: d0e4a754-8a49-4b0f-b202-e9003bdb8f20
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: de21dca9-99fe-4183-b647-debfe112fda4
index: y
internal: n
snippet: y
---

# Uploading an image asset or a vector asset{#uploading-an-image-asset-or-a-vector-asset}

Before you can upload an image asset, you first request a shared-secret key. You use this shared-secret key to retrieve an upload token. You then use the upload token to upload image assets or vector assets.

## Requesting a shared-secret key {#requesting-a-shared-secret-key}

Request a *shared-secret key* by sending an email to Scene 7 Technical Support at s7support@adobe.com.

In the email message, provide the company name that you want to use to upload image assets. After you receive the key from Scene7, save it locally for future use.

## Retrieving the upload token {#retrieving-the-upload-token}

The *upload token* ensures that no one can use the same shared-secret key to upload assets. It ensures that the upload is legitimate and comes from a trusted source.

The upload token is an alphanumeric string that is available only for a specific amount of time. Use the following URLs, substituting your shared-secret key, to retrieve the upload token.

* Image
  `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`In this example, the shared-secret key is `fece4b21-87ee-47fc-9b99-2e29b78b602`

* Vector
  `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In this example, the shared-secret key is `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

By default, the upload token expires five minutes (300 seconds) after you retrieve it. To request more time, include `expires` in the URL and the amount of time you require in seconds. For example, the following sample image URL retrieves an upload token that is valid for 1800 seconds:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

The successful response for images looks like the following:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content - Images</serviceName> 
        <version>1.0.0</version> 
        <operationName>get_uploadtoken</operationName> 
        <serviceStatus>SUCCESS</serviceStatus> 
        <title>Upload Token for fece4b21-87ee-47fc-9b99-2e29b78b602</title> 
        <message> 
            <uploadtoken>aa2a378a-cd25-4c80-994d-312094e0ef20_1800</uploadtoken> 
            <expiration_in_seconds>1800</expiration_in_seconds> 
        </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Save the upload token locally for use with future requests.

You can use the following fields in the query URL string to retrieve an upload token:

|URL parameter|Required or optional|Value|
|--- |--- |--- |
|op|Required|get_uploadtoken|
|shared_secret|Required|The shared-secret key for the company that is doing the upload.|
|expires|Optional|Number of seconds that the upload token is valid. Default is 300 seconds, if not specified.|

**Sample image URL:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**Allowed HTTP methods:** GET and POST

You can now upload an image asset.

See [Uploading an image asset](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Uploading an image asset {#uploading-an-image-asset}

After you retrieve an upload token that is valid for a specific amount of time, you can upload an image asset. You upload the asset as a multipart/form post while sending the rest of the values as a URL query string, as shown in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

See [Retrieving the upload token](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

See [Retrieving a shared-secret key](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

You can also send other optional values as URL query strings, as in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

The `file_limit` parameter specifies the file-size limit in bytes. The `file_exts` parameter specifies the filename extensions that are allowed for upload. Both of these values are optional.

A global limit is set in the application for the file size limit and the filename extensions allowed. If what you send in the request is a subset of the global limits, it is honored. The global limits are the following:

|Global limit|Value|
|--- |--- |
|File size for all clients|20 MB|
|Supported image file formats for upload|BMP, GIF, JPG, PNG, PSD|

The following HTML form lets a user upload an asset. The form asks the user to enter the following information:

* A company name.
* An upload token.
* A file size limit.
* A list of filename extensions.
* Whether or not to preserve the color profile and file name associated with the asset.
* Whether or not to use Knockout Background. If you enable Knockout Background, set the Corner, Tolerance, and Fill Method. See Knockout Background in [Image Editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload).
* The name of the file to upload

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment&gt; elements under &lt;adobefig&gt;.</p>

 -->

![]()

You can view the HTML source code associated with the form above by clicking the following link:

[https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

In Firefox, right-click in the browser window, and then click **View Page Source**. The code shows the corresponding URL query string and the POST method that are run when the user clicks **Submit**.

To view the XML response in Internet Explorer, click **View** &gt; **Source**. To view XML response in Firefox, click **Tools** &gt; **Web Developer** &gt; **Page Source**. Firefox is recommended for viewing XML responses.

The following is a sample response from a successful upload:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>upload</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Your file has been uploaded Successfully.</title> 
            <message> 
            <url>https://s7w2p1.scene7.com/is/image/ </url> 
            <path>000Company/ugc/1442564.tif</path> 
            <fullurl>https://s7w2p1.scene7.com/is/image/000Company/ugc/1442564.tif </fullurl> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

>[!NOTE]
>
>The uploaded asset (JPG, GIF, and so on) is converted to the PTIFF format and the response sends a direct link to that PTIFF asset.

The asset is like any other ImageServing resource; you can apply processing queries to it. For example, the following URL requests an asset that is stretched to the specified width and height.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Send the asset to upload as a multipart/form post while sending the rest of the values as a URL query string. You can use the following fields in the URL query string to upload an asset:

|URL Parameter|Required or optional|Value|
|--- |--- |--- |
|op|Required|upload|
|upload_token|Required|Upload token for the shared-secret key associated with the company.|
|company_name|Required|Name of the company performing the upload.|
|file_limit|Optional|File size limit, in bytes, for the asset.|
|file_exts|Optional|List of allowable extensions for the image asset file.|
|preserve_colorprofile|Optional|Preserves any embedded color profile while converting the uploaded file to PTIFF format. Possible values are true or false. Default is false.|
|preserve_filename|Optional|Preserves the filename of the uploaded asset. Possible values are true or false. Default is false.|

>[!NOTE]
>
>You are required to send the asset to be uploaded as the only field in a multipart POST request.

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Allowed HTTP method:**

POST

### Getting asset metadata for images {#getting-asset-metadata-for-images}

You can use `image_info` to retrieve metadata for an asset that you uploaded, as shown in the following example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

An example of a successful response looks like the following:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>image_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>More information on 1442564.tif</title> 
            <message> 
            File created on Tue Sep 08 19:02:04 CDT 2009, File Size = 243494 bytes 
            <imageFormat>Tiff</imageFormat> 
            <colorSpace>Rgb</colorSpace> 
            <width>686</width> 
            <height>457</height> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

You can use the following fields in the URL query string to request information for an asset:

|URL Parameter|Required or optional|Value|
|--- |--- |--- |
|op|Required|image_info|
|shared_secret|Required|The shared-secret key for the company.|
|image_name|Required|Name of the image.|

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Allowed HTTP method:**

GET and POST

## Uploading a vector asset {#uploading-a-vector-asset}

After you retrieve an upload token that is valid for a specific amount of time, you can upload a vector asset. You upload the asset as a multipart/form post while sending the rest of the values as a URL query string, as shown in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

See [Retrieving the upload token](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

See [Retrieving a shared-secret key](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

You can also send other optional values as URL query strings, as in this example:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. The `file_exts` parameter specifies the filename extensions that are allowed for upload. Both of these values are optional.

A global limit is set in the application for the file size limit and the filename extensions allowed. If what you send in the request is a subset of the global limits, it is honored. The global limits are the following:

|Global limit|Value|
|--- |--- |
|File size for all clients|20 MB|
|Supported vector file formats for upload|AI, EPS, PDF (only when the PDF is previously opened and saved in Adobe Illustrator CS6)|

The following HTML form lets a user upload an asset. The form asks the user to enter the following information:

* A company name.
* An upload token.
* A file size limit.
* A list of filename extensions.
* Whether or not to preserve the color profile and file name associated with the asset.
* Whether or not to use Knockout Background. If you enable Knockout Background, set the Corner, Tolerance, and Fill Method. See Knockout Background in [Image Editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload).
* The name of the file to upload

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment&gt; elements under &lt;adobefig&gt;.</p>

 -->

![]()

The following HTML code is displayed when you right-click in the browser window, and then click **View Source** for the form shown in the illustration. The code shows the corresponding URL query string and the POST method that are run when the user clicks **Submit**.

```as3
<body> 
<script language="javascript"> 
function uploadImage() 
{ 
document.image_upload.action="vector?op=upload&company_name="+document.image_upload.company_name.value+"&upload_token="+document.image_upload.upload_token.value+"&file_limit="+document.image_upload.file_limit.value+"&file_exts="+document.image_upload.file_exts.value; 
return true; 
} 
</script> 
<form method="POST" enctype="multipart/form-data" name="image_upload" id="image_upload" onSubmit="return uploadImage();"> 
<table> 
<tr><td colspan="2"><strong> UGC Vector Upload Test Page: </strong></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr><td><strong> Company Name</strong></td><td><input type="text" size="40" name="company_name"></td></tr> 
<tr><td><strong> Upload Token </strong></td><td><input type="text" size="40" name="upload_token"></td></tr> 
<tr><td><strong> File Size Limit (in bytes) </strong></td><td><input type="text" size="40" name="file_limit"> bytes</td></tr> 
<tr><td><strong> File Extensions allowed </strong></td><td><input type="text" size="40" name="file_exts"></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>File to upload: : </strong></td> 
<td><input name="filename" type="file" id="filename" size="58" maxlength="1024" /></td> 
</tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>Click Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

To view the XML response in Internet Explorer, click **View** &gt; **Source**. To view XML response in Firefox, click **View** &gt; **Page Source**. Firefox is recommended for viewing XML responses.

The following is a sample response from a successful upload:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
    <scene7> 
    <user_generated_content> 
    <response> 
    <serviceName>User Generated Content -Vector</serviceName> 
    <version>1.0.0</version> 
    <operationName>upload</operationName> 
    <serviceStatus>SUCCESS</serviceStatus> 
    <title>Your file has been uploaded Successfully.</title> 
    <message> 
    <url>https://s7w2p1.scene7.com/is/agm</url> 
    <path>W2PTest/ugc/8875744.fxg</path> 
    <fullurl> 
        https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg 
    </fullurl> 
</message> 
</response> 
</user_generated_content> 
</scene7>
```

>[!NOTE]
>
>The uploaded asset (AI, EPS, PDF so on) is converted to the FXG format and the response sends a direct link to that FXG asset.

The asset is like any other Web-to-print resource; you can apply processing queries to it. For example, the following URL converts an FXG resource into a 500x500 png image.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Send the asset to upload as a multipart/form post while sending the rest of the values as a URL query string. You can use the following fields in the URL query string to upload an asset:

|URL Parameter|Required or optional|Value|
|--- |--- |--- |
|op|Required|upload|
|upload_token|Required|Upload token for the shared-secret key associated with the company.|
|company_name|Required|Name of the company performing the upload.|
|file_limit|Optional|File size limit, in bytes, for the asset.|
|file_exts|Optional|List of allowable extensions for the asset file.|

>[!NOTE]
>
>You are required to send the asset to be uploaded as the only field in a multipart POST request.

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Allowed HTTP method:**

POST
