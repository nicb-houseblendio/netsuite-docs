---
id: "bridgehead_N1469122"
type: "bridgehead"
title: "Journal Entry Approval"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Journal Entries Overview > Journal Entry Approval"
parent: "section_N1468996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469122.html"
anchors: ["subsect_156814648049"]
sha256: "2679bd97ba23cb1eb6d126a4ab4c516950300aa78a64e1af6453450998784b0c"
---

You can set up an approval process for journal entries before they post to your general ledger. When you enable the Require Approvals on Journal Entries accounting preference, you require that journal entries are approved by employees with Administrator roles before they're posted to your ledger accounts. If the journal entry approval preference is enabled, journal entries entered by employees without approval permission must be approved before they post to your general ledger. Employees with approval permission can mark their own journal entries approved when entering them. For information about setting this preference, see [Journal Entry Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469391.html).

You can also use SuiteFlow to create a custom journal entry approval routing workflow. For details, see [Using SuiteFlow for Journal Entry Approvals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4643662034.html).

You can approve journal entries at _Transactions > Financial > Approve Journal Entries_. After journal entries are approved, they post to your general ledger. For more information, see [Journal Entry Approval Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1471271.html) and [Approving Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163164516146.html).

## Posting Period for Journal Entries Subject to Approval {#subsect_156814648049}

The Posting Period value shown for a journal entry that is pending approval is the selected posting period. When you edit a journal entry that is pending approval, NetSuite keeps the selected Posting Period and doesn't update it to match the transaction date. NetSuite may recalculate the Posting Period if the selected period is locked or closed.

The Posting Period value you see when a journal entry is **pending approval** depends on the selected period, the transaction date, your role, accounting preferences, and the status of the period as follows:

-   If the selected period is open and not locked, NetSuite saves that period.
    
-   If the selected period is open and locked, NetSuite saves that period only if your role includes the **Override Period Restrictions** permission.
    
-   If the selected period is open and locked and your role doesn't include the override permission, NetSuite recalculates the posting period.
    
-   You can't select a closed period. If the transaction date is in a closed period, the accounting preference **Default Posting Period When Transaction Date in Closed Periods** determines which period displays.
    

You can select a Posting Period for a journal entry that is pending approval or approved. You can't select a closed period. You can select an open and locked period only if your role includes the Override Period Restrictions permission.

When you save the approved journal entry, you may see warnings or errors, depending on the setting of the accounting preference, Allow Transaction Date Outside of Posting Period. For details, see [General Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html).

### Related Topics

-   [Journal Entries Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1468996.html)
-   [Approving Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163164516146.html)
-   [Specialized Types of Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1494510597.html)
-   [Manual Journal Entry Creation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469070.html)
-   [Journal Entry Reversal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469193.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
