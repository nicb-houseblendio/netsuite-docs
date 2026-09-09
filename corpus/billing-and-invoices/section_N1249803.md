---
id: "section_N1249803"
type: "section"
title: "Billing Time to Customers"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Invoices > Billing Costs to Customers > Billing Time to Customers"
parent: "section_N1248576"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1249803.html"
anchors: ["procedure_N1249865"]
sha256: "b0a6a14d46d9de10ab965b9b9eff420f82314005225321c6eb93c8e53cf71dc7"
---

Billing time back to customers lets you to enter time spent on a project for customers, and then bill the cost to them. For example, a locksmith can bill a customer for the time an employee spent installing a safe.

#### To bill time to customers: {#procedure_N1249865}

1.  Enable the Bill Costs to Customers and Time Tracking features:
    
    1.  Go to _Setup > Company > Enable Features_.
        
    2.  On the Transactions subtab, check the **Bill Costs To Customers** box.
        
    3.  On the **Employees** subtab, check the **Time Tracking** box, and then click **Save**.
        
    
    Note:
    
    For OneWorld accounts, you must also set up at least one tax schedule because Advanced Taxes is enabled in all OneWorld accounts.
    
    Note:
    
    In accounts without OneWorld, you can bill costs to customers using items created before enabling the Advanced Taxes feature. If you enable Advanced Taxes after creating an item, you must assign a tax schedule to the item to bill a customer.
    
2.  (Optional) Set preferences to determine ways you track and process the hours that employees work. For more information, see [Setting Up Time Tracking Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902575.html).
    
3.  Enter a time tracking transaction for time you want to bill.
    
    1.  Go to _Transactions > Employees > Track Time_.
        
    2.  When you enter a time tracking transaction for billable time, select the customer or project and service item, and ensure that the **Billable** box is checked.
        
        Then, when you create an invoice, this time appears on the **Billable Time** subtab.
        
        Note:
        
        If the Advanced Pricing feature is enabled, the Rate column on the Billable Time subtab will reflect rates determined by your configured price rules. The rate is sourced according to the transaction date entered on the Invoice or Cash Sale. This may differ from standard rates that do not use rule-based pricing.
        
    
    For more information about creating a time transaction, read [Entering a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904108.html).
    
4.  Create an invoice or cash sale that applies the billable time.
    
    1.  Go to _Billing > Sales > Create Invoices_.
        
    2.  When you create an invoice, apply the appropriate billable time on the **Billable Time** subtab. Click **Mark All** or **Unmark All** to check or clear all time that shows on the subtab.
        
        Note:
        
        To generate deferred revenue for billable time, you must manually select revenue recognition schedules on the **Billable Time** subtab.
        
        For more information about creating an invoice, read [Creating an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html).
        
    3.  To create a cash sale, go to _Billing > Sales > Enter Cash Sales._. For more information, see [Cash Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1244343.html).
        
5.  If you track class, department, and location at the line-item level, you can change these settings for this billable time.
    

When you create the invoice or cash sale, NetSuite bills the customer for the time.

When you bill time back to customers, you can also use billing classes. Billing classes set billable time rates for service items based on employees. For example, a law office can use billing classes to charge specific hourly rates for time billed by partners in the firm.

For more information about billing classes, read [Using Billing Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233375.html).

When billing time to customers, you can select to include the date of service on all custom invoices except finance charge invoices. If you combine time items on invoices, the date of service for all the time items you're billing is grouped under the last date the employee worked.

### Related Topics

-   [Billing Costs to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html)
-   [Billing Items to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248901.html)
-   [Billing Expenses to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1250082.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
