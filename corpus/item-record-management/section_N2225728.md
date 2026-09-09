---
id: "section_N2225728"
type: "section"
title: "Updating Kits with Bins"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Kit/Package Items > Updating Kits with Bins"
parent: "section_N2225190"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225728.html"
anchors: ["procedure_N2225754"]
sha256: "ba96c1859e9c41726dc2e71f7571582d5e9a4fbfd0614496b5d74c536b1276d0"
---

If you use a bin management feature, before order fulfillment, you might need to update kit items if they include members that use bins. If the kit member changes between the time the order is entered and when it is fulfilled, the bin discrepancy could cause errors. A mass update can be run to update the kits that have changed.

For example, you might have a kit item named WidgetKit. WidgetKit includes a member called BinMember1 which uses bins. You enter sales order #1001 and add one WidgetKit to the order. The status of the order is then Pending Fulfillment.

Then, you edit the item record for WidgetKit to remove BinMember1 to add BinMember2. Later, you try to fulfill sales order #1001, but an error prevents you. You need to run the mass update to correct the bin discrepancy.

Note:

Mass update is available only if the Bin Management or Advanced Bin/Numbered Inventory Management feature is enabled.

#### To run a kit member mass update: {#procedure_N2225754}

1.  Go to _Lists > Mass Update > Mass Updates_.
    
2.  Click **Special Transaction Updates**.
    
3.  Click **Update Orders Kit Members with Current Kit Members**.
    
4.  On the **Criteria** subtab in the **Filter** field, select **Item On Any Line**.
    
5.  In the popup window, select one or more items to update.
    
    (From the previous example, you would select WidgetKit.)
    
6.  Click **Set**.
    
7.  Click **Preview**.
    
8.  In the preview, verify that the order needing updating is included.
    
    (From the previous example, verify order #1001.)
    
    the update applies only to sales orders with a status of Pending Fulfillment.
    
9.  Click **Perform Update**.
    

After the Mass Update completes, you can fulfill the order. Any non-bin members of items will also get updated as required.

### Related Topics

-   [Entering Serial and Lot Components on the Item Record for the Kit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225398.html)
-   [Kit/Package Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225190.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
