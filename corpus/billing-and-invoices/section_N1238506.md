---
id: "section_N1238506"
type: "section"
title: "Creating an Invoice"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Invoices > Creating an Invoice"
parent: "section_N1235134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html"
anchors: ["procedure_N1238558"]
sha256: "de4a7c80a1eede05178ae4dc9720e76b38e56c127486665fa11c821fba398e1e"
---

Note:

For information specific to Not-for-Profit (NFP), see [Invoicing Pledges](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1525122362.html).

An invoice is a record of sale to a customer. Create an invoice when you don't get payment for goods or services at the time of delivery.

To record sales on invoices, add each item you sell from your Items list. Each invoice consists of line items and their sales amounts. The sum of all sales amounts on an invoice add up to the total amount the customer owes.

Note:

The fields described below show on standard invoice forms. To create a custom invoice form, go to _Setup > Customization > Forms > Transaction Forms_.

#### To create an invoice: {#procedure_N1238558}

1.  Go to _Billing > Sales > Create Invoices_.
    
2.  Under Primary Information:
    
    1.  In the **Custom Form** field, select the invoice form you want to use. Invoice forms can be standard or customized.
        
    2.  Accept or enter the invoice number in the **Invoice #** field.
        
        Note:
        
        You can edit an automatically generated invoice number only if your company allows it.
        
    3.  In the **Customer** or **Project** field, select the appropriate customer or project.
        
        Note:
        
        If you add, edit, or delete a project after a sales order is billed, the sales order becomes a standalone sales order and is no longer associated with the invoice. Also, the invoice is removed from the Related Records subtab on the sales order.
        
    4.  Accept or enter the date in the **Date** field.
        
        Note:
        
        If you edit the date on an invoice later, the new date also becomes the due date, even if a due date was previously set.
        
    5.  In the **Start Date** field, if you use Advanced Billing, enter the creation date for the first invoice.
        
    6.  In the **End Date** field, enter the date when this invoice is no longer valid.
        
    7.  If you use accounting periods, select the posting period for this invoice.
        
    8.  In the **Due Date** field, enter the invoice due date.
        
    9.  In the **PO#** field, enter any customer purchase order number associated with this invoice.
        
    10.  In the **Memo** field, enter a memo to help identify this invoice.
         
         When you use the Search Transactions feature, you can search for specific words and phrases in the **Memo** field.
         
3.  Under Sales Information:
    
    1.  Select the sales reps associated with this invoice.
        
        You can add sales reps to this transaction in these ways:
        
        -   If you don't use the Team Selling feature, select the sales rep or sales group in the **Sales Rep** field.
            
            The sales rep or sales group associated with the customer on this transaction is selected by default.
            
        -   If you use the Team Selling feature, click the **Sales Team** subtab.
            
            Select the sales team for this transaction. For more information, see [Associating Sales Teams with Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038639.html).
            
    2.  In the **Opportunity** field, select the opportunity for this invoice.
        
        You can change the sales effective date for this transaction. The sales effective date decides which commission plan and historical sales team this transaction applies to.
        
    3.  Check **Exclude Commissions** to exclude this transaction and its subordinate transactions from inclusion in all commission calculations. For example, checking this box on a sales order excludes the sales order and the resulting invoice from all commission calculations for all sales people.
        
    4.  In the **Lead Source** field, select the source of the lead for this invoice. If you use Marketing Automation, select the campaign you want to associate with this transaction's revenue.
        
    5.  The partner linked with this customer appears in the **Partner** field. You can select a different partner.
        
        If you have enabled the Multi-Partner Management feature, you can associate partners with this transaction on the Partners subtab. For more information, see [Associating Partners With Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167413.html).
        
    6.  Under **Classification**, select a department, class, or location for the invoice.
        
        Note:
        
        If you use NetSuite OneWorld and the selected customer is shared with multiple subsidiaries, you can select any subsidiary assigned to the selected customer. For information about sharing customer records with multiple subsidiaries, see [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
        

The Invoice page includes several subtabs. For more information about invoice subtabs, see the links in the following list:

-   The [Adding Items on a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588373194.html) subtab.
    
-   The [Entering Shipping Information about a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4593450742.html) subtab.
    
-   The [Adding Billing Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588267772.html) subtab.
    
-   The [Entering Accounting information about a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4587464246.html) subtab.
    
-   The [Entering Relationships on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586861907.html) subtab.
    
-   The [Associating Sales Teams with Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038639.html) subtab.
    
-   The [Entering Communication Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586862223.html) subtab.
    

You can apply terms to invoices by choosing a term on the invoice record or by setting default terms on the customer record. For more information, see [Using Terms of Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234578.html).

For information about enabling tax lookup, see [Enabling U.S. Tax Lookup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2041606.html).

### Related Topics

-   [Payment Date Prediction for Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0106021633.html)
-   [Custom Workflow Based Invoice Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html)
-   [Custom Invoice Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4438064774.html#bridgehead_N1235418)
-   [Classes and Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1238292.html)
-   [Custom Workflow Based Invoice Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html)
-   [Using the Billing Tab and Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4483926245.html)
-   [Choosing an Invoice Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240040.html)
-   [Billing Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4063198073.html)
-   [Billing or Invoicing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240951.html)
-   [Invoicing Billable Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1241287.html)
-   [Closing or Voiding an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158654862294.html)
-   [Creating Installments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540928779.html)
-   [Printing an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1242104.html)
-   [Progress Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1243687.html)
-   [Billing Costs to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html)
-   [Displaying Deposit Balance on Customer Statements and Remittance Slips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4204723346.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
