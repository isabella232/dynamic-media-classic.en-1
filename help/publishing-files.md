---
title: Publishing files
seo-title: Publishing files
description: null
seo-description: Learn how to publish files.
uuid: cdcf519b-4c1e-430b-b43a-2f20f75071b1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 39099bc0-9228-46f0-9bee-3542059f4695
index: y
internal: n
snippet: y
---

# Publishing files{#publishing-files}

You publish your assets to Scene7 Image Servers. You can publish assets on a one-time basis or arrange for Scene7 to publish assets on a recurring schedule. After your assets are published, they are available to you for delivery. You can copy the URL calls from the Scene7 Publishing System and add them to your website or application.

Scene7 Publishing System now supports the delivery of all images and video over HTTP/2. That is, a published URL or embed code for the image or video is available to be integrated with any application that accepts a hosted asset. That published asset is then delivered by way of HTTP/2 protocol. This method of delivery improves the way browsers and servers communicate, allowing for better response and load times of all your Scene7 assets. See [HTTP2 Delivery of Content FAQ](https://docs.adobe.com/content/docs/en/aem/6-2/administer/integration/marketing-cloud/scene7/http2faq.html).

## Publish After Uploading {#publish-after-uploading}

Assets either in a published or unpublished state. By default, any assets that you upload into Scene7 are automatically marked for publishing.

For more information, see the [Instant Publish Notice PDF](https://marketing.adobe.com/resources/help/en_US/s7/rendering-instant-publish-notification.pdf).

Use these techniques to mark assets for publish:

**Publish After Uploading** On the Upload page, near the bottom, select Publish After Uploading. The default is a selected state.

**Publish After Uploading** In the Job Options dialog box, select Publish After Uploading. The default is a selected state.

Some "child" assets are automatically marked for publish when their parents are marked for publish. This table lists child assets that are marked for publish automatically.

|Parent (group) item|Child (member) items|
|--- |--- |
|Image sets|Images within the set.|
|Swatch sets|Swatches within the set.|
|Spin sets|Images within the set.|
|Templates|Template files, pages, and images.|

Derived images are also automatically marked for publish when their parent images are being published. Derived images include images you adjusted with image-editing options. You can see these derived images in Detail view under Built & Derivatives.

## Creating a publish job {#creating-a-publish-job}

Create a publish job to publish assets you have uploaded to Scene7 servers but chose not to automatically published them yet. You can perform a one-time publish job or schedule jobs to recur on a regular basis. Scene7 offers advanced publishing options for publishing to specific servers and options for republishing assets that have already been published.

**To create a publish job**

1. On the Global Navigation bar, click **Publish**.
1. In the Publish dialog box, choose whether you want a one-time or recurring publish job.

   See [Creating a one-time publish job](publishing-files.md#creating_a_one_time_publish_job) and [Creating a recurring publish job](publishing-files.md#creating_a_recurring_publish_job).

1. Enter a job name.
1. Optionally, display the Advanced options and choose these options.

   See [Advanced publish options](publishing-files.md#advanced_publish_options).

1. Click **Submit Publish**.

SPS tracks publish jobs on the Jobs page. You can review publish jobs on that page.

>[!NOTE]
>
>Assets you republish (you have published them before) do not appear immediately on your website because of the web caching mechanism on the content delivery network (CDN). See [Republished assets and CDN delays](publishing-files.md#republished_assets_and_cdn_delays).

### Creating a one-time publish job {#creating-a-one-time-publish-job}

Create a one-time publish job by selecting the One-Time option on the Publish page.

If you want the publish job to occur at a later date, select the When menu, and choose Schedule For Later. Then use the Calendar and Time slider to select a day and time to execute the publish job.

### Creating a recurring publish job {#creating-a-recurring-publish-job}

Create a recurring publish job by selecting the Recurring option on the Publish page.

Then choose a Repeat option—Daily, Weekly, Monthly, or Custom—to declare when you want the publishing job to recur. Scene7 presents calendar tools for scheduling the recurring publish job. You can choose the Custom option and enter a rule in the Rule box to describe a custom job interval.

See [Creating a custom upload or publish job time interval](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Recurring publish (and upload) jobs are listed on the Jobs page. You can edit or delete a scheduled job by going to the Scheduled tab of the Jobs page.

### Advanced publish options {#advanced-publish-options}

You can display the Advanced options on the Publish page and choose these options for handling a publish job:

**Publish To** Choose a server type to publish assets only to a specific server, not to all servers.

**Publish** By default, SPS publishes only assets that are new and have not been published before (the New Since Last Publish option). However, you can choose Full Publish to also publish assets that have been updated or changed since they were last published. Choose Full w/ Search Data if you are publishing an eCatalog and you want readers to be able to search it by keyword.

**Run Job As** Choose a user name from the list. You can sort jobs by user name on the Jobs page. By choosing a name, you associate a publish job with a user.

**HTTP Notification** Enter a URL to trigger subsequent publish jobs.

See [Using an upload or publish job as a trigger](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Canceling a publish job {#canceling-a-publish-job}

You can cancel an in-progress publish job. Moreover, if you are an administrator, you can cancel an in-progress publishing job from the company Jobs page.

To cancel a publishing job, go to the Jobs page and click Cancel. On the Scheduled tab of the Jobs page, you can pause or resume a job by deselecting or selecting the check box in the job’s Active column.

>[!NOTE]
>
>After you cancel a publish job, its status changes to “stopping” until the job reaches a point where it can stop safely. Stopping a publish job can take some time if the job is in the process of getting data from the database.

## Manually publishing assets {#manually-publishing-assets}

You can publish individual assets manually instead of creating a publishing job. When you publish sets, such as an Image Set or an Adaptive Video Set, the set (or “parent”) and all members (or “children”) within that set get published.

Unpublished assets are indicated in the user interface by a grey, round icon with a slash through it (unpublished state), to the left of the asset’s name. After an asset is published, the icon turns green and has a white check mark in the center (published state).

**To manually publish assets**

1. Do one of the following:

    * In the Grid View, List View, or Details View, use standard file selection methods to select one or more unpublished assets.

      On the Global Navigation Bar, click **File** &gt; **Publish**.
    
    * In the Grid View, List View, or Details View, click the grey, round icon with a slash through it, to the left of the asset’s name.

## Manually unpublishing assets {#manually-unpublishing-assets}

You can unpublish individual assets manually. When you unpublish sets, such as a Swatch Set or an eCatalog, the set (or “parent”) itself goes into an unpublished state. However, the members (or “children”) within that set are not affected; instead, they each retain their existing published or unpublished state.

Published assets are indicated in the user interface by a round, green icon with a white check mark in the center (published state), to the left of the asset’s name. After an asset is unpublished, the icon turns grey with a slash through it (unpublished state),

**To manually unpublish assets**

1. Do one of the following:

    * In the Grid View, List View, or Details View, select one or more pubished assets.

      On the Global Navigation Bar, click **File** &gt; **Unpublish**.
    
    * In the Grid View, List View, or Details View, click the round, green check mark icon to the left of the asset’s name.

## Getting an asset’s publish history {#getting-an-asset-s-publish-history}

The last date an asset was published is shown in Detail view at the top of the panel. You can get more details about the publishing history by opening the History & Published Servers panel in Detail view. From there, you can see when the asset was published and to which servers it was published.

## Republished assets and CDN delays {#republished-assets-and-cdn-delays}

Scene7 assets are distributed on the content delivery network (CDN). CDN is a system of computer servers networked together that cooperate transparently to deliver content, especially large media content, to end users. In the CDN system, web content is stored in web caches across the Internet (called the edge cache network). Web content is delivered from these web caches to end users to make for faster deliveries.

The first time someone downloads a web page, the assets are delivered to a CDN web cache server. They are stored on this server so that the next time someone in the same area accesses the web page, the same cached content can be delivered faster. The content is delivered faster because it is located closer to the end user. CDN makes for faster web page displays. It decreases bandwidth demands on the central server because content is delivered from the edge cache network, not from a central server in every instance.

Newly published Scene7 content is available immediately to the end user and quickly populates the edge cache network. However, newly republished content—images that have the exact same names as images previously published to an image server—is not updated on CDN for up to ten hours. Instead, end users see what is in a web cache on the CDN network. For this reason, your Scene7 republished assets may not appear to end users for ten hours.

If you want your newly republished image assets to be available sooner than the ten-hour delay, you can flush web caches on CDN. Flushing these web caches removes old content from CDN web caches and replaces it with your most recently published assets.

To flush the cache, click File &gt; Invalidate CDN. All selected files are removed from the cache. If there are no publishable assets, or if you are not a company admin, the Remove from CDN option is not available.

>[!MORE_LIKE_THIS]
>
>* [Checking job files](checking-job-files.md#checking_job_files)
>* [Editing, deleting, pausing, and resuming recurring jobs](checking-job-files.md#editing_deleting_pausing_and_resuming_recurring_jobs)
