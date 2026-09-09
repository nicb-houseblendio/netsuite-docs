---
id: "section_N1227269"
type: "section"
title: "Printing a Picking Ticket"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Printing a Picking Ticket"
parent: "chapter_N1222915"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1227269.html"
anchors: ["procedure_N1227304"]
sha256: "7cfd09fed591616841282119d4f116fecefb082ac828269e1b8f655304c5042a"
---

You can print a picking ticket for an order to indicate the items to pull from inventory to fulfill an order.

When printing a picking ticket, items on the order that have already been shipped are not displayed. In this case, the picking ticket is blank because there are no items to pick.

Note:

If Bin Management, Units of Measure, and Advanced Bin/Numbered Inventory Management are enabled, bin quantities on hand display in the base unit of measure.

You need Adobe Reader to print PDF forms. Visit the [Adobe Web site](http://www.adobe.com/products/acrobat.html) to download the latest version at no charge. Next, in NetSuite, go to _Home > Set Preferences_. On the Transactions subtab, clear the Print Using HTML box under Printing and click Save.

#### To print a picking ticket: {#procedure_N1227304}

1.  Go to _Transactions > Management > Print Checks and Forms_.
    
2.  On the Print Checks and Forms page, click **Picking Tickets**.
    
3.  On the Print Picking Tickets page, you can filter the list in the **Filter By** field to show only orders with All Items Fully Committed or orders with at least Some Items Committed.
    
    If you choose to Ignore Item Availability, all open orders show in the list.
    
4.  If you use locations, select a location to print picking tickets for.
    
5.  If you use the Multiple Shipping Routes feature, a picking ticket is generated for each shipping route. The Print Picking Tickets queue shows a separate line for each shipping route on the same order.
    
    For more information, see [Item Fulfillments and Multiple Shipping Routes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263863.html).
    
6.  Check the **Allow Reprinting** box to be able to reprint previously printed transactions.
    
    When you check this box, all documents appear at the bottom of the page in segments.
    
7.  Click **Customize** to include additional information on the page.
    
    This additional information is not added to the printed picking ticket.
    
8.  In the **Print** column, check the box next to the orders you want to print picking tickets for, or click **Mark All** to print picking tickets for all orders on the page.
    
9.  Click the **Print** button.
    
    Note:
    
    If you use the Multi-Language feature and have customers that use a different language than the one you set at _Home > Set Preferences_, when you point to the Print icon, you can select **Print in Customer's Locale** to translate the transaction into the customer's predefined language. For more information, see [Configuring Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N247147.html).
    
10.  If you are using Adobe Acrobat, click the printer button in the Adobe application frame.
     
     A Print window opens.
     
11.  Specify the printing details.
     
     For example, if you want to print multiple copies of each picking ticket, specify the number.
     
12.  Click **OK**.
     

Now, you can use picking tickets to pull the items you need to ship. The layout and details printed on a picking ticket depend on the selected picking ticket form. You can create custom picking tickets to include additional fields or specify item sorting.

You can also print a picking ticket when viewing an order.

-   To view a sales order, go to _Transactions > Sales > Enter Sales Orders > List_ and click View next to a sales order. Point to the print icon in the transaction header and select Print Picking Ticket.
    
-   To view a transfer order, go to _Transactions > Inventory > Enter Transfer Orders > List_.
    

NetSuite forms can be purchased from the [NEBS Web site](http://www.netsuiteforms.com). You can print picking tickets on blank paper as well.

### Related Topics:

-   [Sorting Items on Picking Tickets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1227589.html)
-   [Kit Items on Picking Tickets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1227764.html)
-   [Bin Numbers on Picking Tickets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1229129.html)
-   [Multiple Shipping Routes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263041.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
