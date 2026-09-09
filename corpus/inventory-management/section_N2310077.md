---
id: "section_N2310077"
type: "section"
title: "Setting Transfer Order Preferences"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Transferring Inventory > Setting Transfer Order Preferences"
parent: "section_N2308202"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html"
anchors: ["procedure_N2310101"]
sha256: "4c45e4cae466bec6d2de30158c535be0635f9770239930e151dd74198e2daa3b"
---

You can set preferences that determine handling for transfer orders that you enter, including the default order status and approval requirements.

#### To set transfer order preferences: {#procedure_N2310101}

1.  Go to _Setup > Accounting > Accounting Preferences_.
    
2.  Click the **Order Management** subtab.
    
3.  To set a default on manual orders, in the Transfer Orders section, select a **Default Transfer Order Status**:
    
    -   **Pending Approval Firm** - Requires someone with sufficient permission to approve the order before it is processed. Firmed transfer orders are not available to be rescheduled or cancelled.
        
    -   **Pending Approval Open** - Requires someone with sufficient permission to approve the order before it is processed. Transfer orders that are Open, not Firmed, are available to be rescheduled or cancelled. Recommendations for Open transfer orders are removed for each demand planning run.
        
    -   **Pending Fulfillment** - To send transfer orders directly to the fulfillment queue without requiring further approval.
        
4.  To set a default on auto-generated transfer orders, in the **Generate Transfer Orders in Supply Planning** field, select one of the following:
    
    -   **Generate in Pending Approval Firm Status** - Requires someone with sufficient permission to approve the order before it is processed. Firmed transfer orders are not available to be rescheduled or cancelled.
        
    -   **Generate in Pending Approval Open Status** - Requires someone with sufficient permission to approve the order before it is processed. Transfer orders that are Open, not Firmed, are available to be rescheduled or cancelled. Recommendations for Open transfer orders are removed for each demand planning run.
        
    -   **Generate in Pending Fulfillment Status** - To send transfer orders directly to the fulfillment queue without requiring further approval.
        
    
    Note:
    
    The **Generate Transfer Orders in Supply Planning** field is only available in accounts that have Supply Planning features enabled. For more information, see [Enabling Supply Planning Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161780351051.html).
    
5.  To use the transfer price as a declared shipping value for reference only, check the **Use Item Cost as Transfer Cost** box.
    
    For example, for insurance or international shipping.
    
    Note:
    
    This preference can be applied to items that use the **Standard** costing method. When this preference is set, NetSuite uses the standard cost at the source location as the transfer cost for those items on the transfer order.
    
    -   The transfer price is not a charge for the destination location.
        
    -   The transfer price does not affect inventory costing on transactions.
        
    -   The transfer price defaults to show the value in the **Transfer Price** field of item records. This value can be changed on individual transfer orders.
        
    -   Partial fulfillment and receipt of transfer orders is allowed, but you cannot receive more than you have fulfilled as of any date. For example, if you have fulfilled 10 widgets out of 20 on a transfer order, you cannot receive 12 widgets on that order.
        
    
    To use the transfer price shown on the transfer order as the item cost on the item receipt, clear the **Use Item Cost as Transfer Cost** box.
    
    Important:
    
    If no transfer price is entered on the transfer order, no cost is recorded on the item receipt.
    
    -   Any difference between the actual cost and the transfer price posts to a Gain/Loss account when the item is shipped.
        
    -   The transfer price and the Gain/Loss account are defined on each item record.
        
    -   The transfer price defaults to show the value in the Transfer Price field of item records. This value can be changed on individual transfer orders.
        
        For example, for an order you are transferring, the transfer price and actual cost are as follows:
        
        Transfer Price $120
        
        Item Cost $100
        
        This table shows the posting amounts at the time of shipment:
        
        |  | DR | CR |
        | --- | --- | --- |
        | In-Transit | $120 (transfer price) |  |
        | Inventory Asset |  | $100 (item cost) |
        | Gain/Loss |  | $20 transfer price - item cost) |
        
        This table shows the posting amounts at the time of receipt:
        
        |  | DR | CR |
        | --- | --- | --- |
        | Inventory Asset | $120 (transfer price) |  |
        | In-Transit |  | $120 (item cost) |
        
    
    Note:
    
    This preference can also be set on individual transfer orders when they are created. Individual orders default to show the setting chosen in this field. The setting cannot be changed after the order is saved or after approval if you use approval routing.
    
6.  To set a default incoterm on transfer orders, select one of the following **Default Transfer Order Incoterms**:
    
    -   **Delivered at Place (DAP)** - Inventory ownership is transferred at the destination point.
        
    -   **Ex Work (EXW)** - Inventory ownership is transferred at the shipping point.
        
7.  To set a default time between the moment an order is shipped from one location and the moment it is received at a second location, enter a **Default Lead Time Between Locations**.
    
    For example, enter 31 to set a default lead time of 31 days.
    
8.  Click **Save**.
    

### Related Topics

-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html)
-   [Inventory Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308766.html)
-   [Entering a Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310933.html)
-   [Approving Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2311649.html)
-   [Fulfilling Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312176.html)
-   [Pick, Pack, and Ship with Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312623.html)
-   [Receiving Fulfilled Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312912.html)
-   [Intercompany Inventory Transfers - Non-Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html)
-   [Closing Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2316558.html)
-   [Inventory Replenishment and Withdrawal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317004.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
