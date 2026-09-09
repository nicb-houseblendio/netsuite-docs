---
id: "section_N1218788"
type: "section"
title: "Approving Sales Orders"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Sales Orders > Approving Sales Orders"
parent: "chapter_N1215966"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1218788.html"
anchors: ["subsect_1124013244", "subsect_1124013144"]
sha256: "f17abcb0fbbcfc45057253ff0ea4f0cbdad88015e340d5371ed87035cc705319"
---

If a sales order is Pending Approval, it needs to be approved by someone with the right permissions before NetSuite can process it.

If you have a Web store or use online ordering, you can easily approve sale orders that arrive through your website.

#### To approve a sales order:

1.  Go to _Opportunities > Transactions > Approve Sales Orders_.
    
    You'll see a list of orders at the bottom of the page.
    
2.  In the **Supervisor** field, select a name to filter the sales order list by supervisor.
    
    Clear this field to see all sales orders pending approval.
    
3.  Check the box in the **Approve** column for each sales order you want to approve.
    
4.  In the **Date** field, select the date range for the transactions you want to show in the list. The date range you select is shown in the From and To fields. If you enter a different range, the Date field shows Custom.
    
5.  To approve a specific order, enter an order number in the **Select Order** number field, or scan the bar code.
    
    The Security Match column checks the credit card for:
    
    -   Address Verification Service (AVS) street address match
        
    -   Address Verification Service (AVS) postal zip code match
        
    -   3- or 4-digit Card Security Code match
        
    
    The **Amount** field shows the total amount of orders you've checked for approval.
    
6.  Click **Submit**.
    

Now you can process your sales orders and turn them into cash sales or invoices. To do this, go to _Transactions > Sales > Fulfill Orders (Administrator)_.

## Resetting Approval Status {#subsect_1124013244}

You can reset the status of an order that is approved and pending fulfillment to Pending Approval. If you have permission to approve and edit sales orders, the Status field appears when you edit an unfulfilled sales order. When a sales order is partially fulfilled, the status can't be changed back to Pending Approval. For more information about setting permissions, see [Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2394992.html).

#### To reset approval status:

1.  In the **Status** field, select **Pending Approval**.
    
2.  Click **Save**.
    

To edit an existing sales order, go to _Opportunities > Transactions > Sales Orders_ and click **Edit** next to the order.

## Requiring Re-approval {#subsect_1124013144}

You can also require re-approval when someone edits a sales order that was previously approved. However, partially fulfilled sales orders are not affected by this preference. When a sales order is partially fulfilled, the status can't be changed back to pending approval.

#### To require re-approval of an edited sales order:

1.  Go to _Setup > Accounting > Preferences > Accounting Preferences (Administrator)_.
    
2.  On the **Order Management** subtab, check the **Require Re-approval on Edit of Sales Order** box and click **Save**.
    

### Related Topics

-   [Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1215966.html)
-   [Sales Order Entry Workflow Chart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216314.html)
-   [Creating Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216500.html)
-   [The Standard Sales Order Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1218600.html)
-   [Closing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698204292.html)
-   [Reopening a Closed Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161133765436.html)
-   [Invoicing Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1219162.html)
-   [Viewing the Status of Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1220604.html)
-   [Printing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221008.html)
-   [Creating Invoices or Cash Sales from Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221414.html)
-   [Creating Progress Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221802.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
