---
id: "section_N1445585"
type: "section"
title: "Accounting Period Setup"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Accounting Period Setup"
parent: "chapter_N1445226"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html"
anchors: []
sha256: "2bbf749fc2088fab0949c86a0fa62fc7b5381ff526f158eb61d51d53e0d44904"
---

A user with at least **Edit** level of the **Manage Accounting Periods** permission can set up fiscal periods one period at a time or one fiscal year at a time. For more information, see:

-   [Manage Accounting Periods Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445839.html)
    
-   [Setting Up Accounting Periods for a Year](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446183.html)
    
-   [Setting Up Single Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446470.html)
    
-   [Editing an Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446881.html)
    
-   [Accounting Period Deletion Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1448709.html)
    

Users with custom Accounting Center roles must have the **Posting Period on Transactions** permission to set up accounting periods.

Important:

If you don't use NetSuite OneWorld, you can't disable the Accounting Periods feature if an accounting period exists. To disable the feature you must delete all created accounting periods.

In NetSuite OneWorld, if you enable the Multiple Calendars feature you can create fiscal calendars and use different accounting period rollups for your subsidiaries. The base accounting periods that roll up into these hierarchies are common to all subsidiaries.

If you use fiscal calendars and are creating an Accounting Period search (_Lists > Search > Saved Search > New_ > Accounting Period), you can filter your search based on the fiscal calendar.

For information about defining a saved search, see [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html). For information about fiscal calendars, see [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html).

For information about managing tax periods, see [Working with Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797157.html).

For more information about accounting periods, see the following help topics:

-   [Setting Up Accounting Periods for a Full Year for Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449871.html)
    
-   [Setting Up Single Accounting Periods for Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449971.html)
    

Important:

Each day must belong to an accounting period to ensure accuracy in reporting.

Accounting periods can't be set up until the Accounting Periods feature has been enabled. See [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html).

Note:

If your system has historical transaction data and you want to use the Accounting Periods feature, enable the feature and then create an accounting period for a past quarter or month. NetSuite automatically assigns that accounting period to the transactions dated within the period's date range.

If you create an accounting period that precedes a locked period, the new period you create is locked upon creation. For example, you have created an accounting period for fiscal year 2013. The period is closed and locked. You have transactions to enter for fiscal year 2012, so you create an accounting period for that fiscal year. When you save the new period, it's saved locked to prevent mismatches and accidental general ledger impact in the periods that follow. You must manually unlock A/R and A/P in each period to enter the transactions.

When you set up or make changes to accounting periods, a batch process runs to align transactions with the appropriate accounting period. See [Viewing the Status of Accounting Period Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449023.html).

Users with **View** level of the **Manage Accounting Periods** permission can view the Manage Accounting Periods page but can't add or edit periods.

Note:

If the Accounting Periods feature has been enabled, users can set a personal preference to view report data by period. See [Reporting by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1458661.html). After this preference has been set for a user's reports, these reports can't display results to the user until accounting periods for the entire fiscal year have been set up.

### Related Topics

-   [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html)
-   [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html)
-   [GL Audit Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3735573963.html)
-   [Rules for Future Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451349.html)
-   [Accounting Period Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html)
-   [Year-End Closing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457773.html)
-   [Reporting by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1458661.html)
-   [Searching by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1459178.html)
-   [Locking Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N560870.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
