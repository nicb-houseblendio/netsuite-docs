---
id: "section_N1449211"
type: "section"
title: "Fiscal Calendars"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Fiscal Calendars"
parent: "chapter_N1445226"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html"
anchors: ["svg_1", "svg_1Invisible_Layer", "svg_1Layer_1", "svg_1Bendy_Thin", "svg_1Node", "bridgehead_N1449277", "bridgehead_N1449326"]
sha256: "f6519cc1da83c672a7f0c563cc85198596d8e191919f786fdd31ce4370dc085b"
---

Fiscal calendars apply to accounting periods and tax periods. To use fiscal calendars, the Multiple Calendars feature must be enabled. This feature is available only for NetSuite OneWorld and by default, isn't enabled. The Multiple Calendars feature also determines the rollup structure for tax periods. For more information, see [Setting Up Tax Periods Using a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799689.html).

If you create different accounting period rollups for subsidiaries, the accounting period rollup is defined within the context of fiscal calendar. Each accounting period rollup groups transaction data from a common set of base periods into fiscal years. This enables you to report transaction activity using different fiscal year start and end dates, as needed, to meet statutory and organizational reporting requirements.

A fiscal calendar determines the start date for a fiscal year and rolls up the accounting periods to build a fiscal year. The lowest level accounting periods that make up a fiscal year are shared across all fiscal calendars. Aggregate periods within a fiscal year, such as quarters and years, are unique to a fiscal calendar. Base period names are shared across all fiscal calendars, and base period names in a fiscal calendar must be unique.

You then assign a fiscal calendar to a subsidiary to determine how to roll up accounting periods for reporting activity in that subsidiary. A subsidiary can have only one fiscal calendar in effect at a time. You can change the fiscal calendar assigned to a subsidiary as needed.

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                                                                                                                         

The diagram above shows a subsidiary hierarchy with three fiscal calendars. The Standard Fiscal Calendar starts January 1 and is assigned to the U.S., APAC, and Japan subsidiaries. The accounting period rollup for these subsidiaries organizes fiscal years to start January 1 and end December 31. The July Fiscal Calendar is assigned to the U.K. subsidiary to create fiscal years beginning July 1 and ending June 30. The India subsidiary fiscal year runs April 1 through March 31, so the April Fiscal Calendar is assigned to the India subsidiary.

## Default Fiscal Calendar {#bridgehead_N1449277}

NetSuite creates a default Standard Fiscal Calendar when you enable the Multiple Calendars feature. Your existing fiscal year structure determines the start date and period rollup structure for the Standard Fiscal Calendar.

Note:

For new implementations or if you enable the Multiple Calendars feature before creating any accounting periods, the Standard Fiscal Calendar doesn't have a start date or accounting period rollup structure until you set up accounting periods.

The Standard Fiscal Calendar is assigned to all existing subsidiaries and to any new subsidiaries you create. It remains the default fiscal calendar until you designate a different calendar as the default. When you change the default fiscal calendar, only subsidiaries created after that point are assigned the new default fiscal calendar. Existing subsidiaries continue to use the Standard Fiscal Calendar. The fiscal calendar for subsidiaries previously assigned doesn't change.

Note:

Rename the Standard Fiscal Calendar when it's no longer the default fiscal calendar.

## Accounting Period Rollups {#bridgehead_N1449326}

An accounting period rollup provides the structure to organize the base accounting periods for reporting. The base accounting period is typically a month. Month periods can be calendar months, 4 week months, or months of 4-4-5 weeks. The **Set Up Full Year** function creates fiscal years based on calendar months. If you want to use periods other than months, you must use manually set up accounting periods and fiscal years using **New Year Only**, **New Quarter Only**, and **Base Period** buttons. Best practice is to use Set Up Full Year to generate your accounting periods.

On the Manage Accounting Period page, select a fiscal calendar to display accounting periods using the period rollup for that calendar. The fiscal calendar determines the rollup hierarchy for the accounting periods. You must set up a fiscal year for the Manage Accounting Periods page to display a fiscal period rollup.

Existing base accounting periods that are not included in the accounting period rollups for a fiscal calendar display on the Manage Accounting Periods page under **Unassigned**. For complete consolidated reporting, you must define a complete rollup hierarchy for a base period by assigning its sub-period of relationship for each fiscal calendar

To add unassigned periods to accounting rollups:

1.  On the Manage Accounting Periods page, select a fiscal calendar and check for unassigned periods.
    
2.  Click an unassigned period to edit.
    
3.  On the Edit Accounting Period page, assign the period to a sub-period for each fiscal calendar that exists.
    
4.  Click **Save**.
    

For more information about fiscal calendars and multiple calendars, see the following topics:

-   [Enabling Multiple Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449485.html)
    
-   [Creating a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449559.html)
    
-   [Setting Up Accounting Periods for a Full Year for Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449871.html)
    
-   [Setting Up Single Accounting Periods for Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449971.html)
    
-   [Adjustment Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450241.html)
    
-   [Restriction and Automation Rules Governing Accounting Period Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450765.html)
    
-   [Multiple Calendars with Other NetSuite Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450943.html)
    
-   [Searching Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4193640975.html)
    

### Related Topics

-   [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html)
-   [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html)
-   [GL Audit Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3735573963.html)
-   [Rules for Future Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451349.html)
-   [Accounting Period Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html)
-   [Year-End Closing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457773.html)
-   [Reporting by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1458661.html)
-   [Searching by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1459178.html)
-   [Locking Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N560870.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
