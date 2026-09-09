---
id: "section_N2274082"
type: "section"
title: "Creating Bin Records"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Bin Management > Creating Bin Records"
parent: "section_N2270284"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274082.html"
anchors: ["procedure_N2274151"]
sha256: "1a70e28650ecad176418443308315f44728e7ec82a829cdb496bb54effe001cf"
---

You can use bin records to define bin locations within a warehouse or stock room. Bin record numbers are associated with items and included on receiving and fulfilling transactions to keep track of inventory for each bin.

Note the following guidelines when creating bin records:

-   There is no limit on the number of bin records you can create.
    
-   If you use the basic Bin Management feature with the Multi-Location Inventory feature, you must use bins in all locations. If you use the Advanced Bin / Numbered Inventory Management feature with the Multi-Location Inventory feature, you can use bins on a per-location basis.
    
-   Item costing is not calculated per bin, and only on-hand and available quantities are tracked per bin. Committed, backordered, and ordered quantities are not tracked per bin.
    

#### To create bin records: {#procedure_N2274151}

1.  Go to Lists > Supply Chain > Bins > New.
    
2.  In the **Bin Number** field, enter a number or code to designate a bin location in your warehouse or stock room.
    
    For example, you can name rows and shelves in your warehouse by letter and bins by number. The first bin in the first shelf on the first row would be **AA01**.
    
3.  If you use the Multi-Location Inventory feature, select the location for this bin.
    
    You cannot change the location after you save the bin record.
    
4.  In the **Memo** field, include further notes on the bin's location or notes on what should be stored in the bin.
    
5.  Check the **Inactive** box to inactivate this bin record.
    
6.  Click **Save**.
    

After you create bin records, you can set up item records for use with bins. Read [Setting Up Item Records for Bins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274433.html).

### Related Topics

-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
-   [Basic Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271509.html)
-   [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html)
-   [Enabling Bin Management Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273046.html)
-   [Setting Bin Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273755.html)
-   [Setting Up Item Records for Bins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274433.html)
-   [Bin Transfers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2278346.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
