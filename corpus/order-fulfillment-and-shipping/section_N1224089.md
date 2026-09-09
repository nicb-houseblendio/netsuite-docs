---
id: "section_N1224089"
type: "section"
title: "Advanced Shipping"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Advanced Shipping"
parent: "chapter_N1222915"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1224089.html"
anchors: ["procedure_N1224129"]
sha256: "433c363e4c84bd83cf920644d4aebfdbba6399eccd1ed59faee02d71f62a240e"
---

Advanced shipping lets your shipping and accounting departments work separately on fulfilling and billing orders. Your shipping department fulfills part or all of an order when it's ready to ship. Then, your accounting department creates an invoice or cash sale for the shipped items and rendered services.

Advanced Shipping lets you track partial shipments and invoice customers for partial or full orders. Your picking tickets show the items on the order that are shipped.

If you want to create invoices for a whole order before it's fully fulfilled, enable the **Invoice in Advance of Fulfillment** preference. You can create an invoice or cash sale for the entire order, even if you've only shipped part of it. For information about enabling this preference, read [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1384948.html).

Note:

If an item is manually added to an invoice, the on-hand quantity displayed for the item on the invoice and on any linked fulfillments shows the corresponding reduction.

You can also optionally use the Advanced Billing feature with the Advanced Shipping feature. For more information, read [Fulfilling Orders Using Advanced Shipping with Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1226246.html).

You can choose to fulfill a single order or multiple orders.

Note:

You cannot include a partially processed order when fulfilling multiple orders. Partially processed orders must be fulfilled individually.

#### To enable Advanced Shipping: {#procedure_N1224129}

1.  Go to _Setup > Company > Enable Features_.
    
2.  Click the **Transactions** subtab.
    
3.  Check the **Advanced Shipping** box.
    
4.  Click **Save**.
    

After you have enabled Advanced Shipping, certain roles may need to be customized to allow them to fulfill orders. Administrators should ensure that the required role has the following permissions:

-   Item Fulfillment - this permission adds the fulfill button on sales orders.
    
-   Fulfill Orders - this permission adds the menu option to the bulk Fulfill Orders page.
    

#### To add Fulfillment permissions to a role:

1.  Go to _Setup > Users/Roles > Manage Roles_.
    
2.  Click **Customize** on the role you want to add the fulfill permission to.
    
3.  On the **Permissions** subtab under Transactions, select **Item Fulfillment**.
    
4.  In the **Level** column, select **Full** and click **OK**.
    
5.  Repeat the above steps for the permission **Fulfil Orders**.
    
6.  Click **Save**.
    

Once the role has been customized to include the fulfillment permission, the role should then be assigned to the user. For more information on customizing roles see [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html).

Note:

After you have enabled Advanced Shipping, it cannot be turned off unless all fulfilled sales orders are billed.

### Related Topics:

-   [Fulfill a Single Order Using Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1224254.html)
-   [Fulfill Multiple Orders Using Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1225980.html)
-   [Fulfilling Orders Using Advanced Shipping with Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1226246.html)
-   [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
