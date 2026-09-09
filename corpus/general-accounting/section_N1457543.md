---
id: "section_N1457543"
type: "section"
title: "Reopening a Closed Period"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Accounting Period Close > Reopening a Closed Period"
parent: "section_N1452509"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457543.html"
anchors: ["procedure_N1457581"]
sha256: "ed66574c8f60355a0daaee8a29875aa2337459cfbbdd7657bc290f54af38ddae"
---

When a period is closed, it's considered complete and no one can add or make general ledger impacting changes to posting transactions for the period. If a period that has been closed requires later changes, you must reopen the period before these changes can be completed.

You must have the **Manage Accounting Periods** permission to reopen a period. For more information, see [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html).

If your user role has the Period Closing Management permission and the Allow Quick Close of Accounting Periods preference is enabled, you can close one or more accounting periods with a single click. For more information, see [Using Quick Close to Close Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html#bridgehead_4634078458).

If you use Multi-Book Accounting, you can individually close and reopen accounting periods associated with any accounting book, without impacting your other accounting books. You choose the accounting book for which you want to close a period through the Filters section at the top of the Manage Accounting Periods page. The accounting books available for selection depend upon your user role and associated permissions. For more information about the Extended Accounting Period Close Process feature, see [Accounting Book Period Close Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4308385929.html).

Note:

These restrictions don't apply to non-posting transactions such as sales orders and return authorizations. See [Non-Posting Transactions in Locked and Closed Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452887.html).

#### To reopen a closed period: {#procedure_N1457581}

1.  Go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.
    
2.  Click the **Checklist** icon ![Checklist icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/PeriodCheckIcon.png) for the period.
    
3.  On the Period Close Checklist page, click the arrow icon for the **Close** task.
    
4.  On the Close Accounting Period page, click **Reopen Period**.
    
5.  Enter text in the **Justification** field to explain why you're reopening the period, click **Reopen Period** again, and review the warning text to make sure you understand the following:
    
    If you reopen the period, you may need to redo checklist tasks to close the period. Also, any later closed periods are automatically reopened and you may need to redo checklist tasks for those periods as well before you can close them.
    
6.  If you want to continue, click **OK** in the warning dialog.
    
    The justification text is saved in a user note.
    

Note:

If the **Allow Non-G/L Changes** box is checked on a period record, you can make changes to posting transactions that don't affect the general ledger. You must have the Setup permission **Allow Non G/L Changes** to make these changes.

### Related Topics

-   [Accounting Period Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html)
-   [Non-Posting Transactions in Locked and Closed Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452887.html)
-   [Using the Period Close Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1455781.html)
-   [Inventory Tasks on the Period Close Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1456591.html)
-   [Unlocking Period Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457300.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
