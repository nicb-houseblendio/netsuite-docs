---
id: "section_N1311510"
type: "section"
title: "Issuing a Customer Credit Memo"
branch: "customer-returns"
category: "order-management"
breadcrumb: "Order Management > Customer Returns > Customer Credits and Refunds > Customer Credits > Issuing a Customer Credit Memo"
parent: "section_4417991103"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1311510.html"
anchors: ["procedure_N1311558"]
sha256: "2dfe459f97c377f2e338521ae94b23a940270a42e25c5611a966268fde79c5a0"
---

A credit memo is a transaction that decreases the amount a customer owes you. A credit memo created from a return authorization has no impact on inventory; however, a stand-alone credit memo does impact inventory.

Note:

You can use the Import Assistant to import credit memo data from a CSV file. See [Credit Memo Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N408112.html).

#### To issue a credit memo: {#procedure_N1311558}

1.  Go to _Transactions > Customers > Issue Credit Memos (Administrator)_.
    
2.  Under Primary Information:
    
    1.  In the **Custom Form** field, select the credit memo form you want to use.
        
    2.  Select the customer you are crediting.
        
    3.  Accept today's date, or enter another.
        
    4.  If you use accounting periods, select the posting period for this credit.
        
    5.  Enter the customer's original purchase order number.
        
    6.  If you like, enter a memo that will appear on the 2-line Accounts Receivable register.
        
3.  Under Sales Information:
    
    1.  You can change the sales effective date for this transaction. The sales effective date determines which commission plan and historical sales team this transaction applies to.
        
    2.  Check **Exclude Commissions** to exclude this transaction and its subordinate transactions from inclusion in all commission calculations. For example, selecting this box on a sales order excludes the sales order and the resulting invoice from all commission calculations for all sales people.
        
4.  Under Classification, select a department, class, and location you want this order associated with.
    
    Note:
    
    If you use NetSuite OneWorld and the selected customer is shared with multiple subsidiaries, you can choose any subsidiary assigned to the selected customer. For information about sharing customer records with multiple subsidiaries, see [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
    
5.  On the **Items** subtab, enter information about each item credited, and click **Add** after each.
    
    If the item being returned is a serialized item, you can:
    
    -   enter the customer name, then enter the item number in the item field. Next, click **List** to select the serial number sold to this customer.
        
    -   enter the serial number and the item number will autofill the Item field.
        
    
    For more information, see [Adding Items on a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588373194.html).
    
6.  On the **Billing** subtab, the default billing address for the selected customer is displayed in the **Bill To** field. You can change this address as needed. For more information, see [Adding Billing Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588267772.html).
    
7.  On the **Shipping** subtab, enter the shipping details for this transaction. For more information, see [Entering Shipping Information about a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4593450742.html).
    
8.  The Accounting subtab only shows if you are using the Multiple Currencies or Revenue Recognition features, if you have not enabled the Per-Line Taxes preference at _Setup > Accounting > Taxes > Set Up Taxes (Administrator)_, or if you have added fields to this subtab. For more information, see [Entering Accounting information about a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4587464246.html).
    
9.  On the **Relationships** subtab, enter a contact or partner details for this transaction. For more information, see [Entering Relationships on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586861907.html).
    
10.  On the **Sales Team** subtab, if you use the Team Selling feature, select the Sales Team for this transaction. For more information, see [Associating Sales Teams with Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038639.html).
     
11.  On the **Communication** subtab, enter communication information for this transaction. For more information, see [Entering Communication Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586862223.html).
     
12.  Click **Save**.
     

If you issue a credit memo after a customer has paid an invoice, this memo can be applied to any of the customer's open or future invoices. To do this, go to _Transactions > Customers > Accept Customer Payments (Administrator)_, and select the appropriate customer.

### Related Topics:

-   [Customer Credit Memos](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1311306.html)
-   [Crediting an Authorized Customer Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1312244.html)
-   [Applying a Customer Credit Memo](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1312521.html)
-   [Printing a Customer Credit Memo](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1313142.html)
-   [Processing Return Authorizations and Credit Transactions with a Different Location in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0708104225.html)
-   [Refunding an Authorized Customer Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1313511.html)
-   [Refunding an Open Balance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1313840.html)
-   [Credit Memo Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N408112.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
