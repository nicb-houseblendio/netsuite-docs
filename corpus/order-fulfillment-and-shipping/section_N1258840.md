---
id: "section_N1258840"
type: "section"
title: "Shipping Items"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > Setting Up Shipping > Shipping Items"
parent: "section_N1257579"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1258840.html"
anchors: ["bridgehead_N1258952"]
sha256: "03913f8590860b214bbf79d2a98da733e207f8b6fb9bd1f5556cf9af57e74cc9"
---

Shipping item records outline how an item is shipped. This includes shipping rate information, handling rates, rules for shipping and handling, and when shipping is free. NetSuite also refers to a Shipping Item as Shipping Method and Ship Via.

Shipping item records enable you to do the following:

-   Enter a handling charge
    
-   Set the shipping charge method
    
    For example, by weight or flat rate
    
-   Define the country or countries where the shipping item can be used
    
-   Specify the shipping item website
    
-   Enter a name to display in your web store printed forms, and in centers such as the Customer Center
    
-   Set conditions for offering free shipping
    
    To learn more, see [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html).
    

## Automatically Charging for Shipping {#bridgehead_N1258952}

NetSuite enables you to automatically charge for shipping on each order or to enter shipping as a line-item for individual sales orders, cash sales, and invoices.

#### To enable the Charge for Shipping preference :

1.  Go to _Setup > Accounting > Setup Tasks > Shipping_.
    
2.  Check the **Charge for Shipping** box.
    
3.  Click **Save**.
    

**If you automatically charge for shipping**:

-   For each shipping item you create, you can select a different method to charge shipping.
    
    For example, your West Coast store charges shipping by item weight. The East Coast store charges shipping based on the cost of the total order. The Corporate store includes the cost of shipping in item sales prices and uses shipping methods only as descriptive line items on transaction forms.
    
-   Shipping charges allocate income to a separate account.
    
-   Shipping charges are displayed on your website and on transactions based on the selected shipping item.
    
-   If you charge for shipping you can charge a separate handling fee.
    
    Charging a separate handling fee enables you to allocate income from fees charged for the labor and supplies for handling to a separate account.
    
-   You cannot add shipping items to your transactions as line items.
    
    The shipping amount automatically appears based on the shipping item selected in the Ship Via or Shipping Method field.
    
-   Shipping and handling still appear as one total to your customers on your website.
    

#### To charge a separate handling fee:

1.  Go to _Setup > Accounting > Setup Tasks > Shipping_.
    
2.  Check the **Charge Handling Separate from Shipping** box.
    
3.  Click **Save**.
    

**If you do not automatically charge for shipping**:

-   If you do not automatically charge for shipping but want to include shipping items as transaction line items, you can enter a basic shipping item record.
    
    You can then charge for shipping on individual sales orders and invoices. You must specify an amount for each shipping item you add to the transaction.
    
-   A choice or charge for shipping does not show in your website.
    

### Related Topics

-   [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html)
-   [Charging for Shipping and Handling per Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1260542.html)
-   [Creating Shipping Items with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268691.html)
-   [Creating Shipping Items with UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278291.html)
-   [USPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283711.html)
-   [Shipping Basics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262219.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
