---
id: "section_N1449971"
type: "section"
title: "Setting Up Single Accounting Periods for Subsidiaries"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Fiscal Calendars > Setting Up Single Accounting Periods for Subsidiaries"
parent: "section_N1449211"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449971.html"
anchors: ["procedure_N1450013", "procedure_N1450072", "procedure_N1450138"]
sha256: "c8b91333e4a6d43e7b09318e33faaca1ce6f9d70f1e076c1141c9fa64f6e84bf"
---

Setting up accounting periods individually can create incomplete or incorrect period rollups. Be sure to review the accounting period rollups on the Manage Accounting page and verify each fiscal year is complete and correct. Do this for each fiscal calendar.

Important:

Each day must belong to an accounting period to ensure accuracy in reporting.

To set up accounting periods individually for a fiscal year:

-   first set up a year
    
-   set up quarters if desired
    
-   set up base periods
    

#### To set up a new fiscal year: {#procedure_N1450013}

1.  Go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.
    
2.  Select the fiscal calendar.
    
3.  Click **New Year Only**.
    
4.  Enter **Period Name**.
    
5.  Enter a start date and end date for the period.
    
6.  Verify the fiscal calendar selected is correct.
    
7.  Click **Save**.
    

#### To set up a new quarter: {#procedure_N1450072}

1.  Go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.
    
2.  Select the fiscal calendar.
    
3.  Click **New Quarter Only**.
    
4.  Enter the **Period Name**.
    
5.  Enter a start date and end date for the quarter.
    
6.  Verify the fiscal calendar selected is correct.
    
7.  For **Sub-period of**, select the fiscal year to which this quarter belongs.
    
8.  Click **Save**.
    

#### To set up a new period: {#procedure_N1450138}

1.  Go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.
    
2.  Select the fiscal calendar.
    
3.  Click **Base Period** and then enter the **Period Name**.
    
4.  Enter a **Start Date** and **End Date** for the period.
    
    The **Allow Non-G/L Changes** box is read-only unless the period is locked or closed.
    
5.  Verify the fiscal calendar is correct.
    
6.  Check **Period is Adjustment** to mark this period only for adjustment journal entries.
    
    The date range for adjustment period must overlap an existing accounting period.
    
7.  In the **Fiscal Calendar** column, if the period is for the **Standard Fiscal Calendar**, in **Sub-period of** column, select a period to be its parent period.
    
    You can also add a new row and select the fiscal calendar to use for the accounting rollup and the parent period. For example, when creating a period for June 2015, you can select Q2 2015 for the Sub-period of field.
    
8.  Click **Save**.
    

### Related Topics

-   [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html)
-   [Enabling Multiple Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449485.html)
-   [Creating a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449559.html)
-   [Setting Up Accounting Periods for a Full Year for Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449871.html)
-   [Adjustment Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450241.html)
-   [Restriction and Automation Rules Governing Accounting Period Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450765.html)
-   [Multiple Calendars with Other NetSuite Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450943.html)
-   [Searching Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4193640975.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
