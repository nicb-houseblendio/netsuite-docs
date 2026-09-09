---
id: "section_N1457300"
type: "section"
title: "Unlocking Period Transactions"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Accounting Period Close > Unlocking Period Transactions"
parent: "section_N1452509"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457300.html"
anchors: ["procedure_N1457351"]
sha256: "729cf5a8a5c19c053094913c2af5a3a286211705a3dfc460c11963bfadc0880e"
---

Locking out transactions, including custom transactions that post to Accounts Payable, Accounts Receivable, and Payroll (if applicable) are prerequisite tasks for closing a period. These locks enable accounting personnel to review stable accounts and enter adjustments, as necessary.

Locking doesn't lock the entire transaction. It locks the general ledger impacting changes to posting transactions on the locked account. To make general ledger impacting changes to posting transactions on a locked account, the specific type of lock must be released. For example, releasing Lock A/P.

Locking transactions applies to all transactions including general journals and intercompany journals whether they're generated from the user interface, CSV imports, WebServices, SuiteScript, and ODBC.

When a period that has been locked has the Allow Non-G/L Changes box checked, users can make changes to posting transactions if the changes don't affect the general ledger. Users must have the Setup permission **Allow Non G/L Changes** to make such changes. Users with the **Override Period Restrictions** permission can make changes to posting transaction, whether the changes impact the general ledger or not, in a period that has been locked to transactions.

If users who don't have the Override Period Restrictions permission must make changes to posting transactions that impact the general ledger, transactions must be unlocked for the period. You can't unlock transactions for a closed period. You must first reopen the period. See [Reopening a Closed Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457543.html).

Note:

These permission restrictions don't apply to non-posting transactions such as sales orders and return authorizations. See [Non-Posting Transactions in Locked and Closed Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452887.html).

#### To unlock transactions for a period: {#procedure_N1457351}

1.  Go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.
    
2.  Click the **Checklist** icon ![Checklist icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/PeriodCheckIcon.png) for the period.
    
3.  On the Period Close Checklist page, do one of the following
    
    1.  To unlock A/R transactions in the period, click the **Lock A/R** icon, then click **Unlock**.
        
    2.  To unlock A/P transactions in the period, click the **Lock A/P** icon, then click **Unlock**.
        
    3.  To unlock Payroll transactions in the period, click the **Lock Payroll** icon, then click **Unlock**.
        
    4.  To unlock other transactions in the period, click the **Lock All** icon, then click **Unlock**.
        

After all transactions are unlocked for a period with Allow Non-G/L Changes box checked, the box is cleared. If transactions are later locked, you can check the box again.

### Related Topics

-   [Accounting Period Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html)
-   [Non-Posting Transactions in Locked and Closed Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452887.html)
-   [Using the Period Close Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1455781.html)
-   [Inventory Tasks on the Period Close Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1456591.html)
-   [Reopening a Closed Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457543.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
