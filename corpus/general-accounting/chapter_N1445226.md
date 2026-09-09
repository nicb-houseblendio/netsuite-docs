---
id: "chapter_N1445226"
type: "chapter"
title: "Accounting Period Management"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management"
parent: "preface_3710627041"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html"
anchors: ["subsect_1532733689"]
sha256: "c1754afda32aadc0a84889377c23ddb49f4dc9ed540dd7253b4ac08962184145"
---

The Accounting Periods feature supports general ledger management. If accounting periods are not used, NetSuite transactions post in real time. When accounting periods are enabled, users can select a past or future posting period for each transaction, and accounting personnel can more effectively monitor and control the status of accounts.

Note:

If your system has historical transaction data and you want to use the Accounting Periods feature, enable the feature and then create an accounting period for a past quarter or month. NetSuite automatically assigns that accounting period to the transactions dated within the period's date range.

A user with the Enable Features permission can enable the Accounting Periods feature at _Setup> Company > Enable Features_, on the Accounting subtab. After the feature is enabled, periods can be set up at _Setup > Accounting > Manage G/L > Manage Accounting Periods_. See [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html).

Important:

If you don't use NetSuite OneWorld, you can't disable the Accounting Periods feature if an accounting period exists. To disable the feature you must delete all created accounting periods.

NetSuite OneWorld supports using fiscal calendars to define fiscal years with different start and end dates per subsidiary. See [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html).

If your international auditing requirements include gapless numbering sequences to all general ledger posting transactions, enable the GL Audit Numbering feature. When this feature is enabled, numbering general ledger posting transactions is a required task when closing the **last month** in an accounting period. For more information see, [GL Audit Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3735573963.html). If your country requires that corrections are made as adjustment transactions posted to the same accounts as the original transactions, see [GL Impact Locking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4725785967.html).

If you use Multi-Book Accounting, you can individually close and reopen accounting periods associated with any accounting book, without impacting your other accounting books. You choose the accounting book for which you want to close a period through the Filters section at the top of the Manage Accounting Periods page. The accounting books available for selection depend upon your user role and associated permissions. For more information about the Extended Accounting Period Close Process feature, see [Accounting Book Period Close Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4308385929.html).

For information about managing tax periods, see [Working with Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797157.html).

Periods can be locked to prevent the posting of transactions that affect the general ledger. The locking of a period to A/P, A/R, and Payroll transactions provides a pre-closed state that permits the balancing of a period's financials before closing. These locking tasks are the first steps in a Period Close Checklist of tasks available in the NetSuite user interface. After these tasks are completed, the period can be closed. After a period is closed, it's unavailable for adding new posting transactions or making edits that impact the general ledger. For more information, see [Accounting Period Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html).

You can automatically maintain several unlocked current and future periods to facilitate your monthly business and accounting processes and prevent erroneous data entry in future periods. See [Rules for Future Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451349.html).

The Accounting Periods feature permits organization of report, search, and key performance indicator data by periods to simplify financial review and analysis. For information about sorting and filtering report data by period, see [Reporting by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1458661.html). For information about filtering and displaying search data by period, see [Searching by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1459178.html).

## Permissions Related to Accounting Periods {#subsect_1532733689}

Be aware of the following permissions requirements for accounting periods:

-   **Edit** or **Full** level of the **Manage Accounting Periods** permission is required to set up, edit, lock transactions for period close, or reopen accounting periods.
    
    Users with the **View** level of this permission can see the Manage Accounting Periods page but can't make changes to periods.
    
    Important:
    
    When a journal entry, intercompany journal entry, statistical journal entry, or commission transaction has no defined posting period, users with **View** level of the **Manage Accounting Periods** permission see a suggested accounting period in the Posting Period field on the transaction. For example, if January is a locked accounting period, an A/R Clerk with **View** level of the permission would see the suggested posting period as February. An administrator with **Full** level of the permission would see the suggested posting period as January.
    
    For the following transactions, users with **View** level of the **Manage Accounting Periods** permission don't see a suggested posting period when there is no defined accounting period: Cash Sale, Check, Credit Card Charge, Credit Card Refund, Customer Refund, Credit Memo, Customer Payment, Deposit, Expense Report, Inventory Adjustment, Invoice, Item Fulfillment, Item Receipt, Transfer, Vendor Bill, and Vendor Payment.
    
-   The **Override Period Restrictions** permission is required to add and make general ledger impacting changes to posting transactions in periods that have been locked to transactions.
    
-   Users must have both of the above permissions in addition to task-specific permissions to complete Period Close Checklist tasks such as automated intercompany adjustments, open currency balance revaluations, and calculation of consolidated exchange rates.
    
-   The Setup permission **Allow Non G/L Changes** permits changes to posting transactions in locked or closed periods under the following conditions:
    
    -   The **Allow Non-G/L Changes** box is checked on the period record.
        
    -   The change doesn't impact the general ledger.
        
-   No one can make changes to posting transactions in a closed period if the changes would impact the general ledger. The period must be reopened before these changes can be posted.
    
-   These permission restrictions don't apply to the addition or editing of non-posting transactions such as sales orders and return authorizations. See [Non-Posting Transactions in Locked and Closed Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452887.html).
    

### Related Topics

-   [Year-End Closing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457773.html)
-   [Locking Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N560870.html)
-   [NetSuite Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1379709.html)
-   [Accounting Features and Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1383640.html)
-   [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html)
-   [Chart of Accounts Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1439850.html)
-   [General Ledger Impact of Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1459499.html)
-   [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html)
-   [Budgets in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1503165.html)
-   [Account Registers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1508800.html)
-   [Accounting-Related Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1519116.html)
-   [Sequential Liability SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_158408768320.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
