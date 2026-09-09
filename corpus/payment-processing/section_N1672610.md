---
id: "section_N1672610"
type: "section"
title: "Rollback"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Managing Electronic Bank Payments > Rollback"
parent: "section_N1669310"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672610.html"
anchors: ["procedure_N1672629"]
sha256: "e98cc734129ce89022053feffcff7bd3fa784da2c9444e64f58de78a922090dd"
---

In payment rollback, the payment file is deleted and all its associated payments are deleted. Credits aren't included in a payment rollback. Any credit transactions are still applied to a bill or invoice.

Important:

Use Rollback to delete payments created using the Electronic Bank Payments SuiteApp. Deleting payments directly from the payment record may result to duplicate transactions in payment batches and the EP\_00016 error in your next payment run.

Note:

You can roll back payments within 24 hours after the payment file has been generated if the bank has not yet processed the associated payment file.

#### To cancel payments: {#procedure_N1672629}

1.  Go to Payments > Payment Processing > Payments File Administration.
    
2.  Click View next to the payment file that you want to cancel.
    
3.  Click **Rollback**. On the confirmation message that appears, click **OK**.
    
    The value in the **File Processed?** field changes to **Queued**.
    
    You can change the priority of the rollback process for the payment file by clicking **Edit**, and changing the value in the **Priority Queue** field.
    
4.  Click **Refresh** until the value in the **File Processed?** field changes to **Canceled**. The payment file is deleted and all its associated payments are canceled.
    

### Related Topics

-   [Processing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665126.html)
-   [Managing Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669310.html)
-   [Setting Up Multiple Script Queues or Processors to Generate Payment File Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669543.html)
-   [Setting Up Multi-Currency Payments Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670158.html)
-   [Viewing Electronic Bank Payment Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670421.html)
-   [Sending Payment Notifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672006.html)
-   [Reversing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672279.html)
-   [Reprocessing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672857.html)
-   [Recreating a Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3727317578.html)
-   [Removing Transactions from Payment Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4750490863.html)
-   [Verifying Issued Checks with Positive Pay](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673097.html)
-   [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html)
-   [Changing the Priority of a Queued Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1674867.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
