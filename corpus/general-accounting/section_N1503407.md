---
id: "section_N1503407"
type: "section"
title: "Setting Up a Budget"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Budgets > Budgets in NetSuite > Setting Up a Budget"
parent: "chapter_N1503165"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1503407.html"
anchors: ["procedure_N1503431"]
sha256: "5e5207dff4b102501f6f5fd90d522f81dc718c56a5d77b65b75f8e6a89241c4e"
---

Each budget in NetSuite covers a fiscal year, for which you can enter an amount, per account, for each period. In NetSuite OneWorld, budgets are specific to a subsidiary and fiscal year. If the Multi-Book Accounting feature is enabled, each budget is for an accounting book and subsidiary pair for a year.

You can create specific budgets for the following:

-   Customers or Projects
    
-   Items
    
-   Classes
    
-   Departments
    
-   Locations
    

You can also enter budgets for statistical accounts. For example, you can add a budget for the headcount statistical account. In that budget, you can specify the number of new employee requisitions for the Sales Department in the upcoming financial year. You can then compare the budgeted amount against the number of new employees by customizing the Budget vs. Actual report. For more information, see [Using Statistical Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3841945149.html) and [Budget vs. Actual Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2097218.html).

Note:

If you use NetSuite OneWorld, also see [Subsidiary Budgets in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506361.html).

If you use Multiple Budgets, read [Multiple Budgets and Budget Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506174.html) before you begin budget setup.

#### To set up a budget: {#procedure_N1503431}

1.  Go to _Transactions > Financial > Set Up Budgets_.
    
2.  Select the **Accounting Book** for the budget if applicable.
    
    The **Accounting Book** field appears only when you use the Multi-Book Accounting feature. For more information about creating budgets for secondary accounting books, see [Budgets for Secondary Accounting Books](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1545224080.html).
    
3.  Select a **Subsidiary** for the budget, if applicable.
    
    The **Subsidiary** field appears only in NetSuite OneWorld accounts.
    
4.  In the **Year** field, select the fiscal year for which you want to create a budget.
    
5.  In the **Budget Category** field, select the category for this budget or create a new one.
    
    The **Budget Category** field appears only when the Multiple Budgets feature is enabled. For more information, see [Multiple Budgets and Budget Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506174.html).
    
    For example, if you're creating a budget for a statistical account, create a new category and then name it Statistical Accounts.
    
    When the Multiple Budgets and Multiple Currencies features are enabled, you'll also see these fields:
    
    -   **Budget Category Type** - Displays the value Global or Local. **Global** indicates that the budget is defined in the base currency of the root parent subsidiary. Local is an option only for OneWorld accounts. **Local** indicates that the budget is defined in the base currency of the selected subsidiary.
        
    -   **Currency** - Displays the currency in which the budget is defined. This field appears only in OneWorld accounts. The value depends on the Subsidiary selected and Budget Category Type for the Budget Category.
        
6.  To create a budget for specific criteria, select options for one or more of the following fields:
    
    -   **Customers or Projects**
        
    -   **Items**
        
    -   **Classes**
        
    -   **Departments**
        
    -   **Locations**
        
    -   **Custom Segments**
        
7.  To filter the accounts that are listed for the budget, select an **Account Type**. The options are:
    
    -   **Income and Expense** - accounts included in both income and expense sections of Income Statement reports.
        
    -   **Income** - accounts included in income sections of Income Statement reports.
        
    -   **Expense** - accounts included in expense sections of Income Statement reports.
        
    -   **Balance Sheet** - accounts included in Balance Sheet reports, assets, liabilities, and equities.
        
    -   **Existing** - shows only accounts that have existing budget amounts
        
    -   **All** - accounts included in Income Statement, Balance Sheet reports, and statistical accounts.
        
    
    The Budget page displays the accounts in your system specific to the selected account type. It also displays an Apply box, which includes or excludes a specific account in the budget as well as the months of the year.
    
8.  Enter budget amounts in positive numbers for the year using one or a combination of the following options. (For tips on entering data and completing forms, see [Keyboard Shortcuts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N474926.html).)
    
    -   Enter individual values for the account for each month (or accounting period).
        
    -   Enter amounts in the first period, and use the buttons at the top of the account list to populate the other periods.
        
        -   To copy the amount in the first month to all months, check the box in the **Apply** column for the account, and click **Fill**.
            
            In the example in the screenshot, the 12,000.00 in Jan 2019 for the 4000 Sales account would be copied to the other months. The total budget for the account line for the year would be $144,000.
            
        -   To divide the amount in the first month across all months, check the box in the **Apply** column for the account, and click **Distribute**.
            
            In the example in the screenshot, the 12,000.00 in Jan 2019 for the 4000 Sales account would be divided by 12. Each period would have a budgeted amount of 1,000.00.
            
    -   To check all the boxes in the **Apply** column, click **Mark All**.
        
    -   To clear all boxes in the **Apply** column, click **Unmark All**.
        
    -   Click **Clear** to delete all the existing budget amounts.
        
9.  When you've finished entering budget details, click **Save**.
    

Use the Budget Income Statement at _Reports > Banking/Budgeting > Budget Income Statement_ to view the budget. For information about this report, see [Budget Income Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2095701.html).

Note:

Budget data is not displayed in reports if the Report by Period preference is set to Never. If your report's budget columns display all zeros, go to _Home > Set Preferences_. On the Analytics subtab, set the Report by Period preference to All Reports or to Financials Only.

### Related Topics

-   [Budgets in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1503165.html)
-   [Copying a Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1505228.html)
-   [Importing a Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1505717.html)
-   [Multiple Budgets and Budget Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506174.html)
-   [Budget-Related Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158801165026.html)
-   [Subsidiary Budgets in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506361.html)
-   [Budgets for Secondary Accounting Books](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1545224080.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
