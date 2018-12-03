---
title: Checking job files
seo-title: Checking job files
description: null
seo-description: Learn how to check job files.
uuid: d29da54a-9e49-49b1-8b58-cb3ee533d44a
acrolinxstatus: not_checked
contentOwner: admin
cq-gepid: scene7/using/WS74CBEE79-DBB3-464b-8E46-56012F9BC5A8,scene7/using/WS1C9438D8-3730-45b6-A3E0-2DA7E85733B5,scene7/using/WS2BF14BF0-BE02-4b02-B1CE-378F2A6ADF5F,scene7/using/WSBE79FB73-BE0B-4f23-BFFD-BD7EF9FDAE18,scene7/using/WS0311686C-39CC-46d8-99EE-07562BF148AE,scene7/using/WS19DD8DA6-A8E6-4c77-B2F9-A9EF0FB59317,scene7/using/WS810E2BCA-DCB0-4aad-9A0F-EC613FF05679,scene7/using/WSD7D0841C-092B-445c-B680-4257E83019EF
cq-lastmodifiedby: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: f7acd7a4-b5b1-4996-8368-1c83e1b3dce6
donotlocalize: false
gep-conversion-script-version: head1_20111213
lr-creator: admin
lr-lastmodified: 2018-05-21T08 23 42.393-0400
lr-lastmodifiedby: admin
moreHelpPaths: /content/help/en/experience-manager/morehelp/upload_and_publish_assets;/content/help/en/experience-manager/morehelp/upload_and_publish_assets
pagelayout: video
sidecolumn: left
sortdate: 2018-05-21T08 23 00.000-0400
index: y
internal: n
snippet: y
---

# Checking job files{#checking-job-files}

To monitor file uploads to the Scene7 Publishing System and files you publish to Scene7 servers, SPS offers the Jobs page. You can review upload and publish jobs on the Jobs page, check the status of jobs, and cancel publishing jobs from this page. You can also schedule upload and publishing jobs.

When you upload assets, a spinning icon appears next to the Jobs menu, indicating a job is in progress, and the number of files in progress. You can click the icon to see more information about the active job.

>[!NOTE]
>
>A list of your recently published jobs is also available on the Recent Activity page. Click Recent on the Global Navigation bar to open this page.

## About the Jobs page {#about-the-jobs-page}

Select the Jobs button on the Global Navigation bar to open the Jobs page. By default, jobs are listed starting with the most recent.

Jobs are listed in these categories on the History tab of the Jobs page:

**Job Type** An icon indicates the job type: Upload and Publish are the most common job types.

**Job Name** The name of the job. The name includes the user-entered portion of the name and the date-and-time stamp.

**Started** When the job started.

**Total** The number of files transferred.

**W (warnings)** The number of warnings in the job (if any). Warnings indicate problems with the job that did not affect overall job completion. These warnings can usually be ignored because they report on hidden files. For example, .DS_store files (Macintosh) and Thumbs.db files (Windows) contain information about how to display image files to users. Warning entries regarding these files, however, can be ignored because they don’t pertain to how these files are used in Scene7. You can double-click a job name to get detailed information about warnings.

**E (errors)** Lists the number of errors in the job (if any). You can double-click a job name to get detailed information about errors.

**Duration** How long it took to complete the job.

**Status** Shows the status of the job.

**Destination** For upload jobs, the company name and folder to which the files were uploaded. This category doesn’t apply to publish jobs.

**Submitted By** Lists who uploaded the assets.

***Note**: You can cancel in-progress publish and upload jobs by clicking the Cancel button next to the progress bar.*

## Changing views on the Jobs page {#changing-views-on-the-jobs-page}

Use these techniques to sort jobs or change your view of the History tab of the Jobs page:

**Sorting** Select a column name to sort the list by a particular column. You can select the switch beside the column name to sort in descending or ascending order.

**Date Range** Select the Date Range menu and choose an option to narrow the list of jobs to the current date, the previous week, or the previous month. Choose Custom Date Range to enter a specific date range.

**Job Type** Select the Job Type menu and choose Publish or Upload to narrow the list to publish jobs or upload jobs. Choose All to see both types of jobs.

