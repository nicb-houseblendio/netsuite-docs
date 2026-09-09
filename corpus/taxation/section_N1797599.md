---
id: "section_N1797599"
type: "section"
title: "Setting Up Tax Periods"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Working with Tax Periods > Setting Up Tax Periods"
parent: "section_N1797157"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797599.html"
anchors: ["procedure_N1797657", "procedure_N1797777", "procedure_N1797859", "procedure_N1798570"]
sha256: "1e16f8c2a7f7e74d7c453663a0e77a273fd2912a8c64d0b4209f63833e1858d3"
---

Setting up tax periods requires the Manage Tax Reporting Periods permission.

When setting up tax periods, the best practice is to use months for posting tax, even if you intend to run only quarterly or annual reports. Go to the Manage Tax Periods page, select the Set Up Full Year option, and then choose the Calendar Months format.

You can also create periods individually using these options: New Year Only, New Quarter Only, and Base Period. However, setting up tax periods individually can create incomplete or incorrect period rollups if you're not careful. Be sure to review all rollups on the Manage Tax Periods Page to verify that each tax year is complete and correct.

Note:

If you set up quarters without months, you'll be able to run only quarterly tax reports. If you set up years without children, you'll be able to run only annual tax reports. Consequently, you won't be able to run monthly tax reports in the event of internal or external needs such as tax audits, unless you have tax periods set up as months.

Important:

If you're currently using quarters or years as your lowest tier of tax periods instead of months, or if you have set up periods in mixed mode, be aware that as of NetSuite 2013.2, a new **Is Posting** box has been added to the tax period record for quarters and years. you'll be required to define the quarter or year as either posting or non-posting. If there is a quarter or year without children (months or base periods), and you want to use it for tax reporting, then you must make sure that the **Is Posting** box is checked on the tax period record. For more information, see [Tax Period Posting Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3745446316.html).

On the Manage Tax Periods page, you can identify posting periods by their status icons. Non-posting periods don't have status icons.

Month periods are always posting. To define a quarter or year as posting, check the **Is Posting** box on the tax period record. Note that you can't check the **Is Posting** box for quarters and years that have children. Posting periods can't have children.

Note:

The following steps are for setting up tax periods without the Multiple Calendars feature enabled. If you're using the Multiple Calendars feature, see [Setting Up Tax Periods Using a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799689.html).

Follow these steps to set up a full year that has sub-periods.

#### To set up tax periods for a full year: {#procedure_N1797657}

1.  Go to Setup > Accounting > Taxes > Manage Tax Periods.
    
2.  Click **Set Up Full Year**.
    
3.  In the **First Fiscal Month** field, select the first month in your company's fiscal year.
    
4.  In the **Fiscal Year End** field, enter the year for which you're setting up tax periods.
    
5.  In the **Period Format** field, select one of the following to divide the year into:
    
    -   **Quarters** - three-month long sub-periods. These quarters have the Is Posting box checked by default.
        
    -   **Calendar Months** - twelve sub-periods.
        
    -   **4 Weeks** - thirteen four-week long sub-periods
        
    -   **4-4-5 Weeks** - four quarters in which the weeks follow this pattern, instead of the actual calendar dates.
        
6.  Click **Save**.
    

Follow these steps to set up a year.

#### To set up a tax reporting year: {#procedure_N1797777}

1.  Go to Setup > Accounting > Taxes > Manage Tax Periods.
    
2.  Click **New Year Only**.
    
3.  In the **Period Name** field, enter a name for this year.
    
4.  Enter or select a start date for this year.
    
5.  Enter or select an end date for this year.
    
6.  Check the **Is Posting** box to enable NetSuite to post tax to this year period. If the **Is Posting** box isn't checked, then you must set up either quarters or months as sub-periods of this year.
    
7.  Click **Save**.
    

Follow these steps to set up a quarter.

#### To set up a tax reporting quarter: {#procedure_N1797859}

1.  Go to Setup > Accounting > Taxes > Manage Tax Periods.
    
2.  Click **New Quarter Only**.
    
3.  In the **Period Name** field, enter a name for this quarter.
    
4.  Enter or select a start date for this quarter.
    
5.  Enter or select an end date for this quarter.
    
6.  Check the **Is Posting** box to enable NetSuite to post tax to this quarter period. If the **Is Posting** box isn't checked, then you must set up months as sub-periods of this quarter.
    
7.  In the **Sub-period of** field, select the year that this quarter belongs to. The parent period must be already set up. Otherwise, it won't appear in the dropdown list. Note that you can add sub-periods to a non-posting year only.
    
8.  Click **Save**.
    

Follow these steps to set up a base tax period.

#### To set up a base tax period: {#procedure_N1798570}

1.  Go to Setup > Accounting > Taxes > Manage Tax Periods.
    
2.  Click **Base Period**.
    
3.  In the **Period Name** field, enter a name for this base period.
    
4.  Enter or select a start date for this base period.
    
5.  Enter or select an end date for this period.
    
6.  In the **Sub-period of** field, select the parent period that this base period belongs to. The parent period must be already set up. Otherwise, it won't appear in the dropdown list. Sub-periods can be added to a non-posting parent period only.
    
7.  Click **Save**.
    

### Related Topics

-   [Working with Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797157.html)
-   [Tax Periods Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4454154841.html)
-   [Closing Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1798849.html)
-   [Editing and Deleting Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799174.html)
-   [Assigning a Tax Fiscal Calendar to a Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799451.html)
-   [Setting Up Tax Periods Using a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799689.html)
-   [Setting Up Historical and Transitional Tax Periods Using a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1800348.html)
-   [Reporting by Tax Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1803024.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
