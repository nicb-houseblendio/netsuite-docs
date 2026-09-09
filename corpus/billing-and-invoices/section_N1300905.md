---
id: "section_N1300905"
type: "section"
title: "Printing a Statement"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Invoices > Customer Statements > Printing a Statement"
parent: "section_N1300430"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1300905.html"
anchors: ["subsect_160692918259", "procedure_N1300964", "subsect_160692935158", "procedure_N1301129"]
sha256: "046641906ca9636392869f769f4cb7613f3d430cce11607d1f6a195bebfdb6d7"
---

You can print a customer statement to send to a customer.

Your administrator can customize the layout of your printed forms using advanced PDF/HTML templates. For more information, see [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html).

Click a link below for more information about printing a statement:

-   [Bulk Printing Statements](#subsect_160692918259)
    
-   [Printing Individual Statements](#subsect_160692935158)
    

## Bulk Printing Statements {#subsect_160692918259}

Follow this procedure to print many statements at one time.

#### To bulk print statements: {#procedure_N1300964}

1.  Go to one of the following:
    
    -   _Customers > Accounts Receivable > Print Checks and Forms_. On the Printing page, click **Statements**.
        
    -   _Customers > Accounts Receivable > Generate Statements_.
        
2.  In the **Statement Date** field, accept or enter the date you want to appear on your statements.
    
    Note:
    
    The system also uses this date to calculate aging.
    
3.  (Optional) Enter a start date for your statements.
    
    This is the date of the oldest transaction you want to appear on the statement.
    
    If you don't enter a start date, the Balance Forward doesn't appear and all transactions in the customer's history appear on the statement.
    
4.  (Optional) If you want to generate statements for customers with no outstanding balances, check the **Include Zero Balances** box.
    
5.  (Optional) If you want to include only open transactions, check the **Show Only Open Transactions** box.
    
    If you show only open transactions and don't include a start date, the statement includes all open transactions in your customer's history.
    
    Note:
    
    The Show Only Open Transaction option is most useful for statements printed as of your current today date. If you select Show Only Open Transactions and are using a date other that today's date, you may have balance discrepancies.
    
6.  If you use the Consolidated Payments feature, check the **Consolidated Statements** box to print out statements showing the overall balance for the customer-subcustomer hierarchies customers are a part of. Clear this box to print a statement showing only the balance for this customer.
    
    For more information, see [Consolidated Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288474.html).
    
7.  Select the customers to receive statements. You can click the box at the top to select all customers in the list. Click the box again to clear the box for all customers.
    
    Click **Customize** to customize the list to filter the customers listed or to add or remove columns.
    
8.  When you're done, click **Print**.
    

## Printing Individual Statements {#subsect_160692935158}

Follow this procedure to print a single statement.

#### To print an individual statement: {#procedure_N1301129}

1.  Go to _Customers > Accounts Receivable > Individual Statement_.
    
2.  Select the customer you want to generate and print a statement for.
    
3.  In the **Statement Date** field, accept or enter the date you want to appear on the statement.
    
4.  In the **Start Date** field, set the date of the earliest transactions you want to show on this statement. Leave this field blank if you want to show all transactions for this customer.
    
5.  If you use the Consolidated Payments feature, check the **Consolidated Statement** box to print out a statement showing the overall balance for the customer-subcustomer hierarchy this customer is a part of. Clear this box to print a statement showing only the balance for this customer.
    
    For more information, see [Consolidated Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288474.html).
    
6.  Generate the statement:
    
    -   Click **Print** to print the statement.
        
    -   Click **Email** to email the statement.
        
        To email the statement, the customer needs to have an email address in the customer's record first.
        
    -   Click **Fax** to fax the statement.
        
        Note:
        
        Each customer must also have a fax number entered on the customer's record.
        

### Related Topics:

-   [Customer Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1300430.html)
-   [Generating Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1300518.html)
-   [Printing Mini Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1301336.html)
-   [Advanced PDF/HTML Multi-Currency Statement Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4364689607.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
