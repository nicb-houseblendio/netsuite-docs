---
id: "section_N1247359"
type: "section"
title: "Refunding a Cash Sale"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Cash Sales > Refunding a Cash Sale"
parent: "section_N1244343"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1247359.html"
anchors: ["procedure_N1247376"]
sha256: "c3ff6b5b5cb466d2421e8b0725462f67049195d4ceb4e4bc157771440c046204"
---

A cash sale refund returns money to a customer who paid with cash, check, or credit card.

#### To refund a cash sale: {#procedure_N1247376}

1.  Go to _Transactions > Customers > Refund Cash Sales_.
    
2.  Under Primary Information:
    
    1.  In the **Custom Form** field, select a cash refund form.
        
    2.  Accept the next consecutive refund number, or enter another.
        
    3.  In the **Customer** or **Project** field, select the customer whose sale you are refunding.
        
    4.  (Optional) If you want to refund the money using a check, check the **Create Check** box.
        
        To print it later from the checks queue, check the **Print Check** box.
        
        Note:
        
        This is the only way to print the check. If you click **Print**, it prints the refund form, not the check.
        
    5.  (Optional) For credit card refunds, go to the **Billing** subtab. On the **Payment** subtab, fill out the credit card information.
        
    6.  Select the bank account for this refund.
        
        You'll see the associated currency here.
        
    7.  If you're using Multiple Currencies, select the currency for this transaction. You're limited to the currencies set on the customer's record. The customer's primary currency is selected automatically. For more information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).
        
        If you change the currency, prices and amounts are updated to the new currency.
        
    8.  You can change the exchange rate for this transaction only or update the rate on the currency record.
        
    9.  Accept today's date, or enter another.
        
    10.  Select the posting period.
         
    11.  If your customer paid by check, enter the check number.
         
    12.  Enter a memo with notes on the transaction.
         
         You can change the sales effective date for this transaction. The sales effective date determines which commission plan and historical sales team this transaction applies to.
         
3.  Under Sales Information:
    
    1.  Associate sales reps with this transaction by doing one of the following:
        
        -   If you don't use the Team Selling feature, in the **Sales Rep** field, select the sales rep or sales group.
            
            The sales rep or sales group associated with the customer on this transaction is chosen by default.
            
        -   If you use the Team Selling feature, click the **Sales Team** subtab.
            
            Select the sales team for this transaction. For more information, see [Associating Sales Teams with Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038639.html).
            
    2.  Select a partner to associate with this order. If you use the Multi-Partner Management feature, you can associate partners with this transaction on the [Entering Relationships on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586861907.html) subtab.
        
    3.  Check **Exclude Commissions** to exclude this transaction and its subordinates from inclusion in all commission calculations. For example, selecting this box on a sales order excludes the sales order and the resulting invoice from all commission calculations for all sales people.
        
    4.  You can change the sales effective date for this transaction. The sales effective date determines which commission plan and historical sales team this transaction applies to.
        
4.  Under Classification, select a subsidiary, department, class, and location you want this order associated with.
    
    Note:
    
    If you use NetSuite OneWorld and the selected customer is shared with multiple subsidiaries, you can choose any subsidiary assigned to the selected customer. For information about sharing customer records with multiple subsidiaries, see [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
    

The page for refunding a cash sale has several subtabs. The subtabs are determined by the setting and options you've enabled. The following list includes possible subtabs.

-   The [Adding Items on a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588373194.html) subtab.
    
-   The [Entering Shipping Information about a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4593450742.html) subtab.
    
-   The [Adding Billing Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588267772.html) subtab.
    
    Depending on your settings, billing information may display on the Payments subtab.
    
-   The [Entering Payment Information on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586835857.html) subtab.
    
-   The [Entering Accounting information about a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4587464246.html) subtab.
    
-   The [Entering Relationships on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586861907.html) subtab.
    
-   The [Associating Sales Teams with Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038639.html) subtab.
    
-   The [Entering Communication Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586862223.html) subtab.
    

If you refunded by check and click **Print**, it prints the refund form, not the check. To print the check, go to _Customers > Transactions > Print Checks and Forms_.

### Related Topics

-   [Entering a Cash Sale](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1244457.html)
-   [Printing a Sales Receipt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1247063.html)
-   [Approving Cash Sales that Have a Payment Hold](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4353156490.html)
-   [Managing Undeposited Cash Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248314.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
