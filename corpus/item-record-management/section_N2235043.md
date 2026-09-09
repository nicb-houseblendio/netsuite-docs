---
id: "section_N2235043"
type: "section"
title: "Adjusting Serialized Inventory"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Serial Numbered Items > Adjusting Serialized Inventory"
parent: "section_N2230290"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235043.html"
anchors: []
sha256: "33561b51c2cdc3a6d738d521f67d6b36e0e83eba25ca648743c3cfd346cd18ca"
---

Use the following procedure to adjust serialized inventory.

#### To adjust serialized inventory:

1.  Go to _Transactions > Inventory > Adjust Inventory_.
    
2.  To track the inventory variance, under **Primary Information**, select the **Adjustment Account**.
    
3.  If you use Multi-Location Inventory, select the **Location** where the item is located.
    
4.  In the **Adjust Quantity By** field, enter the amount to change the on hand quantity by. The number of serial numbers entered must equal the quantity of the adjustment.
    
    -   For a positive adjustment, enter new serial numbers to be added into inventory. You can also enter a new Unit Cost for the items. The cost applies only to the serial numbers listed in this adjustment line, it doesn't revalue the cost of existing serialized items.
        
    -   For a negative adjustment, enter the in-stock serial numbers you want to remove from inventory. You cannot enter a negative adjustment amount which is greater that the on hand quantity.
        
        If you use Multi-Location Inventory, the serial numbers must be in stock at the selected location.
        
    -   To **choose multiple serial numbered items** on transactions, click the **Select Multiple** link next to the **Serial/Lot Numbers** field. A popup window lists available serial numbers for the item. Click each item in the left pane to add it in the list right pane. When you click **Done**, all items in the right pane are added to the transaction.
        
5.  Click **Add** to save the adjustment line.
    
6.  Click **Save** when you're finished.
    

Serialized items are not available to adjust on the Adjust Inventory Worksheet. The worksheet defines an absolute quantity and value for a certain item on the date of the adjustment. There is no way to determine which serial numbers to add or remove if the item is adjusted. In addition, there is no way to determine the value of the items remaining on hand. For more information about adjusting serialized inventory using Multiple Units of Measure, see [Using Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html).

### Related Topics

-   [Enabling Serial Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230646.html)
-   [Entering Serialized Inventory Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230957.html)
-   [Track Serialized Inventory on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2231339.html)
-   [Add New Serial Numbers to Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2231739.html)
-   [Searching for Serialized Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1508171622.html)
-   [Receiving a Purchase Order With a Serialized Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233116.html)
-   [Serialized Items on Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233510.html)
-   [Fulfilling a Sales Order with a Serialized Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233933.html)
-   [Memorizing Transactions with Serialized Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2234305.html)
-   [Building a Serialized Assembly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2234538.html)
-   [Removing Serial Numbers on Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235383.html)
-   [Serial Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230290.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
