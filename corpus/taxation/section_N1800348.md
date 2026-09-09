---
id: "section_N1800348"
type: "section"
title: "Setting Up Historical and Transitional Tax Periods Using a Fiscal Calendar"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Working with Tax Periods > Setting Up Historical and Transitional Tax Periods Using a Fiscal Calendar"
parent: "section_N1797157"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1800348.html"
anchors: ["bridgehead_N1800363"]
sha256: "9211e0dcf883cead972f2a8d6fd675b1d60500aac88ef8b0d60314f7e68a0988"
---

When you enable Multiple Calendars, existing accounting and tax periods of all your subsidiaries are assigned to the Standard Fiscal Calendar by default. Your existing fiscal year structure determines the start date and period rollup structure for the Standard Fiscal Calendar. For example, your organization previously used a calendar year, January through December, for reporting across all subsidiaries. When you enable Multiple Calendars, the default Standard Fiscal Calendar will have a start date of January.

You can create new fiscal calendars for your subsidiaries that use a tax year with a different start date, but before you do that, make sure that your historical periods are covered. After you set up historical periods, you must set up the rollup for the transitional period.

## Example {#bridgehead_N1800363}

| Subsidiary | Fiscal Calendar Name | Tax Fiscal Calendar Name |
| --- | --- | --- |
| **UK - Manchester Subsidiary** In this example, the subsidiary actually uses an accounting year that starts in April, and a tax year that starts in December. | **April Fiscal Calendar** When setting up historical and transitional accounting periods, use the same start date as the default Standard Fiscal Calendar (for example, January). After setting up historical and transitional accounting periods, change the calendar's start date to April, and then set up the future accounting periods. | **December Fiscal Calendar** When setting up historical and transitional tax periods, use the same start date as the default Standard Fiscal Calendar (for example, January). After setting up historical and transitional tax periods, change the calendar's start date to December, and then set up the future tax periods. |

The following table shows the historical, transitional, and future tax periods for the UK - Manchester Subsidiary example, and what you must do to set them up.

| UK - Manchester Subsidiary Example | Accounting Year | Tax Year |
| --- | --- | --- |
| 1 | **Historical Periods** In this example, before enabling Multiple Calendars, periods were set up for a fiscal year that starts in January. With Multiple Calendars enabled, the system assigns these periods to the default Standard Fiscal Calendar.
1.  Create new fiscal calendars:
    -   Example name: April Fiscal Calendar, but with the same start date as the Standard Fiscal Calendar (January).
    -   Example name: December Fiscal Calendar, but with the same start date as the Standard Fiscal Calendar (January).
2.  Assign the calendars to the subsidiary:
    -   In the Fiscal Calendar field of the Subsidiary record, select April Fiscal Calendar.
    -   In the Tax Fiscal Calendar field of the Subsidiary record, select December Fiscal Calendar.
3.  Set up accounting periods and tax periods for 2007 to 2011 using the Set Up Full Year option:
    -   In the Fiscal Calendar field of the Manage Accounting Periods page, select April Fiscal Calendar.
    -   In the Fiscal Calendar field of the Manage Tax Periods page, select December Fiscal Calendar.

 | FY 2007 (January 2007 - December 2007) | FY 2007 (January 2007 - December 2007) |
| FY 2008 | FY 2008 |
| FY 2009 | FY 2009 |
| FY 2010 | FY 2010 |
| FY 2011 | FY 2011 |
| 2 | **Transitional Period**

1.  Accounting periods - Set up the transitional year (January - March 2012) using the New Year Only option. Use the New Quarter Only and Base Period options to set up quarters and months.
2.  Tax periods - Set up the transitional year (January to November 2012) using the New Year Only option. Use the New Quarter Only and Base Period options to set up quarters and months.

 | Transitional year (January 2012 - March 2012) | Transitional year (January 2012 - November 2012) |
| 3 | **Future Periods**

1.  Accounting periods - Before setting up future years, edit the April Fiscal Calendar to change the start date to April, and then go to Manage Accounting Periods and set up future accounting periods using the Set Up Full Year option.
2.  Tax periods - Before setting up future years, edit the December Fiscal Calendar to change the start date to December, and then go to Manage Tax Periods and set up future tax periods using the Set Up Full Year option.

 | FY 2013 (April 2012- March 2013) | FY 2013 (December 2012 - November 2013) |
| FY 2014 | FY 2014 |
| FY 2015 | FY 2015 |
| FY 2016 | FY 2016 |
| FY 2017 | FY 2017 |
| FY 2018 | FY 2018 |
| FY 2019 | FY 2019 |

### Related Topics

-   [Working with Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797157.html)
-   [Tax Periods Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4454154841.html)
-   [Setting Up Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797599.html)
-   [Closing Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1798849.html)
-   [Editing and Deleting Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799174.html)
-   [Assigning a Tax Fiscal Calendar to a Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799451.html)
-   [Setting Up Tax Periods Using a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799689.html)
-   [Reporting by Tax Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1803024.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
