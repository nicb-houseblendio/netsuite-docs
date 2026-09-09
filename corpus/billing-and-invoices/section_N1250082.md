---
id: "section_N1250082"
type: "section"
title: "Billing Expenses to Customers"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Invoices > Billing Costs to Customers > Billing Expenses to Customers"
parent: "section_N1248576"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1250082.html"
anchors: ["procedure_N1250131", "procedure_N1250353", "procedure_N1250411", "bridgehead_N1250469", "bridgehead_N1250504"]
sha256: "850164280e122f3c6d58e0697cf48884b83517a59e3c292b2c19b65d2e643a33"
---

Billing expenses back to customers lets you to bill customers for the costs you incur while working on a project. For example, a locksmith can bill a customer for subcontractor fees incurred to install a safe for a customer in another state.

To bill expenses back to customers, enable the feature first. An administrator can go to _Setup > Company > Enable Features_. On the Transactions subtab, check the **Bill Costs To Customers** box, and then click **Save**.

When you enable the feature, you can bill expenses to customers on purchase orders or other purchase transactions.

Note:

For OneWorld accounts, you must also set up at least one tax schedule because Advanced Taxes is enabled in all OneWorld accounts.

Note:

In accounts without OneWorld, you can bill costs to customers using items created before enabling the Advanced Taxes feature. If you enable Advanced Taxes after creating an item, assign a tax schedule to the item to bill a customer.

#### To bill expenses to customers using purchase orders: {#procedure_N1250131}

1.  Enter a purchase order for an expense you want to bill to a customer.
    
    When you enter a purchase order for a billable expense, select the expense and identify the customer or project, and then check the **Billable** box.
    
    Note:
    
    You must bill the purchase order before you can bill the customer for the billable expense.
    
    To enter a purchase order for a billable expense, go to _Transactions > Purchases/Vendors > Enter Purchase Orders_.
    
    For more information about purchasing billable expenses, read [Entering a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400504.html).
    
2.  Bill the purchase order that includes the expense you want to bill to a customer.
    
    The bill for the billable expense needs to identify the customer or project and have the **Billable** box checked.
    
    To bill a purchase order, go to _Transactions > Purchases/Vendors > Bill Purchase Orders_.
    
    For more information, read [Billing a Purchase Order With Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403862.html).
    
    After the purchase order is billed, this expense can show on the Billable Expenses subtab of the customer bill.
    
3.  Enter an invoice or cash sale to bill the customer for the billable expense.
    
    When you create an invoice, apply the appropriate billable expense on the **Billable Expenses** subtab. Click **Mark All** or **Unmark All** to check or clear all expenses that show on the subtab.
    
    -   To create an invoice, go to _Billing > Sales > Create Invoices_.
        
        For more information about creating an invoice, read [Creating an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html).
        
    -   To create a cash sale, go to _Billing > Sales > Enter Cash Sales._. For more information, see [Cash Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1244343.html).
        
        For more information about creating a cash sale, read [Entering a Cash Sale](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1244457.html).
        
4.  If you track class, department, and location at the line-item level, you can change these settings for this billable item.
    

When you create the invoice or cash sale, the customer is billed for the expense.

#### To bill expenses to customers using checks: {#procedure_N1250353}

1.  Enter a check to pay a vendor for the item you want to bill to a customer. For more information, read [Adding Expenses to a Check](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1544419.html).
    
2.  On the **Expenses** subtab of the check, select the expense you want to bill to the customer.
    
3.  Identify the customer or project and check the **Billable** box.
    
4.  Complete additional fields on the check as necessary.
    
5.  Click **Save**.
    

Now, this expense can show on the **Billable Items** subtab of the customer bill.

#### To bill expenses to customers using credit card transactions: {#procedure_N1250411}

1.  Enter a credit card transaction to pay a vendor for the expense you want to bill to a customer. For more information, read [Entering Company Credit Card Charges](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1548500.html).
    
2.  On the **Expenses** subtab of the credit card transaction, select the expense you want to bill to the customer.
    
3.  Identify the customer or project and check the **Billable** box.
    
4.  Complete additional fields on the credit card transaction as necessary.
    
5.  Click **Save**.
    

Now, this expense can show on the Billable Expenses subtab of the customer bill.

## Expenses Billable By Default {#bridgehead_N1250469}

You can also set the **Expenses Billable by Default** preference to check the **Billable** box by default when you're creating purchase orders. Then, when you select a customer on an item line of a purchase transaction, the **Billable** box is automatically checked.

You can set the **Expenses Billable by Default** preference at _Setup > Accounting > Preferences > Accounting Preferences_ > Time & Expenses subtab. This preference is dependent on the Bill Costs to Customers feature.

## Copy Expense Memos to Invoices {#bridgehead_N1250504}

You can also set a preference for invoices to include memos entered on billable expenses. To set this preference, go to _Setup > Accounting > Preferences > Accounting Preferences_ > Time & Expenses. Check the **Copy Expense Memos to Invoices** box and then click **Save**.

Note:

When you set this preference, the memos you enter on existing expense records show on invoices you create.

When billing expenses back to customers, you can select to include the date of service on all custom invoices except finance charge invoices. This is the date the bill for the expenses was entered.

### Related Topics

-   [Billing Costs to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html)
-   [Billing Items to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248901.html)
-   [Billing Time to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1249803.html)
-   [Custom Workflow Based Invoice Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html)
-   [Using the Billing Tab and Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4483926245.html)
-   [Global Invoicing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1237960.html)
-   [Creating an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html)
-   [Choosing an Invoice Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240040.html)
-   [Billing Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4063198073.html)
-   [Billing or Invoicing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240951.html)
-   [Invoicing Billable Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1241287.html)
-   [Closing or Voiding an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158654862294.html)
-   [Creating Installments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540928779.html)
-   [Printing an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1242104.html)
-   [Progress Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1243687.html)
-   [Displaying Deposit Balance on Customer Statements and Remittance Slips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4204723346.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
