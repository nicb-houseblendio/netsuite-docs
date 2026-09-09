---
id: "section_N1505228"
type: "section"
title: "Copying a Budget"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Budgets > Budgets in NetSuite > Copying a Budget"
parent: "chapter_N1503165"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1505228.html"
anchors: ["bridgehead_4527945958", "procedure_N1505305", "bridgehead_N1505458", "procedure_N1505467"]
sha256: "d898e277513bdf2b7866697931d90332d5949f8be6489754e9aa7e1641ef041d"
---

You can save time by copying a previous year's budget or basing your budget on last year's actual results. Budgets provide an estimate of revenues and expenses for an account for a fiscal year.

Important:

Before you copy a subsidiary budget, see [Guidelines for Copying a Subsidiary Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1507638.html).

For information, see the following subtopics:

-   [Copying a Previous Year's Budget](#bridgehead_4527945958)
    
-   [Basing a Budget on a Previous Year's Actual Results](#bridgehead_N1505458)
    

## Copying a Previous Year's Budget {#bridgehead_4527945958}

The Copy Budget option creates a new budget record from a budget from different year. For example, if you want this year's budget to be the same as last year's budget, you can copy last year's budget to this year.

If the Accounting Periods feature is enabled, you can create a new budget by copying a budget from any fiscal year where a budget exists. Only those fiscal years where a budget exists can be selected as a source budget year. The process copies the values associated with the specified account types and budget categories to the new budget. If you're replacing the budget, the existing budget is deleted before the process copies the new budget.

If the Accounting Periods feature is **not** enabled, you can create a new budget by copying a budget from any year. The process verifies that a budget exists for the specified year. Then the values associated with the specified account types and budget categories are copied from the source budget to the new budget. If you're replacing the budget, the existing budget is deleted before the process copies the new budget. If a source budget doesn't exist for the specified year, the process leaves the new budget unchanged.

If the source budget doesn't contain data in a specific period, the new budget doesn't contain data for that period.

Note:

NetSuite lets you have only one budget per category per fiscal year. Copying a budget from one year and category to create a budget for the same year and category **doubles** the budgeted amount.

#### To copy a previous year's budget: {#procedure_N1505305}

1.  Go to _Transactions > Financial > Copy Budgets_.
    
2.  Select **From Budget Year**, and then select the year's budget from which you want to copy data.
    
3.  If the Multiple Budgets feature is enabled, in the **From Budget Category** field, select the budget category from which you want to copy.
    
    In NetSuite OneWorld, with the Multiple Budgets and Multiple Currencies features enabled, each budget category has a a type of global or local. This type determines the currency NetSuite uses for a subsidiary's budget and actual amounts.
    
4.  In the **To** fields, select the year and category (if applicable) you want the copied budget to represent.
    
    The **To** list includes all years for periods that have been set up in your account. See [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html).
    
5.  To retain detail information from the source budget into the copy, check the **Keep Detail** box for **Customers**, **Items**, **Departments**, **Classes**, or **Locations**.
    
6.  In the **Account Type** field, select the types of accounts you want to copy into the new budget.
    
    -   **Income** - accounts included in income sections of Income Statement reports.
        
    -   **Expense** - accounts included in expense sections of Income Statement reports.
        
    -   **Balance Sheet** - accounts included in Balance Sheet reports, assets, liabilities, and equities.
        
    -   **Income and Expense** - accounts included in both income and expense sections of Income Statement reports.
        
    -   **All** - accounts included in Income Statement, Balance Sheet reports, and statistical accounts.
        
7.  In the **Modify By** field, enter the percent by which you want to increase or decrease the budget amounts.
    
    -   Enter a positive percent to increase the budget amounts.
        
    -   Enter a negative percent to decrease the budget amounts.
        
8.  Use the **Replace** box to determine whether the copied budget replaces an existing budget or adds to it.
    
    -   Check the box to overwrite existing budget amounts with the copied budget amounts.
        
    -   Clear the box to add copied budget amounts to the existing budget
        
9.  Click **Save**.
    

## Basing a Budget on a Previous Year's Actual Results {#bridgehead_N1505458}

When you create a budget from the actual results of a previous year, NetSuite copies the values for account types and budget categories you specify. If you're replacing values in the new budget, the process deletes the existing budget before copying values to the new budget. This copying ensures that the new budget is identical to the results from a previous fiscal year.

#### To base a budget on a previous year's actual results: {#procedure_N1505467}

1.  Go to _Transactions > Financial > Copy Budgets_.
    
2.  Select **Actuals From Year**, and then choose the year's budget that you want to copy.
    
3.  In the **To Budget Year** field, select the year of the budget you're creating.
    
4.  If the Multiple Budgets feature is enabled, in the **Budget Category** field, select the category for the budget, or create a new one if necessary.
    
    In NetSuite OneWorld, with the Multiple Budgets and Multiple Currencies features enabled, each budget category has a a type of global or local. This type determines the currency NetSuite uses for a subsidiary's budget and actual amounts.
    
5.  In the **Account Type** field, choose the types of accounts you want to copy into the new budget:
    
    -   **Income** - accounts included in income sections of Income Statement reports.
        
    -   **Expense** - accounts included in expense sections of Income Statement reports.
        
    -   **Balance Sheet** - accounts included in Balance Sheet reports, assets, liabilities, and equities.
        
    -   **Income and Expense** - accounts included in both income and expense sections of Income Statement reports.
        
    -   **All** - accounts included in Income Statement, Balance Sheet reports, and statistical accounts.
        
6.  In the **Modify By** field, enter the percent by which you want to increase or decrease the budget amounts.
    
    -   Enter a positive percent to increase the budget amounts.
        
    -   Enter a negative percent to decrease the budget amounts.
        
7.  Use the **Replace** box to determine whether the copied budget replaces an existing budget or adds to it.
    
    -   Check the box to overwrite existing budget amounts with the copied budget amounts.
        
    -   Clear the box to add copied budget amounts to the existing budget
        
8.  To retain detail information from the source budget into the copy, check the **Keep Detail** box for **Customers**, **Items**, **Departments**, **Classes**, or **Locations**.
    
    If you clear all of these boxes, the new budget has no customer, item, department, class, or location criteria.
    
9.  Click **Save**.
    

### Related Topics

-   [Budgets in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1503165.html)
-   [Setting Up a Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1503407.html)
-   [Importing a Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1505717.html)
-   [Multiple Budgets and Budget Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506174.html)
-   [Budget-Related Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158801165026.html)
-   [Subsidiary Budgets in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506361.html)
-   [Budgets for Secondary Accounting Books](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1545224080.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
