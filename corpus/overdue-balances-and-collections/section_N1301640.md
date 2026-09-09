---
id: "section_N1301640"
type: "section"
title: "Finance Charges"
branch: "overdue-balances-and-collections"
category: "order-management"
breadcrumb: "Order Management > Overdue Balances and Collections > Finance Charges"
parent: "section_N1302093"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1301640.html"
anchors: ["bridgehead_N1301704", "procedure_N1301727", "bridgehead_N1301877", "procedure_N1301913"]
sha256: "c4fb815e1ff7149f83e520e7fa57438dd4150909e2cd73003c778d228ae80440"
---

Many businesses charge late fees or finance charges on invoices that are overdue. This allows business owners to recover costs incurred by carrying unpaid bills on their books. Finance charges are usually calculated on a monthly basis for all transactions that meet the criteria that set up by the business owner.

To set up finance changes, go to _Setup > Accounting > Preferences > Finance Charge Preferences_ (Administrator).

After the finance charge process is set up, you can begin to assess charges. To do this, go to _Transactions > Customers > Assess Finance Charges_ (Administrator).

All of the navigation paths in this chapter use the Administrator role.

## Setting Up Finance Charges {#bridgehead_N1301704}

Many businesses charge late fees or finance charges on overdue invoices. This allows business owners to recover costs incurred by carrying unpaid bills on their books. Finance charges are usually calculated on a monthly basis.

#### To set up finance charges: {#procedure_N1301727}

1.  Go to _Setup > Accounting > Preferences > Finance Charge Preferences_.
    
2.  In the **Annual Rate %** field, specify the annual percentage rate of interest you charge on unpaid balances.
    
3.  In the **Income Account** field, use the dropdown list to select the income account that will be credited by this finance charge.
    
4.  In the **Grace Period** field, enter the number of days you allow from the due date of an invoice before you begin to assess finance charges.
    
5.  In the **Minimum Finance Charge** field, enter the minimum finance charge you apply.
    
6.  In the **Assess on Finance Charges** field, place a check mark in the box if you assess finance charges on previously assessed unpaid finance charges.
    
7.  In the **Assess From** field, chose one:
    
    -   **Due Date** if you begin to assess finance charges only when an invoice is due
        
    -   **Transaction Date** if you begin to assess finance charges from the date of transaction
        
8.  In the **Custom Form** field, use the dropdown list to select the form on which you would like to invoice finance charges.
    
    Most companies choose the Standard Finance Charge Invoice, but you can customize the Finance Charge Invoice.
    
9.  When you have finished, click **Save**.
    

Note:

You can update your finance charge settings by going to _Setup > Accounting > Preferences > Finance Charge Preferences_. You cannot change finance charge settings by going at _Lists > Accounting > Items._.

Important:

In accounts with a U.S. parent company, the **Tax Code** field on the Finance Charge Preferences page is currently not being saved. When adding items to an invoice, add a finance charge in the **Item** column, and select the appropriate tax code for it in the **Tax Code** column.

Note:

On Finance Charge transaction, tax code is always "Non-Taxable" regardless any settings and default tax codes.

## Assessing Finance Charges {#bridgehead_N1301877}

Before you can assess finance charges in NetSuite, you must first set up the details of how you charge them. To set up finance changes, go to _Setup > Accounting > Preferences > Finance Charge Preferences_.

#### To assess finance charges: {#procedure_N1301913}

1.  Go to _Transactions > Customers > Assess Finance Charges_.
    
2.  Accept today's date for the transaction, or enter another.
    
    The **Amount** field updates to show the total finance charges you are assessing. Amounts in currencies other than your base currency are converted to your base currency for this total.
    
    Note:
    
    You can only assess finance charges for a customer one time per day even if subsequent charges would be in different currencies than the first finance charge.
    
3.  Choose to print, email or fax the finance charge invoices.
    
    In the fields **To Be Printed**, **To Be Emailed**, and **To Be Faxed**, set your preferences for sending the completed form. You can make a selection in each field individually.
    
    -   Select **Yes** if you want to send the form using the method indicated.
        
        For example, select Yes in the To Be Faxed field to fax the form.
        
    -   Select **No** if you do NOT want to send the form using the method indicated.
        
        For example, select No in the To Be Emailed field to not email the form.
        
    -   Select **Respect Customer Preference** to send the form based on the default preference on the customer record.
        
        For example, if the customer's record indicates to send forms via fax, then the completed form is faxed.
        
        You can set the preference on the Info subtab of a customer record in the Send Transactions Via field.
        
4.  Check the box in front of each customer account on which you want to assess finance charges. You can manually adjust the amount you want to assess for each customer.
    
    If you use the Multiple Currencies feature, each customer with an outstanding finance charge appears in the list one time for each currency in which they have a finance charge. For more information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).
    
5.  Click **Save**.
    

### Related Topics:

-   [Overdue Balances and Collections](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1302093.html)
-   [Dunning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4022915403.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
