---
title: Check job files
description: Learn how to check job files in Dynamic Media Classic.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
---
# Check job files{#checking-job-files}

To monitor file uploads to the Dynamic Media Classic and files you publish to Dynamic Media Classic servers, Dynamic Media Classic offers the Jobs page. You can review upload and publish jobs on the Jobs page, check the status of jobs, and cancel publishing jobs from this page. You can also schedule upload and publishing jobs.

When you upload assets, a spinning icon appears next to the Jobs menu, indicating a job is in progress, and the number of files in progress. You can select the icon to see more information about the active job.

>[!NOTE]
>
>A list of your recently published jobs is also available on the Recent Activity page. Select **[!UICONTROL Recent]** on the Global Navigation bar.

## About the Jobs page {#about-the-jobs-page}

Select **[!UICONTROL Jobs]** on the Global Navigation bar so the Jobs page opens. By default, jobs are listed starting with the most recent.

Jobs are listed in these categories on the History tab of the Jobs page:

* **[!UICONTROL Job Type]** - An icon indicates the job type: Upload and Publish are the most common job types.

* **[!UICONTROL Job Name]** - The name of the job. The name includes the user-entered portion of the name and the date-and-time.

* **[!UICONTROL Started]** - When the job started.

* **[!UICONTROL Total]** - The number of files transferred.

* **[!UICONTROL W (warnings)]** - The number of warnings in the job (if any). Warnings indicate problems with the job that did not affect overall job completion. These warnings can usually be ignored because they report on hidden files. For example, `.DS_store` files (Macintosh) and Thumbs.db files (Windows®) contain information about how to display image files to users. Warning entries regarding these files, however, can be ignored because they don’t pertain to how these files are used in Dynamic Media Classic. You can double-click a job name to get detailed information about warnings.

* **[!UICONTROL E (errors)]** - Lists the number of errors in the job (if any). You can double-click a job name to get detailed information about errors.

* **[!UICONTROL Duration]** - How long it took to complete the job.

* **[!UICONTROL Status]** - Shows the status of the job.

* **[!UICONTROL Destination]** - For upload jobs, the company name, and folder to which the files were uploaded. This category doesn’t apply to publish jobs.

* **[!UICONTROL Submitted By]** - Lists who uploaded the assets.

>[!NOTE]
>
>You can cancel in-progress publish and upload jobs by selecting the **[!UICONTROL Cancel]** button next to the progress bar.

## Change views on the Jobs page {#changing-views-on-the-jobs-page}

Use these techniques to sort jobs or change your view of the History tab of the Jobs page:

* **[!UICONTROL Sorting]** - Select a column name to sort the list by a particular column. You can select the switch beside the column name to sort in descending or ascending order.

* **[!UICONTROL Date Range]** - Select the **[!UICONTROL Date Range]** menu and choose an option to narrow the list of jobs to the current date, the previous week, or the previous month. Select **[!UICONTROL Custom Date Range]**, then enter a specific date range.

* **[!UICONTROL Job Type]** - Select the **[!UICONTROL Job Type]** menu and choose **[!UICONTROL Publish]** or **[!UICONTROL Upload]** to narrow the list to publish jobs or upload jobs. Select **[!UICONTROL All]** to see both types of jobs.

* **[!UICONTROL Show]** - Go to **[!UICONTROL Show]** > **[!UICONTROL My Jobs]** or **[!UICONTROL Show]** > **[!UICONTROL All Jobs]** to narrow the list to jobs you ordered or jobs that people in your company ordered.

## View, copy, or print a Job Details report {#viewing-copying-or-printing-a-job-details-report}

Double-click the name of a report on the Jobs page so the Job Details page opens. This page provides a summary report about the files in the job. Select **[!UICONTROL View Detail]** so you can see an entry’s Dynamic Media Classic ID, destination path, and status information. If you uploaded a PDF or PostScript file that requires fonts that are not available in Dynamic Media Classic, the report lists the missing fonts.

You can copy this information to the Clipboard.

1. Double-click the name of a report on the Jobs page.
1. On the Job Details page, select **[!UICONTROL View Detail]** to get a detailed report about an entry.
1. Select **[!UICONTROL Copy to Clipboard]**.

## Handle recurring upload and publish jobs {#handling-recurring-upload-and-publish-jobs}

Recurring upload and publish jobs that you create on the Upload and Publish pages are listed on the Scheduled tab of the Jobs page. You can edit and delete recurring jobs on the Scheduled tab.

Select the Jobs button on the Global Navigation bar and, on the Jobs page, select the **[!UICONTROL Scheduled]** tab so you can edit and delete recurring jobs.

>[!NOTE]
>
>You can filter the job list on the **[!UICONTROL Scheduled]** tab with the **[!UICONTROL Job Type]** and **[!UICONTROL Show]** menus. Select a job type so you can narrow the list to publish jobs of a specific kind. Select a **[!UICONTROL Show]** option if you want to display jobs you created or jobs created by everyone in your company.

### Edit, delete, pause, and resume recurring jobs {#editing-deleting-pausing-and-resuming-recurring-jobs}

