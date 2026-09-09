---
id: "section_N1227589"
type: "section"
title: "Sorting Items on Picking Tickets"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Printing a Picking Ticket > Sorting Items on Picking Tickets"
parent: "section_N1227269"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1227589.html"
anchors: []
sha256: "42ee1e312d44c824ce63c9d428906f3c14e8c67fa6b83221870a8fd95ae50a82"
---

You can sort items on printed picking tickets to optimize picking operations at your warehouse. Choose a sort order for picking tickets based on picking ticket fields, including custom fields you have created. Standard picking ticket fields include Item, Description, and Ordered. If your warehouse is organized by sections and shelves, you might create custom fields called Shelf and Section. You can sort by one field and then by another field.

To sort items on your picking tickets, you must customize a picking ticket form to determine the sorting order.

#### To customize a picking ticket:

1.  Go to _Customization > Forms > Transaction Forms_. Click Customize next to Standard Picking Ticket. The Custom Transaction Form page is displayed.
    
2.  For printing type, choose **Basic**.
    
    Note:
    
    If you use advanced PDF/HTML templates to format picking tickets, you can sort line items with the `sort_by()` function. See [Syntax for Advanced Template Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2864199.html) for more information.
    
3.  On the Printing Fields tab, click the **Columns** subtab.
    
4.  At the top of the Columns subtab, two sorting fields have dropdown lists that include all column fields that can be displayed on the picking ticket, including custom column fields.
    
    1.  In the **Sort Line Items By** field, choose a field to sort the picking tickets.
        
    2.  In the **Then By** field, choose a field for a secondary sort for picking tickets.
        
    
    For example, if you use the Bin Management feature and also customized your item records with a Widget Number field, you can sort your picking tickets in this manner:
    
    In the Sort Line Items By field, choose Bin Numbers.
    
    In the Then By field, choose your custom Widget Number field.
    
    Using this custom picking ticket, items on picking tickets are first grouped by bin numbers. Also, within each bin number group, items are secondarily grouped by widget number.
    
5.  The sort order on custom forms is ascending by default, but you can check the **Descending** box to change the sort order.
    
6.  Click **Save**.
    

### Related Topics:

-   [Printing a Picking Ticket](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1227269.html)
-   [Kit Items on Picking Tickets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1227764.html)
-   [Bin Numbers on Picking Tickets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1229129.html)
-   [Creating Custom Transaction Line Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828307.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
