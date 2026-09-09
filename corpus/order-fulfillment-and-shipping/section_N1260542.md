---
id: "section_N1260542"
type: "section"
title: "Charging for Shipping and Handling per Item"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > Setting Up Shipping > Charging for Shipping and Handling per Item"
parent: "section_N1257579"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1260542.html"
anchors: ["procedure_N1260613"]
sha256: "40d2b7497fc2012ceeff0247d062c5fcb926815a836a57f5229499a17476035b"
---

You can charge for shipping and handling on a per item basis instead of by total order weight. This makes it easier to charge the appropriate amount for shipping or handling costs. When a customer places an order, NetSuite automatically calculates the shipping and handling charges based on the items purchased.

For example, you can enter shipping and handling costs on each item record. When you invoice those items, the shipping and handling cost on the transaction reflects what you entered on the item record.

#### To automatically charge for shipping:

1.  Go to _Setup > Accounting > Shipping_.
    
2.  Check the **Charge for Shipping** box.
    
3.  Click **Save**.
    

#### To charge for handling:

1.  Check the **Charge for Shipping** box.
    
    You must charge for shipping to be able to charge for handling.
    
2.  Check the **Charge Handling Separate from Shipping box**.
    
3.  Click **Save**.
    

#### To charge per-item shipping or handling costs: {#procedure_N1260613}

1.  Go to _Lists > Accounting > Items._.
    
2.  Beside the item you want to enter a shipping or handling cost for, click **Edit**.
    
3.  On the item record, click the **Sales/Pricing** subtab.
    
4.  In the **Shipping** section, enter a price in the **Shipping Cost** field.
    
5.  Enter the item's handling price in the **Handling Cost** field.
    
6.  Click **Save**.
    
    Repeat these steps for every item you want to charge a specific shipping or handling cost for.
    
7.  To charge per item shipping, create a per item shipping item record to use as the shipping method on transactions and in the web store.
    
    Follow the [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html) procedure and then, on the **Shipping Rate** subtab, select the **By Item** option button.
    
8.  If a shipping cost is not entered on the item record, enter the **Default Charge** amount to display on the transaction or in the web store.
    

To charge the shipping amount entered on item records, select a per item shipping method on transactions and in the web store.

You can display a per item shipping method on your web store as well as other types of shipping methods. However, if the web store shopper selects a shipping method other than the per item shipping method, the shipping cost entered on the item record is overridden.

When you charge for shipping and handling, the full amount is charged on the bill for the first item fulfillment. Subsequent order fulfillments charge shipping or handling.

For example, a customer's order for two bicycle wheels has a $15 charge for shipping. The first fulfillment ships one wheel, and the bill shows a $15 charge for shipping. Fulfillment number two ships the other wheel, and the bill shows no charge for shipping.

If Multiple Shipping Routes is enabled, any shipping or handling rule which has been applied to the transaction will be calculated on a shipment-level basis instead.

For example, when calculating the Free if Total is over rule, the total value of items in that shipment is used to determine whether the discount criteria is met, not the value of the combined transactions on the sales order.

#### To display charges on transactions:

1.  On the transactions you print as line items or as a total amount on the transaction, go to _Setup > Company > Printing & Fax_.
    
2.  Click the **Printing** subtab.
    
3.  To show discount and shipping items with descriptions as line items in transaction columns, check the **Print Discount and Shipping Lines in Columns** box.
    
    If you clear this box, the footer of the transaction shows only a shipping item name and the total shipping and handling cost.
    
4.  Click **Save**.
    

### Related Topics

-   [Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1258840.html)
-   [Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1258840.html)
-   [Free Shipping With an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262298.html)
-   [Shipping Basics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262219.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
