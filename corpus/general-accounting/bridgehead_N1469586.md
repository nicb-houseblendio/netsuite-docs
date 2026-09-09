---
id: "bridgehead_N1469586"
type: "bridgehead"
title: "Require Approvals on Journal Entries Preference"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Journal Entry Preferences > Require Approvals on Journal Entries Preference"
parent: "section_N1469391"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469586.html"
anchors: []
sha256: "0d9cd38db16d594cd9b031ba74bdacd43f6fe07be635ef6e41d94f99bb31f609"
---

You can require approval for journal entries before they're posted. Requiring approval establishes control over the accuracy and materiality of the journal entries in your ledgers.

To enable the Require Approvals on Journal Entries preference, go to _Setup > Accounting > Accounting Preferences_. On the General subtab in the General Ledger section, check the Require Approvals on Journal Entries box.

Note:

If you've enabled the **Journal Entries** approval routing preference and are using SuiteFlow for journal approval, the Require Approvals on Journal Entries preference won't appear.

For information about other journal entry approval options, see [Journal Entry Approval Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1471271.html).

After you enable this preference, a user with the Journal Approval permission (Edit level or higher) must approve each journal entry before it's posted. In addition, journal entry reversals will be approved when their corresponding journal entry is approved. A reversal won't be approved if its corresponding journal entry is also not approved.

By default, only Administrators have this permission. Administrators can add this permission to a customized role, permitting users with that role to approve journal entries. See [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html).

The following permission levels are required to perform actions with approved journals:

-   Users must have the **Edit** level of the Journal Approval permission to edit an approved journal.
    
-   Users must have the **Full** level of the Journal Approval permission to delete an approved journal.
    

### Related Topics

-   [Journal Entry Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469391.html)
-   [Void Transactions Using Reversing Journals Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469460.html)
-   [Reversing Journal Entry Accounting Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497536981.html)
-   [Use Journal Entry Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4643680489.html)
-   [Class, Department, Location Journal Entry Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469649.html)
-   [Revenue Recognition Journal Entry Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4041556974.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
