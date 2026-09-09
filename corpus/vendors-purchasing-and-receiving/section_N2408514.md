---
id: "section_N2408514"
type: "section"
title: "Viewing the Status of a Purchase Order"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Purchasing > Purchase Order Management > Viewing the Status of a Purchase Order"
parent: "section_N2399585"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2408514.html"
anchors: ["procedure_N2408534", "procedure_N2408584"]
sha256: "8f1ed044a5e645d93eb35ea081fb9c740ca689b479e6f72247c85b25214fb7d0"
---

With Advanced Receiving, you can receive purchase orders or parts of purchase orders separately from bills. Your purchase orders have statuses that reflect where the orders are in the receiving and billing process.

#### To enable advanced receiving: {#procedure_N2408534}

1.  Go to _Setup > Company > Enable Features_.
    
2.  Click the **Transactions** subtab.
    
3.  Check the **Advanced Receiving** box.
    
4.  Click **Save**.
    

#### To view the status of a purchase order: {#procedure_N2408584}

1.  Go to _Transactions > Purchases/Vendors > Enter Purchase Orders > List_.
    
2.  On the **Purchase Orders** page, the order **Status** column displays the order status.
    
    Note:
    
    If some lines are fully billed, and at least one is closed, the status of the transaction is closed.
    
    If some lines are fully billed, others closed, but there is at least one open line, note the following. The status of the transaction is the status of that open line. Open implies pending, received, partially received, and partially billed.
    
    -   With the Advanced Receiving Feature off:
        
        -   **Pending Supervisor Approval** - The purchase request has not been approved.
            
        -   **Rejected By Supervisor** - The purchase request has been declined.
            
        -   **Pending Receipt** - The purchase is pending entry of a bill, including partially billed purchase orders.
            
        -   **Partially Received** - The purchase has been partially billed.
            
        -   **Received** - The purchase is completely received and billed.
            
        -   **Closed** - The purchase order has been canceled.
            
    -   With the Advanced Receiving Feature on:
        
        -   **Pending Supervisor Approval** - The purchase request has not been approved.
            
        -   **Rejected By Supervisor** - The purchase request has been declined.
            
        -   **Pending Receipt** - The purchase order is pending receipt of items ordered.
            
        -   **Partially Received** - Not all items on this order have been received, regardless of billing status.
            
        -   **Pending Bill** - This order is pending the entry of a bill, including partially billed purchases.
            
        -   **Pending Billing/Partially Received** - Not all items on this order have been received and are pending the entry of a bill, including partially billed purchases.
            
        -   **Fully Billed** - All items on the order have been received and billed.
            
        -   **Closed** - The purchase order has been canceled.
            
3.  Click **View** to open the order.
    
    Click **Edit** to make changes to the order.
    

To see what has already been received and billed for a purchase order, click the Related Records subtab and click Receipts & Bills.

### Additional Information

-   [Receiving Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2410585.html)

### Related Topics

-   [Setting Purchasing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400174.html)
-   [Entering a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400504.html)
-   [Bulk Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2402825.html)
-   [Ordering Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403352.html)
-   [Billing a Purchase Order With Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403862.html)
-   [Editing a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2404305.html)
-   [Printing a Tax ID or Resale Number on Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4746558953.html)
-   [Purchase Order Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2407704.html)
-   [Purchase Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2399585.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
