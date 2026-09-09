---
id: "section_N1306234"
type: "section"
title: "Entering a Linked Return Authorization"
branch: "customer-returns"
category: "order-management"
breadcrumb: "Order Management > Customer Returns > Customer Return Management > Entering a Linked Return Authorization"
parent: "section_N1302852"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1306234.html"
anchors: ["procedure_N1306284"]
sha256: "8177b3e8636565d361ac0106b49aa48d3ba248fe646b04355140f98a52e7d4a4"
---

A return authorization form is a record of expected customer returns holds information about the items you expect to receive. For more information, read [Return Authorization (RMA) Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1304530.html).

A linked return authorization is created from a sales order, cash sale or invoice. It automatically shows the items from the original sale and is linked to the original sale.

This means that information is sourced from an existing transaction to create the authorization, such as item prices or quantities, so information doesn't need to be entered in the authorization manually.

For information about standalone return authorizations that are not linked to previous sales, read [Entering a Standalone Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1305354.html).

#### To enter a linked return authorization: {#procedure_N1306284}

1.  Do one of the following:
    
    -   View the cash sales list: _Transactions > Sales > Enter Cash Sales > List (Administrator)_
        
    -   View the invoices list: _Transactions > Sales > Create Invoices > List (Administrator)_
        
    -   View the sales order list: _Transactions > Sales > Enter Sales Orders > List (Administrator)_
        
2.  Click **View** next to a cash sale or invoice.
    
3.  Click the **Authorize Return** button.
    
    A customer return authorization opens that shows all items from the original order.
    
    You will receive a popup warning if there are existing return authorizations associated with this order.
    
    You can change the sales effective date for this transaction. The sales effective date determines which commission plan and historical sales team this transaction applies to.
    
4.  Check the **Exclude Commissions** box to exclude this transaction and its subordinate transactions from inclusion in all commission calculations. For example, selecting this box on a sales order excludes the sales order and the resulting invoice from all commission calculations for all sales people.
    
5.  Click the **Items** subtab and verify that all items on the return authorization are being returned.
    
    Important:
    
    If some items are not being returned, remove them by clicking the line-item and then clicking **Remove**.
    
    For more information, see [Adding Items on a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588373194.html).
    
6.  On the **Billing** subtab, the customer's default billing address autofills the **Bill To** text field. You can change this address as needed.
    
    For more information, see [Adding Billing Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588267772.html).
    
7.  On the **Payment** subtab, select the customer's original payment method. For more information, see [Entering Payment Information on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586835857.html).
    
    If you want to credit your customer's credit card account and don't have an MeS merchant account, check the **Card Approved** box after the refund is approved.
    
    If you do have an MeS merchant account, the **Card Approved** box is automatically filled when the refund is approved.
    
    If you don't use NetSuite to process credit cards, enter any authorization information for this credit card.
    
8.  The Accounting subtab only shows if you are using the Multiple Currencies or Revenue Recognition features, if you have not enabled the Per-Line Taxes preference at _Setup > Accounting > Taxes > Set Up Taxes (Administrator)_, or if you have added fields to this subtab. For more information, see [Entering Accounting information about a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4587464246.html).
    
9.  On the **Relationships** subtab, enter a contact or partner details for this transaction. For more information, see [Entering Relationships on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586861907.html).
    
10.  On the **Sales Team** subtab, if you use the Team Selling feature, select the Sales Team for this transaction. For more information, see [Associating Sales Teams with Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038639.html).
     
11.  On the **Communication** subtab, enter communication information for this transaction. For more information, see [Entering Communication Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586862223.html).
     
12.  Click **Save**.
     

The customer return authorization is recorded in the Return Authorizations Register, a non-posting account in your chart of accounts.

Now, you can track the return of these items into your inventory.

### Related Topics:

-   [Customer Return Management Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1303478.html)
-   [Customer Returns Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1303799.html)
-   [Return Authorization (RMA) Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1304530.html)
-   [Preferences for Customer Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1305008.html)
-   [Entering a Standalone Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1305354.html)
-   [Approving a Customer Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1306797.html)
-   [Printing a Customer Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1307142.html)
-   [Receiving a Customer Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1307628.html)
-   [Handling Returned Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1308274.html)
-   [Closing Line Items on a Customer Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1309679.html)
-   [Customer Return Authorization Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1310133.html)
-   [Reporting on Customer Returns Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1310580.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
