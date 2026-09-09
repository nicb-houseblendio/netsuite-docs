---
id: "section_N1476983"
type: "section"
title: "Enabling Intercompany Time and Expenses"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Journal Entries in OneWorld > Enabling Intercompany Time and Expenses"
parent: "section_N1475513"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html"
anchors: []
sha256: "c9bb1edc92f382e16aafe319905f91678eb7447819850cc4c324cbe08b31c027"
---

In OneWorld accounts, before you can enter transactions for an entity such as a customer, a vendor, or an employee, you must assign a single subsidiary to that entity. Transactions involving a customer or vendor generally impact the accounts of the subsidiary assigned to that customer or vendor. Time and expenses entered for an employee generally impact the subsidiary assigned to that employee.

In a multi-subsidiary environment, some transactions may involve more than one subsidiary, impacting the accounts of more than one subsidiary. For example, employees assigned to one subsidiary may be required to enter time or expenses for customers assigned to a different subsidiary. The Intercompany Time and Expense feature enables entry of intercompany time and expenses, and the transfer of time, expense, or both charges from one subsidiary to another.

You can enable the Intercompany Time and Expense feature at _Setup > Company > EnableFeatures,_, on the Accounting subtab.

Note:

If you enabled this feature after April 2014, when you created a qualifying journal entry the system created a single Intercompany Clearing Account of the Type: Other Current Asset. The account was set to the Root Subsidiary and included all child subsidiaries. Adjustment journal entries correctly posted to this new account, and no other currency-locked Intercompany Clearing Accounts were created.

If you enabled this feature prior to April 2014, creating a new adjustment journal entry caused the system to create a new Intercompany Clearing Account (no currency). This account then became the parent of all other existing clearing accounts. New adjustment journal entries use this parent account, and the existing currency-locked Intercompany Clearing Account remained intact. If you edit a transaction that originally posted to the existing currency-locked Intercompany Clearing Account, the GL Impact of that transaction affects that account.

After this feature is enabled, you can set the following OneWorld preferences at _Setup > Accounting > Accounting Preferences_ > General subtab:

-   **Intercompany Time** - Set to **Allow** (default) to permit time entries where the employee and customer have different subsidiaries. Set to **Disallow** to prohibit these transactions.
    
-   **Intercompany Expenses** - Set to **Allow** to permit expenses transactions where the employee and customer have different subsidiaries. Set to **Disallow** to prohibit these transactions. Set to **Allow and Auto Adjust** (default) to enable automated intercompany adjustments.
    

When time and expenses are entered, their impact on employee subsidiary accounts is recorded. For customers that have a subsidiary different from employees, create adjusting journal entries to reverse the impact on employee subsidiary accounts and register the impact on customer subsidiary accounts. You can manually adjust for intercompany time by creating intercompany journal entries. Adjustments for expense transactions can be created manually, or they can be automated by generating specialized transactions called intercompany adjustments.

For information about manually creating journal entries to adjust for intercompany transactions, see [Making Advanced Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4803443925.html).

For information about generating automated intercompany adjustments, see [Creating Intercompany Adjustments for Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1478200.html).

For a sample scenario, see [Example Intercompany Adjustment Scenario](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1478633.html).

If you plan to enable the Intercompany Time and Expense feature, consider the following:

-   **Expense Accounts and Categories** - You should set up expense categories linked to expense accounts that are available to all subsidiaries. In intercompany expense transactions, users can't save expense lines unless they contain expense categories available to both the employee subsidiary and customer subsidiary. See [Account Setup in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N275342.html) and [Creating an Expense Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415916.html).
    
-   **Service Items** - You should set up service items that are available to all subsidiaries. In intercompany time entries, users can't save lines unless they contain service items available to both the employee subsidiary and customer subsidiary. See [Associate Subsidiaries With Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276948.html).
    
-   **Classes, Departments, and Locations** - You must determine a strategy for handling classification segments on intercompany time and expenses.
    
    -   If you don't need to use classes, departments, and locations, you should omit them on intercompany time and expenses. You can set your accounting preferences to make this omission possible. Go to _Setup > Accounting > Preferences > Accounting Preferences_. On the General subtab, do one of the following:
        
        -   Disable the **Make Classes Mandatory**, **Make Departments Mandatory**, and **Make Locations Mandatory** options,
            
            or
            
        -   Enable the **Allow Empty Classifications on Journals** option.
            
    -   If you must use classifications on these transactions, you should set up global classifications that are available to all subsidiaries.
        
    -   If classifications are required for journals, set up global classifications available to all subsidiaries. Without global classifications, errors may occur for automated intercompany adjustments. These errors are caused by expense lines that include a class, department, or location that isn't available to the subsidiary associated with the selected customer.
        
    -   For more information about using classes, departments, and locations, see [Classifications in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N261411.html).
        

When you enable this feature, the system creates an intercompany clearing account. This clearing account prevents you from modifying the subsidiaries associated with all account types except Bank. For more information, see [Intercompany Clearing Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1477786.html).

Warning:

If the Intercompany Time and Expense feature isn't enabled, users can't enter time or expenses where the employee and customer have different subsidiaries.

### Related Topics

-   [Journal Entries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475513.html)
-   [System-Generated Journals for Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1528216938.html)
-   [Elimination Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475762.html)
-   [Making Advanced Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4803443925.html)
-   [Making Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475891.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
