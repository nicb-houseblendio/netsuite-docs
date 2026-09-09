---
id: "section_N1450765"
type: "section"
title: "Restriction and Automation Rules Governing Accounting Period Changes"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Fiscal Calendars > Restriction and Automation Rules Governing Accounting Period Changes"
parent: "section_N1449211"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450765.html"
anchors: []
sha256: "5dcd53f68e0f2dc0bdabc30028bbc855bee6a9d971431930516338a444313b74"
---

When you add, delete, or modify accounting periods, NetSuite attempts to adjust the rollup hierarchy across all fiscal calendars and prevent creating standalone periods. Restriction and automation rules run in the background to simplify managing accounting periods though preserving the integrity of the accounting period structure.

Modifying an accounting period is generally prohibited if doing so removes an existing parent/child without reestablishing a new one.

When you create, update, or delete base or aggregate periods, NetSuite automatically attempts to find the logical parent for a period in the accounting period rollup and across all existing fiscal calendars to prevent creating a standalone period.

-   If one or more aggregate periods exist for the date range, NetSuite assigns the new period to the lowest level aggregate period available, unless you specify a parent.
    
-   You can make changes in a hierarchy such deleting a period, if a suitable parent exists for all periods in the hierarchy. If no logical parent exists, you can't make the change.
    

you're restricted from making a change if the change disrupts the accounting period rollup. The general rules that affect rollups are:

-   A base period must have at least one aggregate level period or parent
    
-   Aggregate periods are the parents for subperiods
    
-   A base period has multiple parents, one in each fiscal calendar context
    
-   A subperiod can be a base period or another aggregate period
    
-   All base periods must have at least one parent
    
-   Parent and child periods roll up into fiscal years for each fiscal calendar
    

### Related Topics

-   [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html)
-   [Enabling Multiple Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449485.html)
-   [Creating a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449559.html)
-   [Setting Up Accounting Periods for a Full Year for Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449871.html)
-   [Setting Up Single Accounting Periods for Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449971.html)
-   [Adjustment Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450241.html)
-   [Multiple Calendars with Other NetSuite Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450943.html)
-   [Searching Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4193640975.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
