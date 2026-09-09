---
id: "section_N1445839"
type: "section"
title: "Manage Accounting Periods Page"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Accounting Period Setup > Manage Accounting Periods Page"
parent: "section_N1445585"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445839.html"
anchors: []
sha256: "159be2d93faea029f9b9c2cd080852658fc5bcadfddead9f05888395610b9cec"
---

The Manage Accounting Periods page is a list of all of the accounting periods set up in your account, and rolled up in the accounting period hierarchy to which they belong. Use this page to set up, view, and edit periods. You can also access the Period Close Checklist to lock, unlock, and close accounting periods. To see this page, go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.

Note:

This page is available if you have the **View** level or higher of the **Manage Accounting Periods** permission. You must have at least the **Edit** level of this permission to set up or edit accounting periods.

If your user role has the Period Closing Management permission and the Allow Quick Close of Accounting Periods preference is enabled, you can close one or more accounting periods with a single click. For more information, see [Using Quick Close to Close Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html#bridgehead_4634078458).

If you use Multi-Book Accounting, you can individually close and reopen accounting periods associated with any accounting book, without impacting your other accounting books. You choose the accounting book for which you want to close a period through the Filters section at the top of this page. The accounting books available for selection depend upon your user role and associated permissions. For more information about the Extended Accounting Period Close Process feature, see [Accounting Book Period Close Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4308385929.html).

You can filter accounting periods by fiscal calendar. For more information, see [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html).

For information about managing tax periods, see [Working with Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797157.html).

Note:

If your system has historical transaction data and you want to use the Accounting Periods feature, enable the feature and then create an accounting period for a past quarter or month. NetSuite automatically assigns that accounting period to the transactions dated within the period's date range.

This page includes the following columns:

-   **Period Name** - name you defined for the accounting period, such as FY 2012 (Fiscal Year 2012), Q1 2014 (First Quarter 2014). Periods are grouped into fiscal years, quarters, and months. Use the + or - icon to expand or collapse the list of periods for a fiscal year.
    
-   **Expand All/Collapse All** - Expand or collapse all periods.
    
-   **Checklist** - Click the Checklist icon ![Checklist icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/PeriodCheckIcon.png) to view a list of tasks to be completed to close the period. You also lock and unlock transaction modules and periods from the Checklist.
    
    Note:
    
    The first time that any task is viewed, System Notes logs a Create entry.
    
-   **Period Close** - A green check mark in this column indicates that all items on the Period Close Checklist have been completed and the accounting period is closed to all transactions and entry.
    
    Note:
    
    If Multi-Book Accounting is provisioned in NetSuite OneWorld and you have enabled the Extended Accounting Period Close Process feature, when you close all of your accounting books at the same time you can point to the Period Close icon to view information about which books are already closed and which are still opened.
    
-   **A/P Transactions** - a lock indicates that ordinary users can't post A/P transactions in this period.
    
-   **A/R Transactions** - a lock indicates that ordinary users can't post A/R transactions in this period.
    
-   **Payroll Transactions** - (if Payroll feature enabled) a lock indicates that ordinary users can't post payroll transactions in this period.
    
-   **All G/L Transactions** - a lock indicates ordinary users can't post any transaction that has general ledger impact in this period.
    
-   **Allow Non-G/L Changes** - a check indicates that users with the **Allow Non G/L Changes** permission can post changes to transactions that don't affect the general ledger.
    

On this page, you can:

-   Click a **Period Name** to make changes to edit the period. See [Editing an Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446881.html).
    
-   Click a **Checklist** icon to review the status of tasks to complete for period close, to go through this close process, and lock or unlock the period or transaction modules. See [Accounting Period Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html).
    
-   Click **Set Up Full Year** to set up an entire year of accounting periods. See [Setting Up Accounting Periods for a Year](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446183.html).
    
-   Click **Create Single Period** to set up a new accounting period. See [Setting Up Single Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446470.html).
    
-   Click **Print** to print the list of Accounting Periods.
    
-   Check the **Show Inactives** box to display inactive periods in the list and also mark periods inactive. By default, only active periods are displayed.
    
    After you check the **Show Inactives** box, an **Inactive** column is added to the page with check boxes for each period.
    
    Note:
    
    You can't create new transactions in inactive periods, but you can run reports for inactive periods.
    

### Related Topics

-   [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html)
-   [Setting Up Accounting Periods for a Year](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446183.html)
-   [Setting Up Single Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446470.html)
-   [Editing an Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446881.html)
-   [Locking and Unlocking Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451780.html)
-   [Accounting Period Deletion Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1448709.html)
-   [Viewing the Status of Accounting Period Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449023.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
