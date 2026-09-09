---
id: "section_N1231493"
type: "section"
title: "Checking the Processing Status of Bulk Fulfilled Orders"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Fulfilling Orders > Checking the Processing Status of Bulk Fulfilled Orders"
parent: "section_N1223349"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231493.html"
anchors: []
sha256: "b34af0e8a7e378e750e57d9fdd8c9f7798c80b44aadbd17ab2f28835fc5e4f8e"
---

After submitting orders for bulk fulfillment, you can check the processing status of the orders. Orders are processed asynchronously, so you can keep working in NetSuite and check the processing status later. Submit multiple fulfillment jobs at one time and track them on the Process Status page.

You can view the processing status of previous bulk fulfill jobs by filtering by date. NetSuite shows bulk fulfillment jobs for the current date by default.

Processing starts right away or after a short delay, depending on the number of records. Processing starts immediately for fewer than 25 records. Otherwise, the bulk processing job is queued and starts after a short delay.

The Process Status page shows the following information:

-   Submission ID - A unique identifier of the bulk processing job.
    
-   Process Type - When fulfilling sales orders, the process type is Fulfill Sales Orders.
    
-   Submission Status:
    
    -   Not Started - The job has been submitted but has not yet started.
        
    -   In Progress - Records in the job are currently being processed. The Percent Complete column indicates progress.
        
    -   Complete - All records in the job have been processed. If errors occurred, the number of errors is shown in the Message column.
        
-   Percent Complete - The percentage of records processed.
    
-   Message - Indicates the number of errors that occurred during the processing.
    
-   Date Created - The date and time the bulk processing was started.
    
-   Created By - The user that submitted the bulk process job.
    

After the processing job is complete, you can view the results of the bulk processing on the Processed Records page. Information about the Processed Records page includes the result status, the result record ID, and an error message if an error occurred. The result record of fulfilling a sales order is an item fulfillment.

#### To check the processing status of bulk fulfilled orders

1.  Go to _Transactions > Sales > Fulfill Orders_ > Status.
    
2.  Click **Filters** to choose the time period for viewing bulk fulfillment jobs. NetSuite uses the current date by default.
    
3.  To view the results of a processing job, click the status link in the Submission Status column.
    
4.  If errors occurred during the processing, the number of errors is shown in the Message column. Click the link to open the Bulk Processing Errors page and view the errors.
    
5.  To view the latest status of the bulk processing jobs, click **Refresh**.
    

If you use the Pick, Pack, and Ship feature, you can check the processing status of orders when you bulk fulfill orders and set the shipping status to Picked, or Packed, or Shipped. The Process Status page is also used when bulk processing other records in NetSuite, for example, when invoicing sales orders or entering memorized transactions.

### Related Topics:

-   [Pick, Pack, and Ship Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1229796.html)
-   [Pick, Pack, and Ship Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230081.html)
-   [Fulfilling Orders Using Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230473.html)
-   [Marking an Order Packed](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230849.html)
-   [Pick, Pack, and Ship Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230081.html)
-   [Order Fulfillment Confirmation Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231778.html)
-   [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