Select a recurring job on the Jobs page and follow these instructions if you want to edit or delete it:

* **Edit a recurring job** - Select the **[!UICONTROL Edit]** button and enter schedule information in the Edit Scheduled Job dialog box. If you want the job to recur at an interval of your choice, go to **[!UICONTROL Repeat]** > **[!UICONTROL Custom]**.

See [Create a custom upload or publish job time interval](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Deleting a recurring job** - Select the **[!UICONTROL Delete]** button.

* **Pausing (and resuming) a recurring job** - In the Active column, deselect a check box to pause a job; select a check box to resume a job that was paused.

### Create a custom upload or publish job time interval {#creating-a-custom-upload-or-publish-job-time-interval}

To create a custom time interval for an upload (via FTP) or a publish job, on the Upload or Publish page, go to **[!UICONTROL Repeat]** > **[!UICONTROL Custom]**. Then enter numbers and wildcards in the Rule box describing a time interval for the upload or publish jobs to recur.

The syntax for describing custom upload and publish time intervals in the Rule box is:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

For example, `0 15 10 * * ?` schedules a job at 10:15.00 every day.

The following tables and list explain how to describe a time interval in the Rule box.

This table shows the time increments, their allowed values, and the wildcards they support:

|Time increments|Values allowed|Comments|Wildcards supported|
|--- |--- |--- |--- |
|Seconds|0-59||`, - * /`|
|Minutes|0-59||`, - * /`|
|Hours|0-23|Note the use of a 24-hour clock.|`, - * /`|
|Day of the month|1-31|You cannot specify a numeric value for both “day of the month” and “day of the week.” One of these fields must use a `?` wildcard character.|`, - * / ? L C`|
|Month|1-12 or Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Sep, Oct, Nov, Dec|Values are case-sensitive.|`, - * /`|
|Day of the week|Mon, Tue, Wed, Thu, Fri, Sat, Sun|Values are case-sensitive. You cannot specify a numeric value for both “day of the month” and “day of the week.” One of these fields must use a `?` wildcard character.|`, - * / ? L C #`|
|Year (optional)|Empty or 1970-2099||`, - * /`|


This table describes the wildcard characters that are allowed in the Rule box and how to use them:

|Wildcard character|Name|What it describes|
|--- |--- |--- |
|`*`|Asterisk|All values (for example, “every minute”).|
|`?`|Question mark|No specific value (for example, “any minute within the specified hour”).|
|`,`|Comma|Other values (for example, “Monday and Wednesday”).|
|`-`|Hyphen|Range of values (for example, “Monday through Friday”).|
|`/`|Forward slash|Increments (for example, “every 15 minutes”).|
|`L`|Capital L|Last “day of the month” or “day of the week” (available for these fields only). For example, if the month is January, an L value for the “day of the month” field schedules the job for January 31. For the “day of the week” field, you can enter this character alone to schedule the job on Saturday. You can use it with a number (for example, `6L`) to specify the last Friday of the month. Do not specify `L` with the comma or hyphen wildcards.|
|`#`|Number sign|“Nth” weekday of the month (available for the “day of the week” field only). For example, `6#3` in the “day of the week” field specifies the third Friday of the month. The `6` denotes “Friday” (the sixth day of the week) and the `3` denotes the third occurrence in the month.|
|`C`|# Capital C|First calendar “day of the month” or “day of the week” (available for these fields only). For example, specifying a value of `1C` for “day of the month” schedules the first day in the calendar that occurs on or after the fifth. For the “day of the week” field, specifying `1C` schedules the first day in the calendar that occurs on or after Sunday|

This list gives examples of describing time intervals in the Rule box:

* `0 0 12 * * ?` : Noon every day
* `0 15 10 ? * *` : 10:15 am every day
* `0 0/5 14 * * ?`: Every 5 minutes between 2:00 and 2:55 pm every day
* `0 0/5 14,18 * * ?` : Every 5 minutes between 2:00 and 2:55 pm every day and every 5 minutes between 6:00 and 6:55 pm every day
* `0 10,44 14 ? 3` : Wed at 2:10 pm and 2:44 pm every Wednesday in March
* `0 15 10 ? *` : Mon-Fri at 10:15 am every weekday
* `0 15 10 20 * ?` : At 10:15 am on the 20th day of every month
* `0 15 10 L * ?` : At 10:15 am on the last day of every month
* `0 15 10 ? * 6L` : At 10:15 am on the last Friday of every month
* `0 15 10 * * 6#3` : At 10:15 am on the third Friday of every month

## Use an upload or publish job as a trigger {#using-an-upload-or-publish-job-as-a-trigger}

When you upload assets via FTP or run a publish job, you can schedule a subsequent job to begin when the upload is complete. (If other jobs are scheduled to begin then, the job you schedule here is queued behind them.) The new job sends a notification to the address you specify so that code at that location can be triggered. This follow-on upload job is given the same name as the current upload job, but with the prefix _Pub.

To make one upload or publish job trigger another job, select **[!UICONTROL Advanced]** on the Upload or Publish page. Then enter the URL in the HTTP Notification text field.
