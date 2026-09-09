---
id: "section_N1672279"
type: "section"
title: "Reversing Payments"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Managing Electronic Bank Payments > Reversing Payments"
parent: "section_N1669310"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672279.html"
anchors: ["procedure_N1672306"]
sha256: "7497175afb223a528ef476c575daf4a48235208eb1d0d23b3579a79e2b07d489"
---

You can reverse payments if the bank has not yet processed the associated payment file. When you reverse a payment, a new payment file is created and the payments are reprocessed. However, any credit transactions are still applied to the bill or invoice. Full payment reversal voids all payments and the payment file is deleted. On the other hand, partial reversal voids only selected payments and a new payment file is created with the remaining payments.

Important:

Use Reverse Payments to void payments created using Electronic Bank Payments SuiteApp. Voiding payments directly from the payment record may result to duplicate transactions in payment batches and EP\_00016 error in your next payment run.

When reversing a PFA with discount payments, you must make sure that the discount accounts are set to the following default values. If the default values are not set then reversing the PFA results in the EP\_00109 error.

-   Purchase Discount Account - Purchase Discounts
    
-   Sales Discount Account - Sales Discounts
    

Note:

The Reverse Payments feature is only available to payment file administration records that were processed through Bill Payment Processing, Invoice Payment Processing and Instant Bank File Generation. Reversing a payment file voids the bill payment transaction using reversing journals, regardless if the Void Transactions Using Reversing Journals preference is disabled. For more information about the Void Transactions Using Reversing Journals preference, see [Journal Entry Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469391.html).

#### To reverse payments: {#procedure_N1672306}

1.  Go to Payments > Payment Processing > Payments File Administration.
    
2.  Click View next to the payment file that you want to recreate.
    
3.  Click **Reverse Payments**.
    
4.  In the **Reversal Reason** field under Payment Information, enter text that explains why you are reversing the payments. This text should be displayed in the **Memo** field of all the payment transactions in the list. However, if the reason for reversal is different for each payment, you can leave this field blank. To enter a reversal reason for the individual payments in the Select Transactions list, see step eight.
    
5.  In the **Reversal Date** field, enter the date for the reversing journal entry that is created after performing the payment reversal.
    
    Note:
    
    If you enter a past date that does not fall within an existing open posting period, the value in the **Posting Period** field changes to the earliest posting period. If you enter a future date that doesn't fall within an existing open posting period, the value in the **Posting Period** field changes to the last posting period.
    
6.  In the **Reversal Posting Period** field, select the accounting period to which the reversing journal entry should be posted. Only open posting periods are displayed in this list.
    
7.  In the **Select** column on the **Select Transactions** subtab, check the box next to each payment that you want to reverse. If you don't select all payments, partial reversal is applied.
    
8.  If each payment has a different reason for reversal, enter the reason in the **Reversal Reason** column. It overrides any text you previously entered in the **Reversal Reason** field under Payment Information.
    
9.  Click **Submit**. The Payment File Administration form is displayed. Notice that the status of the **File Processed?** field is changed to **Queued**.
    
    Note:
    
    You can change the priority of the reversal process for the payment file by clicking **Edit**, and changing the value in the **Priority Queue** field.
    
10.  Click **Refresh** until the value in the **File Processed?** field changes to **Processed**.
     
     The selected payment transactions are voided with a reversal journal entry. A new payment file is created, and an email is sent to you confirming that the process has been completed.
     
     Note:
     
     If all payments in the payment file are selected for reversal, the status of the **File Processed?** field changes to Canceled. If payments in the payment file were partially reversed, the **Status Summary** field is updated to the original number of transactions paid and the original number of transactions marked for payment.
     

### Related Topics

-   [Processing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665126.html)
-   [Managing Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669310.html)
-   [Setting Up Multiple Script Queues or Processors to Generate Payment File Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669543.html)
-   [Setting Up Multi-Currency Payments Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670158.html)
-   [Viewing Electronic Bank Payment Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670421.html)
-   [Sending Payment Notifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672006.html)
-   [Rollback](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672610.html)
-   [Reprocessing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672857.html)
-   [Recreating a Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3727317578.html)
-   [Removing Transactions from Payment Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4750490863.html)
-   [Verifying Issued Checks with Positive Pay](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673097.html)
-   [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html)
-   [Changing the Priority of a Queued Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1674867.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