**Show** Choose Show > My Jobs or Show > All Jobs to narrow the list to jobs you ordered or jobs that people in your company ordered.

## Viewing, copying, or printing a Job Details report {#viewing-copying-or-printing-a-job-details-report}

Double-click the name of a report on the Jobs page to open the Job Details page. This page provides a summary report about the files in the job. Click View Detail to see an entry’s SPS ID, destination path, and status information. If you uploaded a PDF or PostScript file that requires fonts that are not available in SPS, the report lists the missing fonts.

You can copy this information to the Clipboard.

1. Double-click the name of a report on the Jobs page to open the Job Details page.
1. Click View Detail to get a detailed report about an entry.
1. Click Copy to Clipboard.

## Handling recurring upload and publish jobs {#handling-recurring-upload-and-publish-jobs}

Recurring upload and publish jobs that you create on the Upload and Publish pages are listed on the Scheduled tab of the Jobs page. You can edit and delete recurring jobs on the Scheduled tab.

Select the Jobs button on the Global Navigation bar and, on the Jobs page, select the Scheduled tab to edit and delete recurring jobs.

>[!NOTE]
>
>You can filter the job list on the Scheduled tab with the Job Type and Show menus. Choose a Job Type to narrow the list to publish jobs of a specific kind. Choose a Show option to display jobs you created or jobs created by everyone in your company.

### Editing, deleting, pausing, and resuming recurring jobs {#editing-deleting-pausing-and-resuming-recurring-jobs}

Select a recurring job on the Jobs page and follow these instructions to edit or delete it:

**Editing a recurring job** Select the Edit button and enter schedule information in the Edit Scheduled Job dialog box. If you want the job to recur at an interval of your choice, choose Repeat > Custom.

