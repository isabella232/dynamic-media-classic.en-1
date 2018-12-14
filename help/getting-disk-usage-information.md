---
title: Getting disk usage information
seo-title: Getting disk usage information
description: null
seo-description: Learn how to get disk usage information.
uuid: 01361693-53d0-4072-b7c3-f284631d28cf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
discoiquuid: 6763546d-83c4-42dc-879f-6bbfc8b56482
index: y
internal: n
snippet: y
---

# Getting disk usage information{#getting-disk-usage-information}

You can use the `disk_info` parameter to retrieve information about a company’s disk space usage, as shown in the following example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

A sample response looks like the following:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>disk_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Disk Information for d03b7e0b-c9dc-4c6c-af0b-419beeea1c63</title> 
            <message>Total Space available = 1395402342400 bytes. Total Space used = 0 bytes.</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

You can use the following fields in the URL query string to get disk usage information:

<table border="1" cellpadding="4" cellspacing="0" frame="border" rules="rows" summary=""> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e28644" valign="top" width="NaN%"><p>URL parameter</p></th> 
   <th class="cellrowborder" id="d19e28647" valign="top" width="NaN%"><p>Required/optional</p></th> 
   <th class="cellrowborder" id="d19e28650" valign="top" width="NaN%"><p>Value</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e28644 " valign="top" width="NaN%"><p><span class="code">op</span></p></td> 
   <td class="cellrowborder" headers="d19e28647 " valign="top" width="NaN%"><p>Required</p></td> 
   <td class="cellrowborder" headers="d19e28650 " valign="top" width="NaN%"><p><span class="code">disk_info</span></p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e28644 " valign="top" width="NaN%"><p><span class="code">shared_secret</span></p></td> 
   <td class="cellrowborder" headers="d19e28647 " valign="top" width="NaN%"><p>Required</p></td> 
   <td class="cellrowborder" headers="d19e28650 " valign="top" width="NaN%"><p>The shared-secret key for the company</p></td> 
  </tr> 
 </tbody> 
</table>

The following sample code gets disk information for 000Company:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```

