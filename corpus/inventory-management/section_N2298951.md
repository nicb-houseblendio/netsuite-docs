---
id: "section_N2298951"
type: "section"
title: "Creating Calculated Inventory Counts"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Inventory Count > Creating Calculated Inventory Counts"
parent: "section_N2296970"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2298951.html"
anchors: ["procedure_N2298990", "procedure_N2299134", "bridgehead_N2299211"]
sha256: "e4a3a4ed6da0699e7116f1ee90dad26dd23f7692f7dde54a8c824a8d26f956f3"
---

After the count date and interval are recorded for an item, NetSuite uses them to calculate when a count is required. When a new count is due to be recorded, it shows in the list on the Create Inventory Count page.

#### To create calculated inventory counts: {#procedure_N2298990}

1.  Go to _Transactions > Inventory > Create Inventory Count_.
    
2.  Select a location.
    
3.  Enter or select a **Count Start Date**.
    
    This filters the list to show only items that require a count on or after the date entered in this field.
    
4.  Enter or select a **Count End Date**.
    
    This filters the list to show only items that require a count on or before the date entered in this field.
    
5.  Optionally choose a Item classification to filter the list.
    
6.  Check the **Count Bin Rows With Zero Quantity** box to include in the list items with an on-hand count of zero.
    
7.  Check the **Sort Rows by Bin** box to sort the item list by bin number instead of by item number. This can be useful to count all items in a specific area of a warehouse.
    
8.  Select an account to post variances to. This is typically an expense account.
    
    You can choose an account to show in this field by default. For details, read [Setting Up Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2297156.html)
    
9.  Check the box in the **Select** column next to each item you want to count.
    
    Note:
    
    If you use Bin Management, an item does not appear in the list if it uses bins and has no prior transaction history.
    
10.  Click **Submit**. When you click **Submit**, the inventory count transaction is recorded, but not started.
     

After an inventory count is on record, it has an Open status and is a non-posting transaction.

#### To edit an inventory count: {#procedure_N2299134}

1.  Go to _Transactions > Inventory > Enter Inventory Count > List_.
    
2.  Click **Edit** next to the count you want to change.
    
3.  Make necessary edits to the record.
    
4.  Click **Save**.
    

## Starting an Inventory Count {#bridgehead_N2299211}

Read more about starting an inventory count in the topic [Working with an Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2299731.html).

### Related Topics

-   [Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2296970.html)
-   [Setting Up Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2297156.html)
-   [Creating Manual Inventory Counts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2299331.html)
-   [Working with an Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2299731.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
