---
id: "section_N1263649"
type: "section"
title: "Setting a Default Shipping Method Per Item"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > Multiple Shipping Routes > Setting a Default Shipping Method Per Item"
parent: "section_N1263041"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263649.html"
anchors: ["procedure_N1263697"]
sha256: "909433c59952b80be109c8b78e48e8bdf1ee7cd977d484e8b0f9e14add414a90"
---

NetSuite enables you to specify a default shipping method to use when adding an item to a sales order. The default shipping method displays automatically when your sales team selects a shipping method when adding an item to an order.

You can set default shipping methods for Assembly items, Inventory items, Item Groups, and Kits/Packages.

Instead of relying on automatic shipping calculators to pick the best method, the default shipping option enables you to better control shipping costs for orders that typically have items with different size or weight ratios, or require special transportation.

For example, you ship items that vary in weight, such as a sofa and a pillow cover, from a single order. If you specify a default shipping method for each item, then when your sales team adds these items to an order, the default shipping method for each item displays automatically.

This feature restricts shipping items during order entry only. To override the default shipping method:

-   **On the sales order**, select any approved shipping method specified in the **Shipping Methods** field on the Item record.
    
-   **On the order fulfillment**, select any shipping method.
    

Note:

Multiple Shipping Routes must be enabled to specify default shipping methods.

#### To specify a default shipping method for an item: {#procedure_N1263697}

1.  Go to _Lists > Accounting > Items._.
    
2.  Beside the item you want to specify a shipping method for, click **Edit**.
    
3.  Click the **Purchasing/Inventory** subtab.
    
4.  In the **Vendor Bill Matching** section, complete the following:
    
    1.  Select a **Carrier**.
        
    2.  Select a **Shipping Methods**.
        
    3.  Select a **Default Shipping Method** to display when adding an item to a sales order.
        
5.  Click **Save**.
    

#### To specify a carrier and shipping method on the customer record:

1.  Go to _Setup > Accounting > Shipping > Set Up Shipping_.
    
2.  When you create a sales order, the carrier and shipping method for a line item display based on this order:
    
    -   From the Default Shipping Method on the Item record.
        
    -   If the item does not have a default shipping method, then the Shipping Carrier and Shipping Method specified on the Customer record display.
        
    -   If the customer does not have preferred shipping information, then the Default Shipping Carrier and Default Shipping Method from your Shipping setup display.
        

### Related Items

-   [Item Fulfillments and Multiple Shipping Routes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263863.html)
-   [Entering Purchasing and Inventory Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2167714.html)
-   [Order Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1222915.html)
-   [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html)
-   [Multiple Ship To](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4188560821.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
