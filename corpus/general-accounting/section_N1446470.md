---
id: "section_N1446470"
type: "section"
title: "Setting Up Single Accounting Periods"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Accounting Period Setup > Setting Up Single Accounting Periods"
parent: "section_N1445585"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446470.html"
anchors: ["procedure_N1446531", "procedure_N1446593", "procedure_N1446669"]
sha256: "0dc994dce778a9885df03f8cc02910011dc35b1bc3abfa1ebd7c71990454b052"
---

The best practice is to use the Set Up Full Year option to generate all the periods for a year, but you can manually set up your periods, if you prefer. If you manually set up periods you must set up a year period first, which is the highest level period in the accounting period rollup. Then set up the subperiods that belong to that fiscal year. Typically a fiscal year consists of a year, quarters, and months. You can, if needed, set up base periods with other date ranges such as weeks, but it'sn't recommended.

Important:

Each day must belong to an accounting period to ensure accuracy in reporting.

Use caution when setting up individual accounting periods to avoid creating incomplete or incorrect period rollups. In general, it's always best to set up all subperiods for a year.

Important:

You must set up all subperiods for a year for reports to display results by period. Remember to review all rollups on the Manage Accounting Page to verify each fiscal year is complete and correct.

Remember that an adjustment period is a base period. All base periods must roll up to a parent period across all fiscal calendars. If you have an adjustment period without a parent in one fiscal calendar, it's an orphan period. When you run your financial reports in that fiscal calendar, all adjustment journal entries in that adjustment period are not included in your report.

You must have at least **Edit** level of the **Manage Accounting Periods** permission to set up accounting periods.

#### To set up periods one at a time:

1.  Go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.
    
2.  Select the **New Year Only**, **New Quarter Only**, or **Base Period** option.
    

#### To set up a new year: {#procedure_N1446531}

1.  On the Manage Accounting Periods page, click **New Year Only**.
    
2.  In the **Period Name** field, enter a short, descriptive name such as **FY 2014.**
    
    You can enter up to 40 characters, but because these names appear in lists on all transaction forms it's better to enter a short name.
    
3.  In **Start Date**, enter or pick the first date for the fiscal year such as **1/1/2014**.
    
4.  In **End Date**, enter or select the last date for the year such as **12/31/2014**.
    
5.  Click **Save**.
    

#### To set up a new quarter: {#procedure_N1446593}

1.  On the Manage Accounting Periods page, click **New Quarter Only**.
    
2.  Enter a name in the **Period Name** field such as **Q1 2014.**
    
3.  In the **Start Date** field, enter or pick the first date of the period such as **1/1/2014.**
    
4.  In the **End Date** field, enter or pick the last date of the period such as **3/31/2014.**
    
5.  In **Sub-period of**, select the parent period such as **FY 2014**.
    
6.  Click **Save**.
    
7.  Continue setting up the remaining periods for the quarter.
    

#### To set up a new period: {#procedure_N1446669}

1.  On the Manage Accounting Periods page, click **Base Period**.
    
2.  Enter a name in the **Period Name** field such as **Jan 2014.**
    
3.  In the **Start Date** field, enter or pick the first date of the period such as **1/1/2014.**
    
4.  In the **End Date** field, enter or pick the last date of the period such as **1/31/2014.**
    
5.  In **Sub-period of**, select the parent period such as **Q1 2014**.
    
6.  Check **Period is Adjustment** if this is an adjustment period.
    
    You can set up a standalone adjustment period or an adjustment period that overlaps the dates of a base period.
    
7.  Check **Allow Non-G/L Changes** to allow users with the **Allow Non G/L Changes** permission to make non-posting changes to posting transactions after the period has been locked to transactions.
    
    Note:
    
    If you allow non-general ledger changes to posting transactions after the period has been locked to transactions, these changes may trigger inventory costing recalculations even if the change made doesn't directly impact the general ledger. For details, please read Limiting Inventory Costing Triggers under [Inventory Costing Recalculations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197365.html).
    
8.  Click **Save**.
    
9.  Continue setting up the remaining base periods.
    

To edit a period, click the period name in the list of periods on the Manage Accounting Periods page. See [Editing an Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446881.html).

### Related Topics

-   [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html)
-   [Manage Accounting Periods Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445839.html)
-   [Setting Up Accounting Periods for a Year](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446183.html)
-   [Editing an Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446881.html)
-   [Accounting Period Deletion Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1448709.html)
-   [Viewing the Status of Accounting Period Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449023.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
