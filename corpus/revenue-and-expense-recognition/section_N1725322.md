---
id: "section_N1725322"
type: "section"
title: "Updating the VSOE Delivery Status on Items"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > Recognizing Revenue for VSOE Bundles > Updating the VSOE Delivery Status on Items"
parent: "section_N1720104"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725322.html"
anchors: ["procedure_N1725373"]
sha256: "3dfe478ff9fef1c6c1215257732cf8609bcf73271891ee38c0e572e8cf6d00b9"
---

You can bulk update the vendor-specific objective evidence (VSOE) delivery status for many items at one time using the Mark VSOE Delivered Status page. Only items that can have VSOE enabled are included on this page.

For VSOE, the fulfillment status of an item is separate from its delivery status. An item may be marked Delivered even if fulfillment hasn't occurred.

The VSOE delivery status is used in the following two ways:

-   To determine how the sales amount of the bundle is allocated to individual members based on their VSOE settings.
    
-   To specify that revenue recognition for the item can begin when the order has been billed.
    

#### To mark an item's VSOE delivery status: {#procedure_N1725373}

1.  Go to _Transactions > Financial > Mark VSOE Delivered Status_.
    
    This page shows all VSOE items not yet marked as Delivered. Use the filters at the top of the page to narrow the list of items displayed.
    
    For each source transaction, the transaction line number and item name are shown.
    
    You can click the link in the **Source Transaction** column to open the originating transaction.
    
2.  If you use NetSuite OneWorld, select a **Subsidiary** to associate with the status update.
    
3.  Check the box in the **Select** column for all items you want to mark as delivered.
    
    Note:
    
    The accounting period for the transaction must be open to change the delivery status. Transactions in closed periods are skipped.
    
4.  Click **Mark Delivered**.
    

When you click Mark Delivered, the Process Status page opens.

![Screenshot of Process Status page for VSOE items not yet delivered](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/RevenueExpenseRecognition/ERP-MarkDeliveredProcessStatus.png)

On the Process Status page:

-   Click **Refresh** to update the submission status.
    
-   Click the **Complete** link in the **Submission Status** column to go to the Processed Records page.
    

The Processed Records page includes links to the source transactions for the items whose VSOE delivery status was updated.

You can also access the Process Status page directly from the navigation menu. Go to _Transactions > Financial > Mark VSOE Delivered Status > Status_ to open this page.

### Related Topics

-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html)
-   [Allocating VSOE Revenue for a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720414.html)
-   [Updating VSOE Allocations and Delivery Status on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721160.html)
-   [Using VSOE on Sales Orders and Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721728.html)
-   [Billing a VSOE Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725637.html)
-   [Using VSOE with Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1726248.html)
-   [Using VSOE with Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729547.html)
-   [Resolving Undetermined VSOE Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729793.html)
-   [Posting VSOE Revenue to the General Ledger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1732506.html)
-   [Using the Residual Method of Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1733002.html)
-   [VSOE Revenue Recognition Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1736679.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
