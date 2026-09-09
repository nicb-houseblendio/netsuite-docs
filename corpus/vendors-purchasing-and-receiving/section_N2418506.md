---
id: "section_N2418506"
type: "section"
title: "Creating a Landed Cost Item"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Expenses > Landed Cost > Creating a Landed Cost Item"
parent: "section_N2416930"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2418506.html"
anchors: ["procedure_N2418574"]
sha256: "0dc42082d1ec18be757bcb8908eab7aef75f008970d0901bd59d8fac2d750012"
---

To count a charge on a vendor bill as a landed cost, you must select an item on the bill. If you enter a bill that is not associated with an inventory item, you must associate it with a landed cost item you create. An example of a landed cost item is the item 'Freight.'

For example, you use a freight company to deliver inventory items you need. For each shipment, you receive two separate bills. One from the vendor that charges you for the items. One from the freight company that charges you only for transporting the items.

When entering the bill, you must select an item to associate the freight expense as a landed cost. Since the freight bill is not associated with an inventory item, you must create a landed cost item record for Freight.

When creating landed cost items, note the following:

-   Landed Cost items should be named appropriately based on the type of charge, such as landed cost categories like Insurance and Handling.
    
-   The expense account noted should match the corresponding landed cost category or be a contra account shown in the same section of the Income Statement. Ultimately, this expense account is zeroed due to the following General Ledger impact:
    

PO Receipt:

CR - Expense Account - The value in the landed cost category

Separate Vendor Bill:

DB - Expense Account or Contra - Amount received from carrier for freight costs

#### To create a landed cost item: {#procedure_N2418574}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click the item type you want to create to track the landed cost.
    
3.  In the **Item Name/Number** field, enter a unique name for the landed cost expense, such as Freight.
    
4.  On the **Accounting** subtab, in the **Expense Account** field, select the account on which you want to record freight and other such charges.
    
5.  To fill out additional details on the item record, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).
    
6.  Click **Save**.
    

When you create a bill, you can select the landed cost item and track the expense on the bill as a landed cost.

### Additional Information

-   [Vendor Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2370131.html)
-   [Receiving Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2410585.html)

### Related Topics

-   [Landed Cost Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2417056.html)
-   [Landed Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2417902.html)
-   [Landed Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2417902.html)
-   [Setting up an Item Record for Landed Cost](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2418189.html)
-   [Entering Landed Cost on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2418831.html)
-   [Landed Cost and Taxation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554390337.html)
-   [Landed Cost Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2419793.html)
-   [Landed Cost and Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2420792.html)
-   [Landed Cost Allocation per Line](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3728979515.html)
-   [Estimated Landed Cost](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4576786578.html)
-   [Landed Cost](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2416930.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
