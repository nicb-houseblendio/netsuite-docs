---
id: "section_N2199228"
type: "section"
title: "Cost Accounting Status on Item Records"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Cost Accounting Status on Item Records"
parent: "chapter_N2191369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199228.html"
anchors: []
sha256: "89fe4cd111c79587bc1a1ab02c87796d4d252d02d854db4289d76e24ba9a0d7d"
---

Inventory and assembly item records include a **Cost Accounting Status** field that shows the state of cost accounting calculations for that item. If Multi-Location Inventory is enabled, the status is identified per location.

Note:

This field is hidden by default. Customize the item page to display this field. For more information, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).

The Cost Accounting Status indicated can be one of the following:

-   **Pending** - flagged for Cost Accounting but calculations aren't running yet
    
-   **Processing** - flagged for Cost Accounting and calculations are currently running
    
-   **Complete** - not flagged for Cost Accounting and calculations aren't running
    
-   **Failed** - Cost Accounting calculations failed
    

Note:

The **Cost Accounting Status** field is blank if cost accounting calculations have never been run for the item/location.

When you enter a new transaction that affects cost accounting, NetSuite sets the item's cost accounting status to **Pending** if the current status is **Complete** or **Blank**. If the item status is **Processing** or **Failed**, the status isn't reset.

To track the status of items that haven't completed cost calculation runs, see [Inventory Cost Accounting Workbook](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0420024853.html).

### Related Topics

-   [Setting Inventory Costing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497451045.html)
-   [Costing Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2191818.html)
-   [Selecting a Default Cost of Goods Sold (COGS) Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2192814.html)
-   [Inventory Costing and Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2194190.html)
-   [LIFO/FIFO Inventory Costing and Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2194541.html)
-   [System Cost of Goods Sold Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2195087.html)
-   [Viewing Inventory Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197076.html)
-   [Inventory Costing Recalculations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197365.html)
-   [Troubleshoot Inventory Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4447393386.html)
-   [Item Return Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199328.html)
-   [Group Average Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345703444.html)
-   [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html)
-   [Item Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2191369.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
