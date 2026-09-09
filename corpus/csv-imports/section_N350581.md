---
id: "section_N350581"
type: "section"
title: "Checking CSV Import Status"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Step Five Save Mapping & Start Import > Checking CSV Import Status"
parent: "section_N350233"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350581.html"
anchors: ["bridgehead_N350618", "bridgehead_N353043"]
sha256: "68a8de35d0010edae3c352a5eb284ba019c4ac4afe2eb2f241d2d0fe69580d90"
---

You can check the status of an import job on the Job Status page. For details, see [Viewing the CSV Import Job Status Page](#bridgehead_N350618).

After your import job finishes, you'll get an email at the address you used to log in. The email tells you the status, how many records were imported, and how many weren't. For details, see [CSV Import Email Notifications](#bridgehead_N353043).

## Viewing the CSV Import Job Status Page {#bridgehead_N350618}

To see the Job Status page, go to _Setup > Import/Export > View CSV Import Status_.

For each import, the Job Status page shows:

-   The date the import was started.
    
-   The import job name, by default: <import type> - <CSV file name> - <your email address>. Scripted imports can use a different name.
    
-   The current status: Pending, Processing, Completed, or Canceled.
    
    There's also a less common Retry status, which occurs if the import stops because of an infrastructure issue. When that's fixed, the import usually starts again from where it stopped.
    
-   Percentage of the import that is complete.
    
-   A message showing how many records were imported out of the total (For example, '200 records of 205 imported').
    
-   (If your account uses multiple queues:) The queue number (1-5) for the job. The default is 1, but you can change it in [Step Two Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344550.html) of the Import Assistant. See also [Queue Number](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751039561.html).
    
-   For pending and processing jobs, there's a Cancel link. Administrators can cancel any job, but other users can only cancel their own.
    
-   For completed and canceled jobs, a link to a `results.csv` file that includes any records not processed due to errors or cancellation.
    
    -   The `results.csv` file lets you fix errors and rerun the import for any records that didn't go through. See [Post Processing Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353446.html#bridgehead_N353565).
        
    -   Anyone with access to the Job Status page can see all import jobs, but most users can only download `results.csv` files for their own jobs. Only administrators can get `results.csv` files for other users' jobs.
        
    -   The CSV response also tells you if an afterSubmit script fails after the import. If that happens, the records are still created or updated. You only need to retry the user event script, not the whole import. For more information, see [AfterSubmit Script failed, record created with internalId xxx](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4568642498.html#bridgehead_1515678023).
        

CSV import job statuses are stored for 30 days and for up to a maximum of 1,000,000 jobs. Import jobs that occurred more than 30 days ago, or which exceed this number of jobs, are eventually purged. Note that this purging can be delayed for technical reasons, so it is possible to see jobs older than 30 days on the status page.

You can't manually delete jobs from the status page.

## CSV Import Email Notifications {#bridgehead_N353043}

For every CSV import job, you'll get an email at the address you used to log in. Each email has text like the following:

![Sample email.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/CSVImportEmailNotification.png)

The number of records not imported includes any records with errors for which import failed. If the import job was canceled during processing, this number also includes any records that had not yet been processed at the time of cancellation.

Note:

You can't turn off email notifications.

Note:

You won't get an email for single journal entry imports.

### Related Topics

-   [Step Five Save Mapping & Start Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350233.html)
-   [Canceling a CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353181.html)
-   [CSV Import Error Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353446.html)
-   [Deleting Incorrect CSV Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353700.html)
-   [Working with Saved CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353796.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
