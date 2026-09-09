---
id: "section_N1452163"
type: "section"
title: "Locking Accounting Periods in NetSuite OneWorld"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Rules for Future Accounting Periods > Locking Accounting Periods in NetSuite OneWorld"
parent: "section_N1451349"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452163.html"
anchors: ["procedure_N1452331"]
sha256: "95ebcee300e7978b2f1a49a7b96288bb38af697d276028e6655d404138e9ff23"
---

In NetSuite OneWorld, you can lock or unlock accounting periods at the subsidiary level. You can manage your period close process based on the workflow needs of your organization. Only controllers and administrators with the permission to perform period close tasks at the parent subsidiary level can select subsidiaries to lock or unlock.

For information about locking and unlocking accounting periods in NetSuite if you're not using OneWorld, see [Locking and Unlocking Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451780.html).

When an accounting period is locked for a subsidiary, users can't enter transactions for the subsidiary in that period. The locked period isn't available in the Posting Period list in transactions. If a user selects a transaction date that falls within a locked period, the Posting Period is set to the current open period for the subsidiary. This happens only if the **Allow Transaction Date Outside of Posting Period** preference is set to Disallow or Warn.

Note:

Users with the **Override Period Restrictions** permission can select a locked period for the Posting Period on a transaction.

If the **Enable Accounting Period Window** accounting preference is checked, NetSuite maintains a minimum number of unlocked current and future accounting periods. In this case, locking a transaction module or a period for a subsidiary can trigger automatic opening of the next future period, based on the defined minimum period window size. NetSuite opens the next future period for all subsidiaries to maintain the same period window across your organization.

Use the Lock Accounting Period page, available from the Period Close Checklist, to select subsidiaries to lock.

The Subsidiaries subtab on the Lock Accounting Period page displays the subsidiary hierarchy for your organization.

Important:

The Subsidiaries subtab displays only those subsidiaries that your role has permission to access. If your role doesn't have permission to access all of the subsidiaries, you can't see the complete subsidiary hierarchy.

A Lock icon in the Current Value column indicates the subsidiaries that are locked for transactions. Mark or unmark the box in the Lock column for each subsidiary, as needed.

On the Notes subtab, the System Notes subtab displays each change made to the lock status including the subsidiary information. You can include subsidiary information in any searches that include system notes to search and report on period locking history by subsidiary. For information about how to set up a search, see [Creating Saved Searches for System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691977.html).

Note:

The first time that any task is viewed, System Notes logs a Create entry.

On the Period Close Checklist, icons in the Status column indicate whether a task is completed, partially done, or not started. The status for a Lock task shows as partially done when you lock at least one subsidiary for the task.

The Manage Accounting Periods page displays accounting period status at a glance using the following icons:

-   ![Unlocked icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/unlocked.png) **Unlocked** - All subsidiaries are unlocked
    
-   ![Partially Locked icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/inprogress.png) **Partially Locked** - One or more subsidiaries are locked. Point to the icon to see the number of locked subsidiaries. This number reflects the complete subsidiary hierarchy, not only the subsidiaries you have permission to access.
    
-   ![Locked icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/lock.png) **Locked** - All subsidiaries are locked.
    

#### To lock or unlock accounting periods in NetSuite OneWorld: {#procedure_N1452331}

1.  Go to _Setup > Accounting > Manage GL > Manage Accounting Periods_.
    
2.  On the Manage Accounting Periods page, click the **Checklist** icon ![Checklist icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/PeriodCheckIcon.png) for the period.
    
3.  On the Period Close Checklist, click the **Go To Task** icon for **Lock AR**, **Lock AP**, **Lock Payroll**, or **Lock All**.
    
4.  On the **Subsidiaries** subtab, mark the **Lock** box for each subsidiary you want to lock.
    
    You can also **Mark All** or **Unmark All** to change the value of the lock for all subsidiaries.
    
    Important:
    
    **Mark All** or **Unmark All** locks or unlocks only those subsidiaries that display on this subtab, which depending on your permissions, may not include the complete subsidiary hierarchy.
    
    To unlock a subsidiary, clear the **Lock** box.
    
5.  Click **Submit**.
    

### Related Topics

-   [Rules for Future Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451349.html)
-   [Setting the Enable Accounting Period Window Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451595.html)
-   [Locking and Unlocking Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451780.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
