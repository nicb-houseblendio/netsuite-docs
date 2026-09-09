---
id: "section_N1451595"
type: "section"
title: "Setting the Enable Accounting Period Window Preference"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Rules for Future Accounting Periods > Setting the Enable Accounting Period Window Preference"
parent: "section_N1451349"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451595.html"
anchors: ["procedure_N1451625"]
sha256: "980162e0e9e07610d920302cec4afe0babb12a14b64cce2175a01bd086b93fac"
---

Accounting periods and modules are locked or unlocked when you save changes made to the Enable Accounting Period Window accounting preference. If you check the Enable Accounting Period Window box and then later clear it, all future accounting periods are unlocked when you save your preference changes. For more information, see [Rules for Future Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451349.html)

#### To set the Enable Accounting Period Window preference {#procedure_N1451625}

1.  Go to _Setup > Accounting > Preferences > Accounting Preferences_.
    
2.  On the **General** subtab, check the **Enable Accounting Period Window** box.
    
3.  In the **Minimum Period Window Size** field, enter the **minimum** number of current and future accounting periods that you want to be unlocked at all times. You can unlock more than this number of periods manually.
    
    The minimum period window uses the system date as the baseline period to determine the future open periods. For example, if the system date is June 15 and the Minimum Period Window Size is 3, June, July, and August are all open. However, if the Minimum Period Window Size is 1, only June is open.
    
4.  Click **Save**.
    

When you set the **Enable Accounting Period Window** preference, NetSuite automatically sets the **Allow Transaction Date Outside of Posting Period** to **Disallow**. You can reset this preference to Warn or Allow if you want. For more information about this preference, see [General Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html).

In addition, when you enable this preference, future locked accounting periods display a lock ![Lock icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/lock.png) icon.

For instructions on how to lock and unlock accounting periods, see [Locking and Unlocking Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451780.html).

### Related Topics

-   [Rules for Future Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451349.html)
-   [Locking and Unlocking Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1451780.html)
-   [Locking Accounting Periods in NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452163.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
