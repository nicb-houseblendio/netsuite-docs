---
id: "section_N1450241"
type: "section"
title: "Adjustment Periods"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Fiscal Calendars > Adjustment Periods"
parent: "section_N1449211"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450241.html"
anchors: ["procedure_N1450568", "bridgehead_N1450605"]
sha256: "5ecbcebedc6e0478773ced2835c859ce6e0b52a119d7c70881b387c633a70855"
---

Adjustment periods must overlap existing base (non-adjustment) accounting periods when the Multiple Calendars feature enabled.

You can set up new adjustment periods two ways:

-   Use **Set Up Full Year** to generate a one-day adjustment period at the end of a new fiscal year. You must check the **One-day Year-End Adj.** Period box.
    
-   Manually create a period using the **Create Single Period** button and check the **Period is Adjustment** box. Manually created adjustment periods can be more than one day in length.
    

You can post only journal entries to an adjustment period. Adjustment periods are not available in the posting period list for other posting transactions. An adjustment period is never the default posting period, even for a journal.

Note:

If you want an approved journal to post in an adjustment period, you must edit the journal, approve it, and select the adjustment period as the posting period. For more information, see [Journal Entry Approval Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1471271.html).

If you use Multiple Calendars and include adjustment periods in your fiscal years, you can have more than one adjustment period in the same calendar year. Journal entries posted to an adjustment period roll up in the fiscal year to which they belong and are included in consolidated reports accordingly.

|  | Standalone Periods | Overlapping Periods |
| --- | --- | --- |
| Period | Start Date | End Date | Start Date | E nd Date |
| --- | --- | --- | --- | --- |
| Dec 2014 | 12/1/2014 | 12/30/2014 | 12/1/2014 | 12/31/2014 |
| ADJ 2014 | 12/31/2014 | 12/31/2014 | 12/31/2014 | 12/31/2014 |

As best practice, you should lock accounting periods as part of your month-end process. After the period is locked, only users with the Override Period Restrictions permission can post transactions in the period. User with this permission can make adjusting journal entries in locked periods, which serves the same purpose many adjustment period journal entries. If you have more than one fiscal calendar, you may be able to avoid having multiple adjustment periods in the same calendar year by using adjusting journal entries. See [Locking and Unlocking Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451780.html) and [Locking Accounting Periods in NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452163.html).

Note:

Before you can enable the Multiple Calendars feature, all adjustment periods must be overlapping periods.

#### To modify an accounting period date ranges: {#procedure_N1450568}

1.  Go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.
    
2.  Click the accounting period you want to change.
    
3.  Set the **End Date** for the period to include adjustment period date.
    
4.  Click **Save**.
    

## Adjustment Periods without Multiple Calendars {#bridgehead_N1450605}

If you're not using the Multiple Calendars feature, you can create standalone or overlapping adjustment periods. See [Setting Up Accounting Periods for a Year](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446183.html) and [Setting Up Single Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446470.html).

### Related Topics

-   [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html)
-   [Enabling Multiple Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449485.html)
-   [Creating a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449559.html)
-   [Setting Up Accounting Periods for a Full Year for Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449871.html)
-   [Setting Up Single Accounting Periods for Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449971.html)
-   [Restriction and Automation Rules Governing Accounting Period Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450765.html)
-   [Multiple Calendars with Other NetSuite Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1450943.html)
-   [Searching Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4193640975.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
