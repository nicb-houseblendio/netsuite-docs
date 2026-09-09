---
id: "section_N1799689"
type: "section"
title: "Setting Up Tax Periods Using a Fiscal Calendar"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Working with Tax Periods > Setting Up Tax Periods Using a Fiscal Calendar"
parent: "section_N1797157"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799689.html"
anchors: ["bridgehead_N1799790", "procedure_N1799803", "bridgehead_N1799877", "procedure_N1799892", "procedure_N1799980", "procedure_N1800084"]
sha256: "c96ea88e419c1d35b3f839c3cacad2ecab0c60c4ba031cc00c8c7117635942c2"
---

You can set up tax periods using a fiscal calendar if you have the Multiple Calendars feature enabled.

Several subsidiaries can share one fiscal calendar. For more information, see [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html).

Warning:

After enabling Multiple Calendars, this feature can only be disabled if you haven't yet assigned a new fiscal calendar to a subsidiary. If you have already created a new fiscal calendar and assigned it to a subsidiary, you can no longer disable Multiple Calendars.

If the Multiple Calendars feature is enabled in your account, you can do the following:

-   Set up different fiscal calendar definitions on the same subsidiary for accounting and tax calendars
    
-   Define a tax year for a subsidiary, independently of other subsidiaries.
    

The Multiple Calendars feature can be enabled in OneWorld accounts only. A fiscal calendar determines the start date for an accounting year or tax year, and rolls up the accounting periods and tax periods.

**Example:**

The following table shows how subsidiaries can be set up in a OneWorld account with Multiple Calendars:

| Subsidiary | Fiscal Calendar (for accounting year) | Tax Fiscal Calendar (for tax year) |
| --- | --- | --- |
| UK - London subsidiary | April Fiscal Calendar | July Fiscal Calendar |
| UK - Manchester subsidiary | April Fiscal Calendar | December Fiscal Calendar |
| Germany - Berlin subsidiary | January Fiscal Calendar | January Fiscal Calendar |
| Ireland - Dublin subsidiary | January Fiscal Calendar | March Fiscal Calendar |

On the Manage Tax Periods page, you select a fiscal calendar to view tax periods that have been set up for that fiscal calendar. Periods shown as Unassigned are tax periods that haven't been assigned to the selected fiscal calendar.

