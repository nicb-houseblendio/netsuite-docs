---
id: "section_N1451349"
type: "section"
title: "Rules for Future Accounting Periods"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Rules for Future Accounting Periods"
parent: "chapter_N1445226"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451349.html"
anchors: ["bridgehead_N1451399", "bridgehead_N1451411", "bridgehead_N1451423"]
sha256: "24f010d184efbca1161f916263e2746b1978065f59f4d55a50a9d86a23ffb669"
---

Use the **Enable Accounting Period Window** accounting preference to both maintain a minimum number of unlocked accounting periods and prevent entries in locked future periods. When you check the box for this preference, you must set the minimum number of current and future accounting periods available for transactions. All other future periods are locked for posting. NetSuite unlocks the next future period for the window as needed on the first day of each period.

Locking future periods prevents users from entering transaction data and journal entries by mistake. The period window ensures that most users post transactions only within the window of unlocked periods. A user whose role includes the Override Period Restrictions permission, however, can post in either locked or unlocked periods.

The size of the accounting period window is determined by the number you enter in the **Minimum Period Window Size** field below the Enable Accounting Period Window preference. The value in this field is the number of unlocked current and future periods. The accounting period window applies to accounting periods as a whole and individually to accounting transactions for accounts receivable, accounts payable, and payroll. See [Setting the Enable Accounting Period Window Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451595.html).

Note:

You can lock future periods and types of transactions without checking the **Enable Accounting Period Window** accounting preference. However, doing so locks **all** periods or types of transactions prior to that point including the current period. In addition, future locked accounting periods don't display the lock ![Lock icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/lock.png) icon.

## Period Window {#bridgehead_N1451399}

The accounting period window is the minimum number of current and future accounting periods that are open and unlocked. You can configure the size of the window to any number of periods from 1 to 1,000. The accounting period window ensures that a specific number of open periods are unlocked and available for posting transactions. When you close a period or lock a set of transactions, NetSuite unlocks the next period or set of transactions. This prevents accounting period starvation and eliminates the accounting cycle task of opening the next period for data entry.

The minimum period window uses the system date to determine the current and future open periods. For example, if the system date is June 15 and the Minimum Period Window Size is 3, June, July, and August are all open. However, if the Minimum Period Window Size is 1, only June (the current period) is open.

## Period Wall {#bridgehead_N1451411}

The period wall is the end of the current accounting period. If today's date is January 7, the period wall is January 31. Accounting periods to the right of the period wall are future periods. Periods to the left of the wall are the current period and past periods. The period wall concept is useful for determining which periods are past, current, and future for purposes of the period window.

## Locking Accounting Period Window Rules {#bridgehead_N1451423}

Locking accounting periods follows four basic rules. These rules use the period wall to determine whether locking or unlocking affects other accounting periods. Use the diagram below to understand the impact of each rule. Accounting period window rules apply to both accounting periods and to accounting transactions, such as A/R Transactions.

![Diagram showing the impact of four rules that apply to locking accounting periods.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/periodwall.png)

-   Locking a future period automatically locks all future periods after the locking point (to the right of the locking point).
    
-   Locking a past period automatically locks all past periods prior to the locking point (to the left of the locking point).
    
-   Unlocking a future period automatically unlocks all periods between the period wall and the unlocking point.
    
-   Unlocking a past period automatically unlocks all periods between the period wall and the unlocking point.
    

You can manually unlock more periods than the number set in the Minimum Period Window Size preference. Locked future or past periods must be continuous and without gaps from the locking or unlocking point.

You can't lock a period that is within the current minimum period window. For example, if your window size is 3 and your current accounting period is January, you can't lock February or March.

For instructions on how to lock and unlock accounting periods, see [Locking and Unlocking Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451780.html) and [Locking Accounting Periods in NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452163.html).

### Related Topics

-   [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html)
-   [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html)
-   [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html)
-   [GL Audit Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3735573963.html)
-   [Accounting Period Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html)
-   [Year-End Closing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457773.html)
-   [Reporting by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1458661.html)
-   [Searching by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1459178.html)
-   [Locking Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N560870.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
