---
id: "section_N1248576"
type: "section"
title: "Billing Costs to Customers"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Invoices > Billing Costs to Customers"
parent: "section_N1235134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html"
anchors: ["bridgehead_N1248734", "bridgehead_N1248799"]
sha256: "e6968cfbb23974e895ca8b4fb065e1a7a488e050c8944a1471ef4dadb2c06e04"
---

NetSuite lets you to bill costs back to customers for time, items, and expenses you incur while working on a project for them. For example, a locksmith can bill costs to customers in the following ways:

-   **Bill Items to Customers** - Bill a customer for a safe that was ordered.
    
-   **Bill Time to Customers** - Bill a customer for the time an employee spent installing a safe.
    
-   **Bill Expenses to Customers** - Bill a customer for subcontractor fees incurred to install a safe in another state.
    

To bill costs to customers, enable the feature first. An administrator can go to _Setup > Company > Enable Features_. On the **Transactions** subtab, check the **Bill Costs To Customers** box, and then click **Save**.

Note:

Unlike the items added to the Items subtab that are taxed based on the transaction shipping address, billable costs are taxed based on the customer's address.

Bill your costs to customers in one of the following ways:

-   **Enter the time, item or expense, and mark it as billable.**
    
    When you enter time transactions, purchase orders, bills, checks or credit card payments for time, an item or expense, check the **Billable** box. Then, assign a customer to be billed for the item or expense. When you bill the customer, the expense appears on a Billable subtab of the invoice or cash sale.
    
    Important:
    
    The **Billable** box has the following behavior:
    
    -   **Billable** field is disabled if you select a project without customer.
        
    -   **Billable** field is disabled if you select a non-billable project task.
        
    -   If you select a project without a billing type, the default value depends on accounting preference EXPENSES BILLABLE BY DEFAULT.
        
    -   If you select a project with billing type T&M or CB, the default value = T (it doesn't matter what the EXPENSES BILLABLE BY DEFAULT preference is set to).
        
    -   If you select a project with billing type FBI or FBM, the default value = F (it doesn't matter what the EXPENSES BILLABLE BY DEFAULT preference is set to).
        
    
    Note:
    
    If you enter the billable item on a purchase order, bill the purchase order before you bill the customer for the item.
    
-   **Create an invoice or cash sale to bill the customer for the cost you entered.**
    
    When you create a customer invoice or cash sale, the costs you bill to customers show on the Billable Items, Billable Expenses and Billable Time subtabs. After you select the customer on the bill, click the appropriate subtab, and check the line items you want to bill the customer for.
    
    Click **Mark All** or **Unmark All** to check or clear all items, expenses or time that show on the subtab.
    
    For more information, read [Creating an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html) or [Cash Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1244343.html).
    

The items and expenses appear as normal line items on the transaction. The customer only sees the selling price that includes the markup spread over the expense items. However, you'll see the markup as a separate entry when you view the invoice or cash sale in NetSuite.

## Preferences for Billing Costs {#bridgehead_N1248734}

When you use the Bill Costs to Customers feature, set a preference for invoices to include memos you enter on time and expense records. To set this preference, go to _Setup > Accounting > Preferences > Accounting Preferences_ > Time & Expenses. Check the **Copy Time Memos to Invoices** and **Copy Expense Memos to Invoices** boxes and then click **Save**.

Note:

When you set these preferences, the memos you've already entered on existing time and expense records show on invoices you create.

If you want to classify billable costs by class or department, enable the **Allow Per-Line Departments** and **Allow Per-Line Classes** preferences at _Setup > Accounting > Preferences > Accounting Preferences_ > General under Classifications.

To save time, you can create invoices in bulk for billable expenses, time, and items. For more information, read [Invoicing Billable Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1241287.html).

## Tracking Class, Department, and Location for Billable Costs {#bridgehead_N1248799}

If you track class and department on the line-item level, the bill's classifications (class, department, and location) are maintained on the billable subtabs, regardless of the invoice header settings.

You can change the classifications on the billable subtabs of the invoice.

Note:

If you group class, department, and location on invoices, the billable subtabs will use the classifications from the invoice header.

### Related Topics

-   [Billing Costs to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html)
-   [Billing Items to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248901.html)
-   [Billing Time to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1249803.html)
-   [Billing Expenses to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1250082.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
