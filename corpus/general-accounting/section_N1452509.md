---
id: "section_N1452509"
type: "section"
title: "Accounting Period Close"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Accounting Period Close"
parent: "chapter_N1445226"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html"
anchors: ["procedure_0622110625", "procedure_N1452528", "bridgehead_4634078458", "bridgehead_4634104844", "bridgehead_4634106811", "procedure_0621024542", "bridgehead_4634150333", "procedure_0621025118", "bridgehead_N1452595", "procedure_N1452650"]
sha256: "a8092837ac0dfd36000a6fa8341c949f0001db2482fc4b265dce8ce6b876e821"
---

Closing an accounting period means changing its status from Open to Closed. A status of Closed indicates that posting transactions for the period have been completed. This status prevents posting to the general ledger for any dates included in the period, by anyone. Closing a period should be a final step, after a process of accounts review and reconciliation to ensure correctness and balance.

For information about closing accounting periods, see the following topics:

-   [Period Close Checklist](#procedure_N1452528)
    
-   [Using Quick Close to Close Periods](#bridgehead_4634078458)
    
-   [Making Changes to Locked and Closed Periods](#bridgehead_N1452595)
    
-   [Approving Transactions from Closed Periods](#procedure_N1452650)
    

If you use Multi-Book Accounting, you can individually close and reopen accounting periods associated with any accounting book, without impacting your other accounting books.

#### To close the period for the selected accounting book: {#procedure_0622110625}

1.  Go to _Setup > Accounting > Manage GL > Manage Accounting Periods_.
    
2.  Choose the accounting book for which you want to close a period through the Filters section.
    
    The accounting books available for selection depend upon your user role and associated permissions.
    
3.  Go to Period Close Checklist of the period you want to close.
    
4.  Complete all tasks in the checklist. For more details, see [Using the Period Close Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1455781.html).
    
5.  At the end of the checklist, go to the task Close and mark it as complete.
    

For more information about the Extended Accounting Period Close Process feature, see [Accounting Book Period Close Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4308385929.html)

## Period Close Checklist {#procedure_N1452528}

A Period Close Checklist for each period is available from the Manage Accounting Periods page. From this checklist, you can complete required tasks in sequence, and then close the period.

-   Preliminary tasks lock the period to limit posting transactions. Locking tasks include **Lock A/P**, **Lock A/R**, **Lock Payroll** (if the Payroll feature is enabled), and **Lock All**.
    
-   Other tasks such as Create Intercompany Adjustments, Revalue Open Foreign Currency Balances, Recognize Revenue, Reclassify Revenue, and Calculate Consolidated Exchange Rates, provide necessary adjustments. To complete these tasks, users require related permissions. For example, the Revalue Open Foreign Currency Balances task requires Create level Currency Revaluation permission.
    
-   If you have enabled the GL Audit Numbering feature, GL Audit Numbering is listed as a task required as part of the period close process. Assign the number sequence for the period and then verify that the GL audit numbering is gapless. If you use NetSuite OneWorld, you can create sequences for each subsidiary. If you use Multi-Book Accounting, you can define book-specific numbering sequences. For more information, see [GL Audit Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3735573963.html).
    
-   The final task is to close the period.
    
-   The Period Close Checklist provides access to related system and user notes.
    

For more information, including the procedure for closing the period, see [Using the Period Close Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1455781.html) and [Inventory Tasks on the Period Close Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1456591.html).

## Using Quick Close to Close Periods {#bridgehead_4634078458}

The Quick Close preference enables you to close one or more accounting periods with a single click. This time-saving preference is useful when you have reopened one or more closed accounting periods to make a change. With Quick Close, NetSuite marks complete all tasks in all reopened accounting periods, eliminating the requirement to close them one-by-one.

For example, you want to make a change in the January 2016 accounting period. Reopen the period, which reopens all of the subsequent closed periods. Make your change. With Quick Close, you can close the January 2016 period and all subsequent periods at the same time.

The Quick Close preference is also useful when you prefer a one-click method for closing accounting periods. For example, you're the sole proprietor of your business. You process all accounting transactions. You don't want to go through each task on the period close checklist to close accounting periods. With Quick Close, you can close each period with a single click.

Warning:

The Period Close Checklist helps you with your financial closing workflow. Quick Close **doesn't** run period closing tasks. It only marks the tasks as completed. Use Quick Close **only** when you're certain that there is no requirement to run period closing tasks.

-   [Granting Permission to Use Quick Close](#bridgehead_4634104844)
    
-   [Enabling the Quick Close Preference](#bridgehead_4634106811)
    
-   [Closing Accounting Periods with Quick Close](#bridgehead_4634150333)
    

## Granting Permission to Use Quick Close {#bridgehead_4634104844}

Quick Close is automatically granted to administrators. The Setup permission, Period Closing Management, must be added to other roles for users to use the feature. For information about NetSuite permissions, see [NetSuite Permissions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N325094.html) and [Permissions Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326485.html).

## Enabling the Quick Close Preference {#bridgehead_4634106811}

If your user role is granted both the Set Up Accounting and Period Closing Management permissions and you want to use Quick Close, you must enable the Allow Quick Close of Accounting Periods preference.

#### To enable the Allow Quick Close preference: {#procedure_0621024542}

1.  Go to _Setup > Accounting > Accounting Preferences_.
    
    Note:
    
    This preference doesn't appear in user roles that don't have the Period Closing Management permission.
    
2.  On the General subtab under the General Ledger section, click the **Allow Quick Close of Accounting Periods** box.
    
3.  Click **Save**.
    

For information about general accounting preferences, see [General Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html).

## Closing Accounting Periods with Quick Close {#bridgehead_4634150333}

If you have the appropriate permissions and the Allow Quick Close of Accounting Periods preference is enabled, you can close accounting periods using Quick Close.

Important:

The Quick Close function supports closing up to five open accounting periods at a time. Attempting to close more than five periods in one run can cause the system to become unresponsive and the process to fail. If you need to close more than five periods, run Quick Close in smaller batches.

#### To close one or more Accounting Periods with Quick Close: {#procedure_0621025118}

1.  Go to _Setup > Accounting > Manage Accounting Periods_.
    
2.  Click the **Close Multiple Periods** option above the list.
    
3.  In the popup, select the latest period you want to close from the drop down list, NetSuite will include prior open periods up to that date. If Multi-Book Accounting is provisioned (NetSuite OneWorld), select the accounting book associated with the periods you're closing.
    
    Note:
    
    If you're closing more that five periods, divide them into small batches of up to five periods to prevent errors. Start from the oldest open periods in the list, because Quick Close includes all earlier periods up to the one you choose.
    
    For example, to close periods from January 2025 through September 2025, first set _Period to Close = May 2025_ and all previous periods (closes January to May). Then set _Period to Close = Sep 2025 and all previous periods_, to close the remaining four. Repeat this process as needed until all desired periods are closed.
    
4.  Click **Submit**.
    
5.  At the prompt, click **OK**.
    

NetSuite maintains an audit trail of every changed task in every closed accounting period through system notes. For more information, see [System Notes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_158644279544.html).

## Making Changes to Locked and Closed Periods {#bridgehead_N1452595}

Users with the Override Period Restrictions permission can add and edit posting transactions even if the transaction type has been locked for a period. To allow other users to add or edit posting transactions, transactions must be unlocked for the period. See [Unlocking Period Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457300.html).

Note:

Changes to addresses are not permitted in a closed accounting period. Changing the address on a transaction could alter the tax rate, and have an impact on the general ledger.

No one can make general ledger impacting changes to posting transactions in a closed period. The period must be reopened before these changes can be posted. See [Reopening a Closed Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457543.html).

If the Allow Non-G/L Changes box is checked on a period record, you can make changes to posting transactions that don't affect the general ledger. You must have the Setup permission Allow Non G/L Changes to make these changes.

These permission restrictions don't apply to the addition or editing of non-posting transactions such as sales orders and return authorizations. See [Non-Posting Transactions in Locked and Closed Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452887.html).

Note:

Account administrators have both the Override Period Restrictions and Allow Non-G/L Changes permissions. To assign a user these permissions, go to Setup > Users/Roles > Manage Users and select a user. In the user record's **Access** subtab, click the **Global Permissions** subtab. In the **Permission** field, select a permission and click **Add**. Then, click **Save**.

## Approving Transactions from Closed Periods {#procedure_N1452650}

Transactions that are subject to approval must be approved before posting. For journal entries, you can select a posting period before approval.

You can't select a closed period. You can select an open and locked period only if your role includes the Override Period Restrictions permission.

For other posting transactions, the posting period may be determined upon approval and may vary from the period displayed on transaction entry forms and unapproved records.

### Related Topics

-   [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html)
-   [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html)
-   [Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449211.html)
-   [GL Audit Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3735573963.html)
-   [Rules for Future Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451349.html)
-   [Year-End Closing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457773.html)
-   [Reporting by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1458661.html)
-   [Searching by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1459178.html)
-   [Locking Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N560870.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
