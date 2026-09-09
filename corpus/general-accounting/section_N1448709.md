---
id: "section_N1448709"
type: "section"
title: "Accounting Period Deletion Restrictions"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Accounting Period Setup > Accounting Period Deletion Restrictions"
parent: "section_N1445585"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1448709.html"
anchors: []
sha256: "e8afc6315b70643eba3f0c7421a6afa33f2a003361250de2cf630d5cde880a51"
---

You can delete an accounting period, depending on the type of period and its relationship in the accounting period hierarchy. If you use fiscal calendars, additional restrictions apply. The general rules for deleting a period are shown in the following table.

| Period Type | Restriction | Result |
| --- | --- | --- |
| Base Period | Allowed only if the period has no transactions | Deletes the period. With Multiple Calendars enabled, deletes the period from all fiscal calendars. |
| Quarter | Allowed | With Multiple Calendars disabled, deletes the quarter only if the base periods attached to the quarter have no transactions. If true, deletes the quarter and all its base periods. With Multiple Calendars enabled, deletes the quarter and reassigns its base periods to the fiscal year. |
| Year | Allowed only if the year has no subperiods, or if its subperiods can be deleted | Deletes the year and all subperiods for that year. |

For instructions to delete an accounting period, see [Editing an Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446881.html).

For information about fiscal calendars, see [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html).

### Related Topics

-   [Manage Accounting Periods Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445839.html)
-   [Setting Up Accounting Periods for a Year](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446183.html)
-   [Setting Up Single Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446470.html)
-   [Editing an Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446881.html)
-   [Viewing the Status of Accounting Period Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449023.html)
-   [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
