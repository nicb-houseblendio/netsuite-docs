---
id: "section_N1672857"
type: "section"
title: "Reprocessing Payments"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Managing Electronic Bank Payments > Reprocessing Payments"
parent: "section_N1669310"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672857.html"
anchors: ["procedure_N1672869"]
sha256: "f06b2e7f4703cdc43531036fd7de02a04458c6fb26a1e6a06642aa83317403de"
---

You can reprocess PFA (Payment File Administration) records with Cancelled or Processed with Errors status.

Note:

Reprocessing of a payment file with a bill that has been placed on payment hold shows an error on the Payment File Administration record.

#### To reprocess canceled payments: {#procedure_N1672869}

1.  Go to Payments > Payment Processing > Payments File Administration.
    
2.  Click View next to the payment file that you want to reprocess.
    
3.  Click **Reprocess**. On the confirmation message that appears, click **OK**.
    
    The value in the **File Processed?** field changes to **Queued**.
    
    You can change the priority of the reprocess task for the payment file by clicking **Edit**, and changing the value in the **Priority Queue** field.
    
4.  Click **Refresh** until the value in the **File Processed?** field changes to **Processed**. The payment file is recreated and all its associated payments are processed.
    

### Related Topics

-   [Processing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665126.html)
-   [Managing Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669310.html)
-   [Setting Up Multiple Script Queues or Processors to Generate Payment File Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669543.html)
-   [Setting Up Multi-Currency Payments Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670158.html)
-   [Viewing Electronic Bank Payment Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670421.html)
-   [Sending Payment Notifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672006.html)
-   [Reversing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672279.html)
-   [Rollback](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672610.html)
-   [Removing Transactions from Payment Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4750490863.html)
-   [Verifying Issued Checks with Positive Pay](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673097.html)
-   [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html)
-   [Changing the Priority of a Queued Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1674867.html)
-   [Recreating a Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3727317578.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
