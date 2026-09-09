---
id: "section_N275342"
type: "section"
title: "Account Setup in OneWorld"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Set up NetSuite OneWorld > Account Setup in OneWorld"
parent: "section_N268052"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N275342.html"
anchors: []
sha256: "4eba44b83793457f0dfb96ddbff1a3d81e16c1a1d9723ecab417f92bfb54f711"
---

If you use NetSuite OneWorld, you can associate an account with one or more specific subsidiaries. This association limits availability of the account to the selected subsidiaries only.

Note:

Bank accounts and credit card accounts are restricted to one subsidiary. When you create a bank account or credit card account, you can select only one subsidiary for the account.

Each account is assigned the following exchange rate types:

-   **General Rate Type** - This rate type is used for the income statement, balance sheet, and other general purposes.
    
-   **Cash Flow Rate Type** - This rate type is used for the cash flow statement.
    

Go to _Setup > Accounting > Manage G/L > Chart of Accounts_. Click an **Edit** link next to account. Set up the account record as follows:

1.  In the **General Rate Type** field, select **Current**, **Average**, or **Historical** to determine which consolidated rate to use in all cases except cash flow.
    
    Tip:
    
    **Current** - Also referred to as 'ending rate,' the system uses this rate for all balance sheet accounts that do not use historical rates.
    
    **Average** - The system uses this rate for all income statement accounts.
    
    **Historical** - The system uses this rate for equity accounts and fixed asset accounts on the balance sheet.
    
2.  In the **Cash Flow Rate Type** field, select **Current**, **Average**, or **Historical** to determine which consolidated rate to use.
    
    For example, long-term assets use the **Historical** rate type on the cash flow statement. Balance sheet uses the **Current** rate type on the cash flow statement.
    
3.  If necessary, select one or more subsidiaries in the **Subsidiaries** field.
    
    -   If the root subsidiary is selected and the **Include Children** box is checked, then all subsidiaries can access the account.
        
    -   If one or more subsidiaries are selected, then the account can be selected for records and transactions associated with those subsidiaries.
        

For more details about rate types, see [Consolidated Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405625.html).

For more information about setting up accounts, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html).

Note:

If the **Intercompany Time and Expense** feature is enabled in your account, an intercompany clearing account is automatically created when there is an associated transaction. For more information, see [Intercompany Clearing Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1477786.html).

### Related Topics

-   [Payroll Setup in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N275739.html)
-   [Inventory Setup in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N275901.html)
-   [Multiple Vendors Setup in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276076.html)
-   [Logos in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276203.html)
-   [Set up NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268052.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