See [Creating a custom upload or publish job time interval](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

**Deleting a recurring job** Select the Delete button.

**Pausing (and resuming) a recurring job** In the Active column, deselect a check box to pause a job; select a check box to resume a job that was paused.

### Creating a custom upload or publish job time interval {#creating-a-custom-upload-or-publish-job-time-interval}

To create a custom time interval for an upload (via FTP) or a publish job, choose Repeat &gt; Custom on the Upload or Publish page. Then enter numbers and wildcards in the Rule box to describe a time interval for the upload or publish jobs to recur.

The syntax for describing custom upload and publish time intervals in the Rule box is:

[seconds] [minutes] [hour of day] [day of month] [month] [day of week]

For example, `0 15 10 * * ?` schedules a job at 10:15.00 every day.

The following tables and list explain how to describe a time interval in the Rule box.

This table shows the time increments, their allowed values, and the wildcards they support:

<table cellpadding="4" cellspacing="0"> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e12012" valign="top" width="NaN%"><p>Time increments</p></th> 
   <th class="cellrowborder" id="d19e12015" valign="top" width="NaN%"><p>Values allowed</p></th> 
   <th class="cellrowborder" id="d19e12018" valign="top" width="NaN%"><p>Comments</p></th> 
   <th class="cellrowborder" id="d19e12021" valign="top" width="NaN%"><p>Wildcards supported</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e12012 " valign="top" width="NaN%"><p>Seconds</p></td> 
   <td class="cellrowborder" headers="d19e12015 " valign="top" width="NaN%"><p>0-59</p></td> 
   <td class="cellrowborder" headers="d19e12018 " valign="top" width="NaN%"><p></p></td> 
   <td class="cellrowborder" headers="d19e12021 " valign="top" width="NaN%"><p>, - * / </p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e12012 " valign="top" width="NaN%"><p>Minutes</p></td> 
   <td class="cellrowborder" headers="d19e12015 " valign="top" width="NaN%"><p>0-59</p></td> 
   <td class="cellrowborder" headers="d19e12018 " valign="top" width="NaN%"><p></p></td> 
   <td class="cellrowborder" headers="d19e12021 " valign="top" width="NaN%"><p>, - * / </p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e12012 " valign="top" width="NaN%"><p>Hours</p></td> 
   <td class="cellrowborder" headers="d19e12015 " valign="top" width="NaN%"><p>0-23</p></td> 
   <td class="cellrowborder" headers="d19e12018 " valign="top" width="NaN%"><p>Note the use of a 24-hour clock.</p></td> 
   <td class="cellrowborder" headers="d19e12021 " valign="top" width="NaN%"><p>, - * / </p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e12012 " valign="top" width="NaN%"><p>Day of the month</p></td> 
   <td class="cellrowborder" headers="d19e12015 " valign="top" width="NaN%"><p>1-31</p></td> 
   <td class="cellrowborder" headers="d19e12018 " valign="top" width="NaN%"><p>You cannot specify a numeric value for both “day of the month” and “day of the week.” One of these fields must use a ? wildcard character.</p></td> 
   <td class="cellrowborder" headers="d19e12021 " valign="top" width="NaN%"><p>, - * / ? L C</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e12012 " valign="top" width="NaN%"><p>Month</p></td> 
   <td class="cellrowborder" headers="d19e12015 " valign="top" width="NaN%"><p>1-12 or Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Sep, Oct, Nov, Dec</p></td> 
   <td class="cellrowborder" headers="d19e12018 " valign="top" width="NaN%"><p>Values are case sensitive. </p></td> 
   <td class="cellrowborder" headers="d19e12021 " valign="top" width="NaN%"><p>, - * / </p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e12012 " valign="top" width="NaN%"><p>Day of the week</p></td> 
   <td class="cellrowborder" headers="d19e12015 " valign="top" width="NaN%"><p>Mon, Tue, Wed, Thu, Fri, Sat, Sun</p></td> 
   <td class="cellrowborder" headers="d19e12018 " valign="top" width="NaN%"><p>Values are case sensitive. You cannot specify a numeric value for both “day of the month” and “day of the week.” One of these fields must use a ? wildcard character.</p></td> 
   <td class="cellrowborder" headers="d19e12021 " valign="top" width="NaN%"><p>, - * / ? L C #</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e12012 " valign="top" width="NaN%"><p>Year (optional)</p></td> 
   <td class="cellrowborder" headers="d19e12015 " valign="top" width="NaN%"><p>Empty or 1970-2099</p></td> 
   <td class="cellrowborder" headers="d19e12018 " valign="top" width="NaN%"><p></p></td> 
   <td class="cellrowborder" headers="d19e12021 " valign="top" width="NaN%"><p>, - * / </p></td> 
  </tr> 
 </tbody> 
</table>

This table describes the wildcard characters that are allowed in the Rule box and how to use them:

<table cellpadding="4" cellspacing="0"> 
 <thead align="left"> 
  <tr> 
   <th class="cellrowborder" id="d19e12122" valign="top" width="NaN%"><p>Wildcard character</p></th> 
   <th class="cellrowborder" id="d19e12125" valign="top" width="NaN%"><p>Name</p></th> 
   <th class="cellrowborder" id="d19e12128" valign="top" width="NaN%"><p>What it describes</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td class="cellrowborder" headers="d19e12122 " valign="top" width="NaN%"><p>*</p></td> 
   <td class="cellrowborder" headers="d19e12125 " valign="top" width="NaN%"><p>Asterisk</p></td> 
   <td class="cellrowborder" headers="d19e12128 " valign="top" width="NaN%"><p>All values (for example, “every minute”).</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e12122 " valign="top" width="NaN%"><p>?</p></td> 
   <td class="cellrowborder" headers="d19e12125 " valign="top" width="NaN%"><p>Question mark</p></td> 
   <td class="cellrowborder" headers="d19e12128 " valign="top" width="NaN%"><p>No specific value (for example, “any minute within the specified hour”).</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e12122 " valign="top" width="NaN%"><p>,</p></td> 
   <td class="cellrowborder" headers="d19e12125 " valign="top" width="NaN%"><p>Comma</p></td> 
   <td class="cellrowborder" headers="d19e12128 " valign="top" width="NaN%"><p>Additional values (for example, “Monday and Wednesday”).</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e12122 " valign="top" width="NaN%"><p>-</p></td> 
   <td class="cellrowborder" headers="d19e12125 " valign="top" width="NaN%"><p>Hyphen</p></td> 
   <td class="cellrowborder" headers="d19e12128 " valign="top" width="NaN%"><p>Range of values (for example, “Monday through Friday”).</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e12122 " valign="top" width="NaN%"><p>/</p></td> 
   <td class="cellrowborder" headers="d19e12125 " valign="top" width="NaN%"><p>Forward slash</p></td> 
   <td class="cellrowborder" headers="d19e12128 " valign="top" width="NaN%"><p>Increments (for example, “every 15 minutes”).</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e12122 " valign="top" width="NaN%"><p>L</p></td> 
   <td class="cellrowborder" headers="d19e12125 " valign="top" width="NaN%"><p>Capital L</p></td> 
   <td class="cellrowborder" headers="d19e12128 " valign="top" width="NaN%"><p>Last “day of the month” or “day of the week” (available for these fields only). For example, if the month is January, an L value for the “day of the month” field schedules the job for January 31.</p><p>For the “day of the week” field, you can enter this character alone to schedule the job on Saturday. You can use it with a number (for example, 6L) to specify the last Friday of the month.</p><p>Do not specify L with the comma or hyphen wildcards.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e12122 " valign="top" width="NaN%"><p>#</p></td> 
   <td class="cellrowborder" headers="d19e12125 " valign="top" width="NaN%"><p>Number sign</p></td> 
   <td class="cellrowborder" headers="d19e12128 " valign="top" width="NaN%"><p>“Nth” weekday of the month (available for the “day of the week” field only).</p><p>For example, 6#3 in the “day of the week” field specifies the third Friday of the month. The 6 denotes “Friday” (the sixth day of the week) and the 3 denotes the third occurrence in the month.</p></td> 
  </tr> 
  <tr> 
   <td class="cellrowborder" headers="d19e12122 " valign="top" width="NaN%"><p>C</p></td> 
   <td class="cellrowborder" headers="d19e12125 " valign="top" width="NaN%"><p># Capital C</p></td> 
   <td class="cellrowborder" headers="d19e12128 " valign="top" width="NaN%"><p>First calendar “day of the month” or “day of the week” (available for these fields only). For example, specifying a value of 1C for “day of the month” schedules the first day in the calendar that occurs on or after the fifth.</p><p>For the “day of the week” field, specifying 1C schedules the first day in the calendar that occurs on or after Sunday</p></td> 
  </tr> 
 </tbody> 
</table>

This list gives examples of describing time intervals in the Rule box:

* 0 0 12 &#42; &#42; ?: Noon every day
* 0 15 10 ? &#42; &#42;: 10:15 am every day
* 0 0/5 14 &#42; &#42; ?: Every 5 minutes between 2:00 and 2:55 pm every day
* 0 0/5 14,18 &#42; &#42; ?: Every 5 minutes between 2:00 and 2:55 pm every day and every 5 minutes between 6:00 and 6:55 pm every day
* 0 10,44 14 ? 3: Wed at 2:10 pm and 2:44 pm every Wednesday in March
* 0 15 10 ? &#42;: Mon-Fri at 10:15 am every weekday
* 0 15 10 20 &#42; ?: At 10:15 am on the 20th day of every month
* 0 15 10 L &#42; ?: At 10:15 am on the last day of every month
* 0 15 10 ? &#42; 6L: At 10:15 am on the last Friday of every month
* 0 15 10 &#42; &#42; 6#3: At 10:15 am on the third Friday of every month

## Using an upload or publish job as a trigger {#using-an-upload-or-publish-job-as-a-trigger}

When you upload assets via FTP or run a publish job, you can schedule a subsequent job to begin as soon as the upload is complete. (If other jobs are scheduled to begin at that time, the job you schedule here is queued behind them.) The new job sends a notification to the address you specify so that code at that location can be triggered. This follow-on upload job is given the same name as the current upload job, but with the prefix _Pub.

To make one upload or publish job trigger another job, select Advanced on the Upload or Publish page. Then enter the URL in the HTTP Notification text field.
