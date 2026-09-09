---
id: "section_N1719864"
type: "section"
title: "Creating a Transaction VSOE Bundle"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > Creating VSOE Bundles > Creating a Transaction VSOE Bundle"
parent: "section_N1719451"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1719864.html"
anchors: ["procedure_N1719884"]
sha256: "e95e76ce34e2667a4fce5b21e5db70146fff3f13299ebbf60e440a209a04f696"
---

Instead of creating an item group to bundle vendor-specific objective evidence (VSOE) items, you can designate an entire sales transaction as a VSOE bundle. If you include VSOE item groups in a transaction VSOE bundle, the items are processed as individual items rather than a group.

#### To create a transaction bundle: {#procedure_N1719884}

1.  Go to a new transaction form for one of the following:
    
    -   Cash Sale
        
    -   Credit Memo
        
    -   Invoice
        
    -   Refund
        
    -   Return Authorization
        
    -   Sales Order
        
2.  Check the **Transaction Is VSOE Bundle** box on the **Accounting** subtab.
    
3.  Add items to the transaction.
    
    You must add at least two items.
    
    You can't add an item group that is a VSOE bundle.
    
4.  Complete the remainder of the transaction as necessary, and click **Save**.
    

Note:

If a sales order isn't marked **Transaction is VSOE Bundle**, the sales order allocation and delivered flags don't propagate to invoices for the sales order.

Now, items on the transaction that have VSOE settings can be processed for VSOE. See [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html).

### Related Topics

-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html)
-   [Creating VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1719451.html)
-   [Creating an Item Group VSOE Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1719644.html)
-   [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
