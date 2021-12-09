---
title: Manage content variations
description: Learn how to manage content variations in Adobe Dynamic Media Classic.
uuid: 1e40a526-02f8-41d9-886f-6d094546bc13
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: aa129b0e-fc73-4fc2-a894-4560b3f46c4f
feature: Dynamic Media Classic
role: User
exl-id: 65b8c314-7ec1-417f-8a7b-aa13762072a1
---
# Manage content variations{#managing-content-variations}

Use template sets to manage the way asset variations are published.

Create a template set to manage variations of a template. You can control which variation is used without changing the code on your site. This method helps content managers rotate content without requiring IT to change a URL in the Web code.

Universal URLs are used to display the template variation that appears on the page, based on the order they are listed in the set. The template at the top of the template set list is always published.

You can use any image preset URL from the list. Image preset URLs are like universal URLs. There can be more than one image preset URL.

1. Go to **[!UICONTROL Build]** > **[!UICONTROL Template Sets]**.
1. In the builder, select a template, then select **[!UICONTROL Add/Preview]**.
1. Modify the template properties and select **[!UICONTROL Save As]** to create another version.
1. Type a name, and then select **[!UICONTROL Save]**.

   Both the asset and the template must be published.

1. Go to the Detail page to get a copy URL from the URLs section.

You can move a template in the template order (for example, to the top of the list) by dragging it to its new location. Publish again to submit the new order.

>[!NOTE]
>
>If necessary, clear the cache to see the changes. The change only appears on the website after the change has made its way through the cache cycle.
