---
title: Deleting an uploaded asset
seo-title: Deleting an uploaded asset
description: null
seo-description: Learn how to delete an uploaded asset.
uuid: bc1e2264-1534-4fa6-ab06-b8f7a9ea7acd
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WSef8d5860223939e262378f7012f30ab2cff-7ffb
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
discoiquuid: cfeb3e5a-b9d7-4883-a587-edafd46b8423
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 43.124-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/user_generated_content;/content/help/en/experience-manager/morehelp/user_generated_content
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
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

<table border="1" cellpadding="4" cellspacing="0" frame="border" rules="rows" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e28552" valign="top" width="NaN%"><p>URL parameter</p></th> 
   <th class="cellrowborder" id="d19e28555" valign="top" width="NaN%"><p>Required/optional</p></th> 
   <th class="cellrowborder" id="d19e28558" valign="top" width="NaN%"><p>Value</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e28552 " valign="top" width="NaN%"><p><span class="code">op</span></p></td> 
   <td class="cellrowborder" headers="d19e28555 " valign="top" width="NaN%"><p>Required</p></td> 
   <td class="cellrowborder" headers="d19e28558 " valign="top" width="NaN%"><p><span class="code">delete</span></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e28552 " valign="top" width="NaN%"><p><span class="code">shared_secret</span></p></td> 
   <td class="cellrowborder" headers="d19e28555 " valign="top" width="NaN%"><p>Required</p></td> 
   <td class="cellrowborder" headers="d19e28558 " valign="top" width="NaN%"><p>The shared-secret key for the company.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e28552 " valign="top" width="NaN%"> 
    <ul> 
     <li><p>For images:</p><p><span class="code">image_name</span></p></li> 
     <li><p>For Vector:</p><p>fxg_name</p></li> 
    </ul></td> 
   <td class="cellrowborder" headers="d19e28555 " valign="top" width="NaN%"><p>Required</p></td> 
   <td class="cellrowborder" headers="d19e28558 " valign="top" width="NaN%"><p>Name of the asset to delete.</p></td> 
  </tr> 
 </tbody> 
</table>

**Sample image URL:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg`
