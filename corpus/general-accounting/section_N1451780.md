---
id: "section_N1451780"
type: "section"
title: "Locking and Unlocking Accounting Periods"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Rules for Future Accounting Periods > Locking and Unlocking Accounting Periods"
parent: "section_N1451349"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451780.html"
anchors: ["procedure_N1451808", "procedure_N1451877", "procedure_N1451965", "bridgehead_N1452030"]
sha256: "d451e2774e0a8757d9dd25865363ea95e76b6467a255a06c13e16e8723f9983b"
---

You can lock accounting periods or transaction modules for a period to prevent users from posting transactions that affect the general ledger. Locking is part of the period close process.

If you check the Enable Accounting Period Window accounting preference, you can also lock future periods to provide greater control for your accounting process. When this preference is checked, lock ![Lock icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/lock.png) icons are displayed for future accounting periods. See [Rules for Future Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451349.html) for information about how locking and unlocking periods performs with this preference.

#### To lock an accounting period: {#procedure_N1451808}

1.  Go to _Setup > Accounting > Manage GL > Manage Accounting Periods_.
    
2.  Click the **Checklist** icon ![Checklist icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/PeriodCheckIcon.png) for the period.
    
3.  Click the **Go To Task** icon for **Lock All**.
    
4.  If you're a NetSuite OneWorld user, select which parent or subsidiary to lock the accounting period for.
    
5.  On the Task: Lock Accounting Period (All) page, click **Submit**.
    

#### To lock a transaction module: {#procedure_N1451877}

1.  Go to _Setup > Accounting > Manage GL > Manage Accounting Periods_.
    
2.  Click the **Checklist** icon ![Checklist icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/PeriodCheckIcon.png) for the period.
    
3.  On the Period Close Checklist page, do one of the following:
    
    1.  To lock A/R transactions in the period, click the **Lock A/R** icon, then click **Lock**.
        
    2.  To lock A/P transactions in the period, click the **Lock A/P** icon, then click **Lock**.
        
    3.  To lock Payroll transactions in the period, click the **Lock Payroll** icon, then click **Lock**.
        
    
    Note:
    
    If you're a NetSuite OneWorld user, select which parent or subsidiary to lock the accounting period for before you click Lock.
    

To unlock an accounting period, you must unlock each transaction module in the period.

#### To unlock an accounting period: {#procedure_N1451965}

1.  Go to _Setup > Accounting > Manage GL > Manage Accounting Periods_.
    
2.  On the Manage Accounting Periods page, click the **Checklist** icon ![Checklist icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/PeriodCheckIcon.png) for the period.
    
3.  On the Period Close Checklist page, click the **Lock A/R** icon, then click **Unlock**.
    
    Repeat this step for **Lock A/P**, **Lock Payroll**, and **Lock All** tasks.
    
    Note:
    
    If you're a NetSuite OneWorld user, select which parent or subsidiary to unlock the accounting period for before you click Unlock.
    

## To unlock a transaction module: {#bridgehead_N1452030}

For information about how to unlock a transaction module for a period, see [Unlocking Period Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457300.html).

When you unlock a transaction module such as A/R Transactions, All GL Transactions is also unlocked.

### Related Topics

-   [Rules for Future Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451349.html)
-   [Setting the Enable Accounting Period Window Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451595.html)
-   [Locking Accounting Periods in NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452163.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
