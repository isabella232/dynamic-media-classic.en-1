---
title: Video SEO (Search Engine Optimization)
description: Learn how to configure video SEO settings.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Administrator
---

# Video SEO (Search Engine Optimization){#video-seo-search-engine-optimization}

SEO is the process of improving the volume of traffic to a Web site from search engines. While search engines excel at gathering information about text-based content, they cannot adequately acquire information about video unless this information is provided to them.

Using Dynamic Media Classic Video SEO, you can apply video metadata to provide search engines with descriptions of your videos. Dynamic Media Classic gives you the ability to create Video Sitemaps and mRSS feeds. These standard XML files are used for submitting video information to search engines:

**Video Sitemap** Informs Google exactly where and what the video content is on a site. So, videos are fully searchable on Google. For example, a Video Sitemap can specify the running time and categories of videos. For information about video Sitemaps, see https://www.google.com/support/webmasters/bin/answer.py?answer=80471.

**mRSS (Media Really Simple Syndication) feed** Used by content publishers to feed media files into Yahoo! Video Search. For information about mRSS feeds, see https://www.rssboard.org/media-rss.

>[!NOTE]
>
>Google supports both the Video Sitemap and mRSS feed protocol for submitting information to search engines.

Dynamic Media Classic can generate Video Sitemaps and mRSS feeds from metadata that is stored with each video. When you create Video Sitemaps and mRSS feeds, you decide which metadata fields from video files to include. In this way, you describe your videos to search engines so that search engines can more accurately direct traffic to videos on your web site

>[!NOTE]
>
>Before creating a Video Sitemap or mRSS feed, find out which fields the search engine requires in the XML file and how to structure these fields. To create a successful Video Sitemap or mRSS feed, it must satisfy the requirements of the search engine.

Dynamic Media Classic creates reports about Video Sitemaps and mRSS feeds after you generate them. These reports are available on the Video SEO Report screen.

>[!NOTE]
>
>For the Video Sitemaps and mRSS feeds, Dynamic Media Classic captures metadata only from videos that are marked for publish. Mark videos for publish to include their metadata in Video Sitemaps and mRSS feeds.

## Choosing video SEO settings {#choosing-video-seo-settings}

Choose Video SEO settings for Video Sitemaps and mRSS feeds on the Video Search Engine Optimization Settings screen. To open this screen, choose Setup > Application Setup > Video SEO > Settings.

In the General Setting area, choose whether to generate Video Sitemaps, mRSS feeds, or both. In the Generation Settings area, map metadata fields to input fields.

After you choose settings, click Generate (or Save & Generate) to create the Video Sitemap, mRSS feeds, or both.

### Choosing General Settings {#choosing-general-settings}

On the Generation Mode drop-down list, choose a report mode:

**Video Sitemap** Create a Video Sitemap.

**mRSS Feed** Create a Media RSS (mRSS) feed.

**Both** Create both types of XML files.

**Off** To stop generating Video Sitemaps and Media RSS (mRSS) feeds, choose this option.

On the Automatic/Manual Mode drop-down list, choose whether to generate automatically or manually:

**Automatic Mode** Dynamic Media Classic automatically generates one Video Sitemap, Media RSS (mRSS) feed, or both, each day. Choose the Mark for Publish option to automatically mark for publish the XML file that Dynamic Media Classic generates.

**Manual Mode** Dynamic Media Classic generates the Video Sitemap, Media RSS (mRSS) feed, or both, when you click Generate or Save & Generate in the Video Search Optimization Settings screen. Choose these options as well:

**No Further Settings** Doesn't mark for publish the XML file that is generated.

**Mark for Publish** Marks for publish the XML file that is generated.

**Allow Partial Generation** Search engines can reject an XML file if it does not contain complete metadata information for all videos. This option generates the XML file even if metadata isn’t available for some videos. A warning is registered on the Report screen. Choose this option if you intend to export the XML file and process the missing information manually.

### Choosing Generation Settings {#choosing-generation-settings}

The Generation Settings area lists input fields for the Video Sitemap and/or mRSS feed, and in the Metadata panel, the names of metadata fields. Use the General Settings area to map input fields to metadata fields. By doing so, you tell Dynamic Media Classic where to obtain metadata for the Video Sitemap and/or mRSS feed.

1. On the Metadata Views menu, choose a metadata view. After you choose a view, the names of metadata fields appear in the Metadata panel. (For information about metadata views, see [Metadata Views](application-setup.md#metadata_views).)
1. Drag metadata field names from the Metadata panel to the Landing Page, Title, Description, Tags, and Category input fields. The Landing Page, Title, and Description fields are required.

   >[!NOTE]
   >
   >You can also manually enter data in input fields.

1. Click Save (to save your settings without generating the XML file), Generate (to generate the XML file), or Save & Generate (to save and generate the file).

   The XML file is generated and recorded in the Job log. Video Sitemap (video-sitemap) and a Media RSS (mRSS) feed (mrss-feed) files are stored in the root folder of your company.

>[!NOTE]
>
>Publish the Video Sitemap or mRSS feed before you can submit it to search engines. Video Sitemap and Media RSS (mRSS) feed files are stored in the root folder of the company. Mark these XML files for publish, if necessary, and click Publish.

## Submitting Video Sitemap and mRSS-Feed files to search engines {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Video Sitemap and Media RSS (mRSS) feed files are stored in the root folder of the company:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Copy one of these URLs into the search engine’s webmaster tools to submit your Video Sitemap or Media RSS (mRSS) feed file to search engines.

## Viewing Video SEO reports {#viewing-video-seo-reports}

View Video SEO reports on the Video Search Engine Optimization Report screen. To open this screen, click Setup > Application Setup > Video SEO > Reports.

If errors occurred when a report was generated, they are listed on the Report screen.
