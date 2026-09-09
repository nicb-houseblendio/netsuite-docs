---
id: "bridgehead_N1449790"
type: "bridgehead"
title: "Moving Subsidiaries to a New Fiscal Year"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Fiscal Calendars > Creating a Fiscal Calendar > Moving Subsidiaries to a New Fiscal Year"
parent: "section_N1449559"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1449790.html"
anchors: []
sha256: "c988bffadbf06beab268364279b5b6bc50f9380ffd5e02d907d072113a5ca474"
---

When you add new fiscal calendars, you can introduce a gap in reporting coverage in the accounting rollup for the subsidiaries associated with a new fiscal calendar. For example, your organization previously used a calendar year, January through December, for reporting across all subsidiaries. With the **Multiple Calendars** feature enabled, you add a fiscal calendar, FC April, that runs April through March and assign it to Subsidiary B. The first fiscal year for this subsidiary begins April 1, which leaves a reporting gap for January, February, and March of that year.

To provide full reporting coverage:

1.  Create a new fiscal calendar and set the start date to be the same as Standard Fiscal Calendar. Assign subsidiaries to the new calendar.
    
2.  Use **Set Up Full Year** to generate accounting period rollups for the new fiscal calendar to provide reporting coverage for all historical, closed, or existing fiscal years.
    
3.  Set up the accounting period rollup for the short year or transition period that falls before the first day the new fiscal calendar starts. Set up the base periods and rollup hierarchy manually using the **New Year Only**, **New Quarter Only**, and **Base Period** buttons.
    
4.  Change the **Start Date** for the new fiscal calendar to the date you want to use for the calendar in the future.
    
5.  Use **Set Up Full Year** and generate accounting period rollups for future fiscal years.
    

For the above example, add fiscal calendar, FC April, with a start date of January 1. Generate fiscal years for FC April for all periods before April of the first year you want to use FC April. Then change the start date of FC April to April 1 and use Set Up Full Year to generate accounting period rollups using the new calendar.

### Related Topics

-   [Creating a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449559.html)
-   [Editing a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1449653.html)
-   [Assigning Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1449741.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
