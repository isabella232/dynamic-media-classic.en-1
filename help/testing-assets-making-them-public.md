---
title: Testing assets before making them public
description: Learn how to test assets before making them public.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67

---

# Testing assets before making them public {#testing-assets-before-making-them-public}

Secure Testing helps you define a secure test environment and build a robust B2B solution, based upon a configurable set of IP address and ranges. This functionality lets you match your Dynamic Media Classic deployments with the architecture of your content management and commerce platform.

With Secure Testing, you can preview the staging version of the website with unpublished content.

You might prefer to create a staging environment rather than making assets publicly available for the following reasons:

* Preview websites before public launch (staging website).
* Serve assets that require restricted access, such as eCatalogs that show prices in a B2B web application.
* Use assets behind a firewall as part of product information management system, customer service application, training site, and so on.

>[!NOTE]
>
>Secure Testing does not affect access to Dynamic Media Classic. Dynamic Media Classic security remains consistent and requires the usual credentials for access to Dynamic Media Classic and related web services.

## How Secure Testing works {#how-secure-testing-works}

Most corporations run their Internet behind a firewall. Access to the Internet is possible through certain routes and typically through a limited range of public IP addresses.

From your corporate network, you can figure out your public IP address using websites like https://whatismyip.com or request this information from your corporate IT organization.

With the Secure Testing, Dynamic Media Classic establishes a dedicated Image Server for staging environments or internal applications. Any request to this server checks the origin IP address. If the incoming request is not within the approved list of IP addresses, a failure response is returned. The Dynamic Media Classic Company Administrator configures the approved list of IP addresses for their company’s Secure Testing environment.

Because the location of the original request must be confirmed, the traffic of the Secure Testing service is not routed through a content distribution network like public Dynamic Media Image Server traffic. Requests to the Secure Testing service might have a slightly higher latency compared to the public Dynamic Media Image Servers.

Unpublished assets are immediately available from the Secure Testing services, without the need to publish. This allows you to run a preview before assets are published to their public facing image server.

***note**: Secure Testing services leverage the Catalog Server that is configured with an internal publish context. Therefore, if your company is configured to publish to Secure Testing, be aware that any uploaded assets in Dynamic Media Classic immediately become available on Secure Testing services. This functionality is true regardless of whether or not the assets are marked for publish on upload.*

Secure Testing services currently support the following asset types and functionalities:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Images.
* Vignettes (Render Server requests).
* Render Server requests (supported, but must be requested explicitly by customer).
* Sets, including image sets, eCatalog, render sets, and media sets.
* Standard Dynamic Media Classic rich media viewers.
* Dynamic Media Classic OnDemand JSP pages.
* Static content, such as PDF files and progressively served videos.
* HTTP video streaming.
* Progressive video streaming.

The following asset types and functionalities are currently not supported:

* RTMP video streaming
* UGC services
* Web-to-print
* Dynamic Media Classic Info or eCatalog search

## Testing the Secure Testing service {#testing-the-secure-testing-service}

You should test the Secure Testing service to make sure it works as expected.

Note: If you do not mention any IP's under Setup > Publish Setup > Image Server > Test Image Service
if you add an IP only that IP will be able to call the assets and no other IP will be allowed to make the calls. As long there is no IP mentioned under that section all IP's are allowed to make the calls for the assets, and they will show up.

**Prepare your account**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Contact Technical Support and request that Secure Testing be enabled on your account.
1. In Dynamic Media Classic, click **Setup** > **Publish Setup** > **Image Server**.
1. On the Image Server Publish page, in the Publish Context drop-down list, select **Test Image Serving**.
1. For the Client Address Filter, click **Add**.
1. Select the check box to enable (turn on) the address, and then type an IP address and net mask in the respective text fields.

   >[!NOTE]
   >
   >If you add a single IP address and net mask, that address can make asset calls. However, any other IP addresses and net masks that you add are not permitted to make asset calls. As such, you may want to consider disabling (turn off) the check box in the step above to turn off the ability to specify an IP address and net mask. Doing so effectively permits *all* IP addresses to make asset calls, and they will all show up. 

1. Do one of the following:
   * Repeat the previous two steps to add more IP addresses.
   * Continue to the next step.
1. At the lower-left of the Image Server Publish page, click **Save**
1. Upload the desired images to your Dynamic Media Classic account.

   See [Uploading files](uploading-files.md#uploading_files).

1. Make sure some of the images are marked for publish and others are unmarked, and then submit the publish job.

   See [Publishing](publishing-files.md#publishing_files).

1. Determine the name of your Secure Testing service by clicking **Setup** > **Application Setup** > **General Settings**. 
1. On the Application General Settings page, under the Servers group, find the name to the right of **Test Publish Context Server Name**.

Contact Adobe Care if the server name is missing or the URLs to the server do not work.

**Prepare website variations**

You need two variations of a website that links the published and unpublished assets:

* Public version - Link assets using your traditional Dynamic Media Classic URL syntax.
* Staging version - Link assets using the same syntax but with the Secure Testing site name.

**Run the tests**

Perform the following tests:

1. Check whether assets are visible from within your corporate network.

   From within the corporate network identified by the previously defined IP address range, the staging version of the website should display all images, whether marked for publish or not. This allows you to test without accidentally making images available before preview approval or product launch.

   Confirm that the public version of your site shows published assets as previously experienced with Dynamic Media Classic.

1. From outside your corporate network, verify that nonpublished assets (that is, unmarked for publish) are protected from third-party access.

   Access your network from outside (such as, from your home computer or over a 3G connection), then verify that the public version of the site shows all published assets but none of the unpublished content.

   Confirm that the staging version does not show any asset because you are accessing the Secure Testing service from an unapproved IP address.

