---
id: "section_N1449871"
type: "section"
title: "Setting Up Accounting Periods for a Full Year for Subsidiaries"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Fiscal Calendars > Setting Up Accounting Periods for a Full Year for Subsidiaries"
parent: "section_N1449211"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449871.html"
anchors: ["procedure_N1449895"]
sha256: "6ea1e9d0ec20736e3be743142fc921f2d1c81a0c1e693670adc4da091924a0a2"
---

For NetSuite OneWorld with the **Multiple Calendars** feature enabled, best practice is to use **Set Up Full Year** to generate accounting periods and its associated accounting period rollup.

Important:

Each day must belong to an accounting period to ensure accuracy in reporting.

When you set up a new year, the base accounting periods may already exist if they were previously generated for a rollup for another fiscal calendar. In this case, NetSuite generates the fiscal year and quarters for the new calendar, but only generates new months if they were not created for another fiscal calendar. For example, you select a fiscal calendar FC India on the Manage Accounting Periods page and click Set Up Full Year to set up FY 2015. FY 2015 spans April 2014 through March 2015. Base periods for the months April through December 2014 have already been created using the Standard Fiscal Calendar. NetSuite creates new base periods only for January 2015, February 2015, and March 2015 and assigns the existing base periods for 2014 to FY 2015. These new periods are Unassigned periods on the Manage Accounting Periods page for the Standard Fiscal Calendar.

In addition, you can't set up overlapping fiscal years that have different base period formats such as 4 week months and calendar months, even if the years belong to different fiscal calendars.

#### To set up periods for a full year: {#procedure_N1449895}

1.  Go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.
    
2.  Select a fiscal calendar.
    
3.  Click **Set Up Full Year**.
    
4.  On the Accounting Periods for a Full Year page, verify that the Fiscal Calendar is correct.
    
5.  The first fiscal month for the fiscal calendar displays, defaulting from the fiscal calendar selected.
    
6.  Select the format you want to use for your accounting periods: **Calendar Months**, **4 Weeks**, or **4-4-5 Weeks**.
    
7.  In the **Year in Period Name** field, select the starting or ending year to include in the period name.
    
8.  Optionally, check the **One-Day Year-End Adj. Period** box to include an adjustment period at the end of this fiscal year.
    
    The adjustment period always overlaps the last day of the month. For example if the last month in a fiscal year is December and the year includes an adjustment period, the date span for December period is 12/1 through 12/31. The adjustment period is one day: 12/31.
    
9.  Click **Save**.
    

### Related Topics

-   [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html)
-   [Enabling Multiple Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449485.html)
-   [Creating a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449559.html)
-   [Setting Up Single Accounting Periods for Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449971.html)
-   [Adjustment Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450241.html)
-   [Restriction and Automation Rules Governing Accounting Period Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450765.html)
-   [Multiple Calendars with Other NetSuite Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450943.html)
-   [Searching Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4193640975.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
