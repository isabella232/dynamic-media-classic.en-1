---
title: Getting disk usage information
seo-title: Getting disk usage information
description: null
seo-description: Learn how to get disk usage information.
uuid: 471ff302-e362-4c04-a83a-81d8b4cf20fe
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WSef8d5860223939e262378f7012f30ab2cff-7ffa
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
discoiquuid: 3eaae045-30f7-4704-97ad-409a332e21b6
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 43.356-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/user_generated_content;/content/help/en/experience-manager/morehelp/user_generated_content
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
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

