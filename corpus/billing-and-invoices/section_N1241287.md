---
id: "section_N1241287"
type: "section"
title: "Invoicing Billable Customers"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Invoices > Invoicing Billable Customers"
parent: "section_N1235134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1241287.html"
anchors: ["procedure_N1241335"]
sha256: "b7d7f231937696eb3bd82f31f70c1ae3eeb21312cb75ad74ced864463dfaf2ad"
---

When you use the Bill Costs to Customers feature, you can save time by invoicing customers in bulk for billable expenses, items, and time.

If you use the Multiple Currencies feature, you can create invoices only in each customer's primary currency. For more information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).

The Invoice Billable Customers page includes lines from the vendor bill and any applied vendor credit, so you can see which lines are already billed with a credit.

Note:

If the Advanced Pricing feature is enabled, the rate displayed in the Estimate column on the Invoice Billable Customers page is determined by your configured price rules. The rate is sourced based on the invoice date, and may differ from the standard rate if Advanced Pricing is not enabled.

Note:

You can't fulfill or bill sales orders with the status Pending Approval. You also can't close lines on a sales order with this status. If you need to make changes to an order that's pending approval, you can remove line items.

#### To bulk bill customers: {#procedure_N1241335}

1.  Go to _Billing > Sales > Invoice Billable Customers_.
    
2.  Enter the Invoice date to apply to all invoices you're creating.
    
3.  From the **Account** list, select the accounts receivable account to post to.
    
    To set the default A/R account, go to _Setup > Accounting > Accounting Preferences_ (Administrator).
    
    If you want the invoices created to use each customer's default, select **Respect Customer Preference**. You can set the default A/R account for a customer on the Financial subtab of the customer record.
    
4.  From the **Form** list, select the form you want to use for the invoices.
    
5.  Print, email, or fax the invoices.
    
    In the fields **To Be Printed**, **To Be Emailed**, and **To Be Faxed**, set your preferences for sending the completed form. You can select an option in each field individually.
    
    -   Select **Yes** if you want to send the form using the method indicated.
        
        For example, select Yes in the **To Be Faxed** field to fax the form.
        
    -   Select **No** if you don't want to send the form using the method indicated.
        
        For example, select No in the **To Be Emailed** field to not email the form.
        
    -   Select **Respect Customer Preference** to send the form based on the default preference on the customer record.
        
        For example, if the customer's record indicates to send forms by fax, then the completed form is faxed.
        
        Set the preference on the Info subtab of a customer record in the **Send Transactions Via** field.
        
6.  Filter the transactions in the list by checking the **Expenses**, **Items**, or **Time** box. For example, when you check the **Expenses** box, the list shows only transactions for customers with billable expenses.
    
7.  Check the **Charges** box if you want to invoice billable charges.
    
8.  Check the **Credit Card Approved** box if the credit card transaction occurred outside of NetSuite. For example, a charge at a card-swipe terminal.
    
9.  Check the **Show Invoices** box to show a list of invoices created when you submit this page.
    
10.  In the **Bill Date** field, filter the list of transactions by selecting a date range. Then, you can filter the list of transactions to process billable transactions for a particular time frame.
     
     For example, a lawyer can filter the transaction list for billable time during the previous month. Then, customers can be invoiced monthly for billable time accrued during the previous calendar month.
     
11.  Select the invoices to create by checking the **Invoice** box next to the transaction.
     
12.  Click **Submit**.
     

For each transaction you checked, NetSuite creates an invoice using your preferred invoice form. The Results page lists all invoices created in this bulk process.

Note:

When you enter billable time using the Vendor Center for a service item with a price, the billable time shows when you invoice billable customers. The rate shown is the price on the item record.

### Related Topics

-   [Custom Workflow Based Invoice Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html)
-   [Custom Workflow Based Invoice Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html)
-   [Using the Billing Tab and Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4483926245.html)
-   [Global Invoicing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1237960.html)
-   [Creating an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html)
-   [Choosing an Invoice Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240040.html)
-   [Billing Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4063198073.html)
-   [Billing or Invoicing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240951.html)
-   [Closing or Voiding an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158654862294.html)
-   [Creating Installments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540928779.html)
-   [Printing an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1242104.html)
-   [Progress Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1243687.html)
-   [Billing Costs to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html)
-   [Displaying Deposit Balance on Customer Statements and Remittance Slips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4204723346.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