To set up a full year with calendar months and quarters. See [Setting Up a Full Tax Year for a Fiscal Calendar](#bridgehead_N1799790). To set up individual years, quarters, and periods, each with a start date and an end date that you specify, see [Setting Up Tax Periods Individually for a Fiscal Calendar](#bridgehead_N1799877).

Important:

If you enable Multiple Calendars in an account that already contains transactional data, you must first set up your historical and transitional periods using a fiscal calendar before you set up future tax periods. See [Setting Up Historical and Transitional Tax Periods Using a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1800348.html).

Make sure your Subsidiary records are set up with the correct accounting and tax fiscal calendars. You can open a fiscal calendar record to see the subsidiaries that the calendar has been assigned to. For more information, read [Assigning a Tax Fiscal Calendar to a Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799451.html).

## Setting Up a Full Tax Year for a Fiscal Calendar {#bridgehead_N1799790}

When setting up tax periods, the best practice is to use months for posting tax, even if you only intend to run quarterly or annual reports. Go to the Manage Tax Periods page, select the Set Up Full Year option, and then choose the Calendar Months format.

#### To set up a full tax reporting year using a fiscal calendar: {#procedure_N1799803}

1.  Go to Setup > Accounting > Taxes > Manage Tax Periods (Administrator).
    
2.  Select a fiscal calendar.
    
3.  Click **Set Up Full Year**.
    
4.  On the New Tax Reporting Periods for Full Year page, make sure that the values in the **Fiscal Calendar** field and **First Fiscal Month** field are correct.
    
5.  In the **Fiscal Year End** field, enter or accept the fiscal year you want to generate tax periods for. For example, to set up tax periods for 2014, enter **2014** in the **Fiscal Year End** field.
    
6.  In the **Period Format** field, select one of the following to divide the year into:
    
    -   **Quarters** - three-month long sub-periods. These quarters have the Is Posting box checked by default.
        
    -   **Calendar Months** - twelve sub-periods.
        
    -   **4 Weeks** - thirteen four-week long sub-periods
        
    -   **4-4-5 Weeks** - four quarters in which the weeks follow this pattern, instead of the actual calendar dates.
        
7.  In the **Year in Period Name** field, select the starting or ending year to include in the period name.
    
8.  Click **Save**. On the Manage Tax Periods page, the full year that you have created includes quarters and months.
    

## Setting Up Tax Periods Individually for a Fiscal Calendar {#bridgehead_N1799877}

You can create periods individually using these options: New Year Only, New Quarter Only, and Base Period. However, setting up tax periods individually can create incomplete or incorrect period rollups if you're not careful. Be sure to review all rollups on the Manage Tax Periods Page to verify that each tax year is complete and correct.

Note:

If you set up quarters without months, you'll be able to run only quarterly tax reports. If you set up years without children, you'll be able to run only annual tax reports. Consequently, you won't be able to run monthly tax reports in the event of internal or external needs such as tax audits, unless you have tax periods set up as months. The best practice is to use months for posting tax, even if you intend to run only quarterly or annual reports. Go to the Manage Tax Periods page, select the Set Up Full Year option, and then choose the Calendar Months format.

#### To set up a new tax reporting year using a fiscal calendar: {#procedure_N1799892}

1.  Go to Setup > Accounting > Taxes > Manage Tax Periods (Administrator).
    
2.  Select a fiscal calendar.
    
3.  Click **New Year Only**.
    
4.  In the **Period Name** field, enter a name for this tax year. For example, FY 2014.
    
5.  Enter or select a start date for this tax year.
    
6.  Enter or select an end date for this tax year.
    
7.  Make sure that the value displayed in the **Fiscal Calendar** field is correct.
    
8.  Click **Save**. On the Manage Tax Periods page, note that the tax year that you have just created doesn't include the sub-periods such as quarters or months.
    

#### To set up a new tax reporting quarter using a fiscal calendar: {#procedure_N1799980}

1.  Go to Setup > Accounting > Taxes > Manage Tax Periods (Administrator).
    
2.  Select a fiscal calendar.
    
3.  Click **New Quarter Only**.
    
4.  In the **Period Name** field, enter a name for this quarter. For example, **Q1 2014**.
    
5.  Enter or select a start date for this quarter.
    
6.  Enter or select an end date for this quarter.
    
7.  Check the **Is Posting** box to enable NetSuite to post tax to this quarter period. If the **Is Posting** box isn't checked, then you must set up months as sub-periods of this quarter.
    
8.  Make sure that the fiscal calendar displayed is correct.
    
9.  In the **Sub-period of** field, select the tax reporting year that this quarter belongs to. For example, **FY 2014**. The parent period must be already set up. Otherwise, it won't be available in the dropdown list.
    
10.  Click **Save**.
     

#### To set up a new tax reporting period using a fiscal calendar: {#procedure_N1800084}

1.  Go to Setup > Accounting > Taxes > Manage Tax Periods (Administrator).
    
2.  Select a fiscal calendar.
    
3.  Click **Base Period**.
    
4.  In the **Period Name** field, enter a name for this base period.
    
5.  Enter or select a start date for this period.
    
6.  Enter or select an end date for this period.
    
7.  If the period is for the Standard Fiscal Calendar, select a parent period in **Sub-period of** column of the Standard Fiscal Calendar. If this period is for a different fiscal calendar, then add a new row and select the fiscal calendar to use for this tax reporting period.
    
8.  Click **Save**.
    

### Related Topics

-   [Working with Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797157.html)
-   [Tax Periods Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4454154841.html)
-   [Setting Up Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797599.html)
-   [Closing Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1798849.html)
-   [Editing and Deleting Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799174.html)
-   [Assigning a Tax Fiscal Calendar to a Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799451.html)
-   [Setting Up Historical and Transitional Tax Periods Using a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1800348.html)
-   [Reporting by Tax Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1803024.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
