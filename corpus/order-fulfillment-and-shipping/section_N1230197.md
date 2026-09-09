---
id: "section_N1230197"
type: "section"
title: "Setting Up Pick, Pack, and Ship"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Pick, Pack, and Ship > Setting Up Pick, Pack, and Ship"
parent: "section_N1229691"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230197.html"
anchors: ["procedure_N1230209", "procedure_N1230278"]
sha256: "67e50168327c87c4a0808e21af48229870cc5a6b0854942c5058544437000ce9"
---

To use Pick, Pack and Ship, you must enable the feature and set preferences.

#### To enable the feature: {#procedure_N1230209}

1.  Go to _Setup > Company > Enable Features_.
    
2.  On the **Transactions** subtab, check these boxes:
    
    -   **Pick, Pack and Ship**
        
    -   **Advanced Shipping**
        
3.  Click **Save**.
    

#### To set preferences: {#procedure_N1230278}

1.  Go to _Setup > Accounting > Setup Tasks > Shipping_.
    
2.  In the **Default Item Fulfillment Integration Stage** field, select the Picked, Packed, or Shipped stage you want to use as the default fulfillment status in your sales order process. When you fulfill an order, this is the status of the sales order on the Item Fulfillment page. You can always select a different stage when fulfilling an order.
    
3.  If you use the Shipping Label Integration feature, in the **Shipping Label Creation Stage** field, select the earliest stage when you can get tracking numbers and print shipping labels. This does not have to be the same as the Default Item Fulfillment Stage.
    
    For example, you generally want to mark sales orders as Shipped when you fulfill them. For part of your inventory, you know you will change the order fulfillment status to Picked, and need to be able to get tracking numbers and print shipping labels at that stage. You can do so if you set the Shipping Label Creation stage to Picked.
    
    -   Select **Picked** to receive a tracking number and print a bar-coded shipping label when the fulfillment status of an order is at least picked.
        
    -   Select **Packed** to receive a tracking number and print a shipping label when orders are marked packed.
        
    -   Select **Shipped** to have the tracking number and shipping label made available only when the order is marked shipped.
        
4.  Click **Submit**.
    

### Related Topics:

-   [Commitment Settings for Reallocation of Picked or Packed Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0525105436.html)
-   [Order Management Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1388149.html)
-   [Pick, Pack, and Ship Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230081.html)
-   [Fulfilling Orders Using Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230473.html)
-   [Marking an Order Packed](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230849.html)
-   [Marking an Order Shipped](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231176.html)
-   [Pick, Pack, and Ship Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230081.html)
-   [Order Fulfillment Confirmation Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231778.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
