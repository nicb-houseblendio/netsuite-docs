---
id: "section_N2311649"
type: "section"
title: "Approving Transfer Orders"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Transferring Inventory > Approving Transfer Orders"
parent: "section_N2308202"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2311649.html"
anchors: ["procedure_N2311844", "bridgehead_N2311957"]
sha256: "755eecd758f0486b8ed30adf01e8752e5e3b79fe1d64898269af2f16be9ed7b2"
---

After you enter transfer orders, if an order has a status of Pending Approval, the order must be approved by someone with authorization before it can be processed.

You can choose to require approval by default. For details about approval preferences, read [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html).

#### To approve transfer orders: {#procedure_N2311844}

1.  Go to _Transactions > Inventory > Approve Transfer Orders_.
    
2.  In the **Supervisor** field, select a name to filter the sales order list by supervisor.
    
    Clear this field to show all transfer orders pending approval.
    
3.  To approve a specific order, enter an order number in the **Select Order** number field, either manually or by scanning a bar code.
    
4.  In the **Date** field, select the date range for the transactions you want to show in the list. The date range you select is reflected in the **From** and **To** fields. If you enter a different range in the **From** and **To** fields, the **Date** field automatically shows **Custom**.
    
5.  Check the box in the **Approve** column for each transfer order you want to approve.
    
6.  The **Amount** field displays the total amount of orders you have checked for approval.
    
7.  If a source location has not yet been selected, choose a source location.
    
8.  Click **Submit**.
    

After a transfer order is approved, the items are committed to the transfer and cannot be sold when in transit. Approved transfer items also show as on order at the destination location.

You can now fulfill your transfer orders. To do this, go to _Transactions > Sales > Fulfill Orders._.

## Resetting Approval Status {#bridgehead_N2311957}

The status of an order that is approved and pending fulfillment can be reset to Pending Approval. If you have permission to approve and edit transfer orders, the Status field appears when you edit a transfer order that has not been fulfilled.

To reset the status, select Pending Approval in the Status field, then click Save. To edit an existing transfer order, go to _Transactions >Inventory > Enter Transfer Orders > List._. Click Edit next to the order.

### Related Topics

-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html)
-   [Inventory Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308766.html)
-   [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html)
-   [Entering a Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310933.html)
-   [Fulfilling Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312176.html)
-   [Pick, Pack, and Ship with Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312623.html)
-   [Receiving Fulfilled Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312912.html)
-   [Intercompany Inventory Transfers - Non-Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html)
-   [Closing Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2316558.html)
-   [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
