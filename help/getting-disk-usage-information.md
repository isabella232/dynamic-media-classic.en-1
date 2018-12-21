---
title: Getting disk usage information
seo-title: Getting disk usage information
description: null
seo-description: Learn how to get disk usage information.
uuid: 01361693-53d0-4072-b7c3-f284631d28cf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: 6763546d-83c4-42dc-879f-6bbfc8b56482

---

# Getting disk usage information {#getting-disk-usage-information}

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

|URL parameter|Required/optional|Value|
|--- |--- |--- |
|op|Required|disk_info|
|shared_secret|Required|The shared-secret key for the company|

The following sample code gets disk information for 000Company:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```

