---
id: "section_N2300611"
type: "section"
title: "Enabling Available to Promise"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Advanced Inventory Management > Available to Promise > Enabling Available to Promise"
parent: "section_N2300269"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2300611.html"
anchors: []
sha256: "4c89fa72c7d0c91ad3dab10c72406e65068265d2bf3520aa0d92bc00992e48db"
---

Enable the Available to Promise feature to check inventory and assembly item availability.

Note:

To use this feature, enable Demand Planning.

#### To enable the Available to Promise feature:

1.  Go to _Setup > Company > Enable Features_.
    
2.  On the **Items & Inventory** subtab, check the **Available to Promise** box.
    
3.  Click **Save**.
    

After the feature is enabled, you can set up item records for it.

#### To set up an item record for Available to Promise:

1.  Go to _Lists > Accounting > Items_.
    
2.  Beside the name of an inventory or assembly item, click **Edit**.
    
3.  On the item record, click the **Purchasing/Inventory** subtab.
    
4.  In the **Inventory Management** section, select a **Default ATP Method**.
    
    For more information, see [Available to Promise Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2301636.html).
    
5.  In the **ATP Lead Time** field, enter a lead time to use in Available to Promise calculations.
    
    ATP lead time is used as a planning horizon for supply and demand in the ship date recommendation calculations. ATP lead time also provides a ship date on an order when no inventory is available based on future supply and demand.
    
    If you use the Multi-Location Inventory feature, the **Locations** subtab shows an **ATP Lead Time** column. You can enter a distinct ATP lead time for each location in the fields in this column.
    
6.  Enter additional data in fields as necessary.
    
7.  Click **Save**.
    

### Related Topics

-   [Available to Promise Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2301636.html)
-   [Checking Item Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2302738.html)
-   [Available to Promise Earliest Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159250317916.html)
-   [Available to Promise](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2300269.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
