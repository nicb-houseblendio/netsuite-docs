---
id: "section_N1450943"
type: "section"
title: "Multiple Calendars with Other NetSuite Features"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Fiscal Calendars > Multiple Calendars with Other NetSuite Features"
parent: "section_N1449211"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450943.html"
anchors: ["bridgehead_N1451001"]
sha256: "9fb439c67ff2122c8cddf99ad14278672896b5cae0697be3bf395e0242ac06fd"
---

When you enable the Multiple Calendars feature, you can use subsidiary-specific calendars with the following features in NetSuite. Assigning a fiscal calendar to a subsidiary determines the calendar used to set up and manage the following:

-   Budgets
    
-   Forecasts
    
-   Quotas
    
-   Commission
    

With Multiple Calendars enabled, the fiscal calendar assigned to a subsidiary determines when the calendar begins for these features. The Standard Fiscal Calendar is assigned to all subsidiaries when you enable Multiple Calendars. As you create new calendars and assign them to subsidiaries, the monthly organization for following features changes as noted in the following subtopics. These changes apply only for NetSuite OneWorld with the Multiple Calendars feature enabled.

Note:

NetSuite automatically adjusts the quotas of sales representatives in subsidiaries and the parent company when changes are made to the respective fiscal calendar.

Without Multiple Calendars enabled, when you set up a budget or quotas, the calendars of months are based on the First Fiscal Month identified in Company Settings. See [Configuring Company Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N240902.html).

## Using Quotas Per Subsidiary, Multiple Calendars with Quotas {#bridgehead_N1451001}

When you assign a calendar other than the Standard Fiscal Calendar to a subsidiary, NetSuite modifies the organization (monthly quotas and years) of all existing quotas in that subsidiary to begin with the first fiscal month of that calendar. For example, before enabling Multiple Calendars, your fiscal year was based on a calendar year, January to December. You set up quotas for three years - 2012, 2013, and 2014. All quotas were set up for the year periods, January through December. You then enable the Multiple Calendars feature and create a new fiscal calendar that runs April 1 through March 31. You assign the new fiscal calendar to the India Subsidiary. NetSuite adjusts existing quotas for sales reps in the India Subsidiary to be grouped by years that run for the period April to March. It creates 4 years of quotas as follows:

| Year | Start Month | End Month | Months |
| --- | --- | --- | --- |
| 2011 - 2012 | January 2012 | March 2012 | January, February, March (3 months) |
| 2012 - 2013 | April 2012 | March 2013 | April - March |
| 2013 - 2014 | April 2013 | March 2014 | April - March |
| 2014 - 2015 | April 2014 | December 2014 | April, May, June, July, August, September, October, November, December (9 months) |

The first and last years are not full years because only existing quota months can be reorganized for the new fiscal calendar. New months are not created automatically.

To complete the quotas for Year 2014-2015, edit the quota records and add quota amounts for January, February, and March 2015.

### Related Topics

-   [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html)
-   [Enabling Multiple Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449485.html)
-   [Creating a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449559.html)
-   [Setting Up Accounting Periods for a Full Year for Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449871.html)
-   [Setting Up Single Accounting Periods for Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449971.html)
-   [Adjustment Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450241.html)
-   [Restriction and Automation Rules Governing Accounting Period Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450765.html)
-   [Searching Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4193640975.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
