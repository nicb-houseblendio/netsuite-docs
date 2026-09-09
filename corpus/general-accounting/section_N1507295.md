---
id: "section_N1507295"
type: "section"
title: "Setting Up a Subsidiary Budget"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Budgets > Budgets in NetSuite > Subsidiary Budgets in OneWorld > Setting Up a Subsidiary Budget"
parent: "section_N1506361"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1507295.html"
anchors: ["procedure_N1507314"]
sha256: "b7b73c795a7e06c32aa4b947dd622e0e50544d4e1e6327b90e1cb6e70e38825d"
---

If you use NetSuite OneWorld, you can set up budgets for individual subsidiaries.

#### To create a subsidiary budget: {#procedure_N1507314}

1.  Go to _Transactions > Financial > Set Up Budgets_.
    
2.  In the **Subsidiary** field, select the name of the subsidiary.
    
    Note:
    
    Set the **Enable Budget with Elimination Subsidiaries** preference to be able to select an elimination subsidiary from this list.
    
3.  In the **Year** field, select the fiscal year for which you want to create a budget.
    
4.  In the **Budget Category** field, select:
    
    -   Any budget category defined for your company.
        
    -   **New** - to define a new budget category.
        
    -   **Legacy** - This is the budget category assigned to any budgets created before the Multiple Budgets feature was enabled. It has a budget category type of Global.
        
    
    When you select a defined budget category, NetSuite populates the **Budget Category Type** field with a read-only value, based on the status of the **Global** box for the selected budget category. Also, NetSuite populates the **Currency** field:
    
    -   If the budget category type is global, then the currency used is the root parent's base currency.
        
    -   If the budget category type is local, then the currency used is the subsidiary's base currency. If you're creating budgets in local currencies, then you could create multiple Budget Categories, for example, using alternate exchange rate assumptions.
        
5.  You can create specific budgets within a subsidiary for:
    
    -   **Customers or Projects**
        
    -   **Items**
        
    -   **Classes**
        
    -   **Departments**
        
    -   **Locations**
        
    -   **Custom Segments**
        
    
    To create a specific budget, select from the list for the appropriate field. Leave the fields blank to budget for the entire list in the field. For more information, see [Setting Up a Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1503407.html).
    
6.  In the **Account Type** field, you can select the types of accounts for which you're creating this budget. The options are as follows:
    
    -   **Income and Expense** - accounts included in both income and expense sections of Income Statement reports.
        
    -   **Income** - accounts included in income sections of Income Statement reports.
        
    -   **Expense** - accounts included in expense sections of Income Statement reports.
        
    -   **Balance Sheet** - accounts included in Balance Sheet reports, assets, liabilities, and equities.
        
    -   **Existing** - shows only accounts that have existing budget amounts
        
    -   **All** - accounts included in both Income Statement, statistical accounts, and Balance Sheet reports.
        
    
    Based on the **Account Type** that you select, NetSuite displays a list of the account lines for the that type of account.
    
7.  Enter budget amounts for each account.
    
8.  Click **Save**.
    

### Related Topics

-   [Subsidiary Budgets in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506361.html)
-   [Subsidiary Budgeting Scenario](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506662.html)
-   [Creating Budget Categories for Local Subsidiary Budgeting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506823.html)
-   [Guidelines for Copying a Subsidiary Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1507638.html)
-   [CSV Import for Subsidiary Budgets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1508163.html)
-   [Budget Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1508302.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
