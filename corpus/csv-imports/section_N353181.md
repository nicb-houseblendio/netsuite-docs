---
id: "section_N353181"
type: "section"
title: "Canceling a CSV Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Step Five Save Mapping & Start Import > Canceling a CSV Import"
parent: "section_N350233"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353181.html"
anchors: ["procedure_N353193"]
sha256: "3fafe76551b0292dc285da4b1adef45e4fcbb5b58cf86cd33ea8fb083e1deea2"
---

On the CSV import job status page, you can cancel a CSV import job before it is completed. For example, you may need to cancel an import job that you have discovered includes incorrect data. Or, you may want to cancel a large CSV import job to allow smaller jobs to be processed first, and then restart the larger job later.

#### To cancel a CSV import: {#procedure_N353193}

1.  Go to Setup > Import/Export > View CSV Import Status.
    
2.  Click **Cancel** in the far right column.
    
    -   The Cancel link is available for jobs that are Pending or Processing.
        
    -   Administrators can cancel any pending or processing job, but other users can only cancel their own.
        
3.  The Status column will say 'Canceling' until it's done.
    
4.  As soon as a job is canceled, the next job in the queue, if there is one, starts right away.
    

Other results of import job cancellation vary depending on the job's status when you click **Cancel**.

-   If the job was Pending, it's removed from the Job Status page after it's canceled.
    
-   If a job's status is Processing when you cancel it, the following occurs after cancellation is complete:
    
    -   The Status column says 'Canceled'.
        
    -   The Message column lists the number of records imported before cancellation.
        
    -   The CSV Response column has a link to a `results.csv` file containing any rows that were processed before cancellation but had errors, and any rows not processed before cancellation.
        
    -   An email status notification is sent to the email address used to log in when the import was initiated.
        
        -   This email includes the number of imported and not imported CSV file records.
            
        -   The number of records not imported includes both records with errors and records that were not processed due to the cancellation.
            
        -   For more details, see [CSV Import Email Notifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350581.html#bridgehead_N353043).
            

Note:

Because the next import job in the queue begins immediately after an import job's cancellation is complete, if you need to cancel multiple import jobs, you should cancel them in reverse order, beginning with a job that hasn't started processing yet.

### Related Topics

-   [Step Five Save Mapping & Start Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350233.html)
-   [Checking CSV Import Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350581.html)
-   [CSV Import Error Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353446.html)
-   [Deleting Incorrect CSV Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353700.html)
-   [Working with Saved CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353796.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
