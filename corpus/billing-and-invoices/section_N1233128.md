---
id: "section_N1233128"
type: "section"
title: "Statement Charges"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Billing > Statement Charges"
parent: "chapter_4419712298"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233128.html"
anchors: ["procedure_N1233156"]
sha256: "712c91a7d2a1bd7a49afde98c301a7cad679ddeb858f20f6d68844bca993a58a"
---

Statement charges work like invoices because they track payments you expect from customers. If you want to add up several charges before sending a billing statement to a customer, use statement charges instead of invoices.

For example, a landscaping company offers weekly lawn service to its customers. Each weekly service costs $50. You enter a $50 statement charge each week the lawn service is done. Then, one time each month, you send a statement to the customer showing the total due for services.

#### To enter a statement charge: {#procedure_N1233156}

1.  Go to _Transactions > Sales > Create Statement Charges_ (Administrator).
    
2.  In the **A/R Account** field, choose the account you want to post this statement charge to.
    
3.  In the **Customer** or **Project** field, select the appropriate customer or project.
    
    The currency selected on the customer's record appears here as well as the exchange rate for this customer's currency.
    
    Note:
    
    NetSuite enables you to create a statement charge for intercompany customers and inventory items.
    
4.  Enter a new rate to update this currency's exchange rate.
    
    Note:
    
    If the Advanced Pricing feature is enabled, the Rate field on statement charges is determined by your configured price rules. The rate is sourced based on the transaction date for the statement charge. This may result in rates that differ from those shown without Advanced Pricing enabled.
    
5.  In the **Date** field, accept, enter or pick the correct date.
    
6.  In the **Posting Period** field, select the month and year you want this charge to post.
    
7.  In the **Ref. No.** field, accept or enter a reference number.
    
8.  In the **Due Date** field, enter or pick a date this charge is due.
    
9.  In the **Item** field, select the item to which this charge applies.
    
10.  In the **Quantity** field, enter the appropriate quantity.
     
11.  In the **Description** field, accept or enter a description for this customer charge.
     
     In the Rate field, the rate for the item automatically appears.
     
     In the Total field, the amount in the Quantity field is multiplied by the amount in the Rate field.
     
12.  If you track departments, select the appropriate department for this charge in the **Department** field.
     
13.  If you use NetSuite OneWorld and the selected customer is shared with multiple subsidiaries, you can choose any subsidiary assigned to the selected customer. If you haven't shared the customer record with multiple subsidiaries, you'll see the primary subsidiary as read-only.
     
     For information about sharing customer records with multiple subsidiaries, see [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
     
14.  If you track classes, select the appropriate class for this charge in the **Class** field.
     
15.  Click **Save**.
     

After you create statement charges, you can send them to your customers by generating statements. How you generate statements depends on your role.

-   To generate statements as an Administrator, go to _Transactions > Customers > Generate Statements_.
    
-   To generate statements using the A/R Clerk role, go to _Billing > Sales > Generate Statements_.
    

### Related Topics

-   [Deciding Between Invoices and Cash Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233061.html)
-   [Adding Billing Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588267772.html)
-   [Using Billing Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233375.html)
-   [Using Consolidated Billing for Projects and for Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233909.html)
-   [Creating Terms of Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234186.html)
-   [Using Terms of Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234578.html)
-   [Remittance Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234795.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
