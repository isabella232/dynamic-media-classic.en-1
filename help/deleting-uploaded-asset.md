---
title: Deleting an uploaded asset
seo-title: Deleting an uploaded asset
description: null
seo-description: Learn how to delete an uploaded asset.
uuid: edd2b688-c377-4be1-ba16-d2dd2e6f716d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
discoiquuid: dd338c8c-06c6-44d5-8493-dc2087eeeafb
index: y
internal: n
snippet: y
---

# Deleting an uploaded asset{#deleting-an-uploaded-asset}

You can use the `delete` parameter in this format to delete an asset:

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

The following is an example of a response when an image asset is deleted:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>delete</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Delete request for1442564.tif</title> 
            <message>Your file was successfully deleted</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

You can use the following fields in the URL query string to delete an asset:

|URL parameter|Required/optional|Value|
|--- |--- |--- |
|op|Required|delete|
|shared_secret|Required|The shared-secret key for the company.|
|<ul><li>For images:image_name</li><li>For Vector:fxg_name|Required|Name of the asset to delete.</ul>|

**Sample image URL:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg`
