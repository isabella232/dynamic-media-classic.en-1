---
title: Instrumenting a viewer using the Adobe Analytics Instrumentation Kit
seo-title: Instrumenting a viewer using the Adobe Analytics Instrumentation Kit
description: null
seo-description: Learn how to instrument a viewer using the Adobe Analytics Instrumentation Kit.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038

---

# Instrumenting a viewer using the Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

You can use the Adobe Analytics Instrumentation Kit to integrate an HTML5 viewer with Adobe Analytics.

If you use any of the predefined Scene7 HTML5 viewer presets, be aware that they already contain all the implementation code needed to send data to Adobe Analytics--no further instrumentation is required by you. However, if you choose to create your own custom HTML5 viewers using the HTML5 Viewer SDK, see the *Adobe Scene7 HTML5 Viewer SDK User Guide* for instructions on how to use the Adobe Analytics Tracking Manager component.

The *Adobe Scene7 HTML5 Viewer SDK User Guide* is available as part of the SDK download from Adobe Developer Connection.

See [www.adobe.com/go/learn/learn_s7_devresources_en](https://www.adobe.com/go/learn/learn_s7_devresources_en).

## Set up Adobe Analytics tracking from Scene7 Publishing System {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

For all HTML5 viewers, add the following JavaScript to the HTML container, usually in the &lt;head&gt; element:

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<SPS Company ID>&preset=companypreset-1"></script>
```

`Company` is set to the SPS company name. `&preset` is optional unless the company preset name is not `companypreset`. In such cases, it could be `companypreset-1, companypreset-2`, and so on. The higher number is a newer instance of the preset. To determine the correct company preset value name, click **Copy URL** , and then look at the `preset=`parameter to find the company preset name.

Continuing, you will now you add a function that transmits the viewer event to the Adobe Analytics tracking code.

Add the `s7ComponentEvent()` function to the container HTML (or JSP, or ASPX or other):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

The function name is case sensitive. The only parameter passed to `s7componentEvent`that is required is the last one: `eventData`. `s7track()` is defined in s_code.jsp included above. `s7track` handles all tracking per each event. (To further customize data transmitted to Adobe Analytics, this area is the place to do it.)

## Enabling HREF and ITEM events {#enabling-href-and-item-events}

You can enable HREF (rollover) and ITEM (mouse clicks/touch) events in the viewers through Image Map editing. Define the identifiers for the HREF and ITEM within the Image Map that is associated with viewer content. Add a `&rolloverKey=` parameter to the HREF value within the Image Map.
