---
id: "section_N1471271"
type: "section"
title: "Journal Entry Approval Overview"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Journal Entry Approval Overview"
parent: "chapter_N1468455"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1471271.html"
anchors: []
sha256: "3a66a172941908f7b796c0d5aed230d8607c422df437c23d3bc1f0b8c42fe3e7"
---

NetSuite provides two journal entry approval accounting preferences.

-   **Journal Entries** - This accounting preference is on the **Approval Routing** subtab of the Accounting Preferences page. When the **Journal Entries** box is checked, a workflow for journal entry approval handles approval routing. The workflow may be a custom SuiteFlow or a SuiteApproval workflow. Workflows for journal entry approval don't use the Journal Approval permission to determine who can approve the journal entries. For more information about these options, see [Using SuiteFlow for Journal Entry Approvals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4643662034.html) and [SuiteApprovals SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_161589014381.html).
    
    Note:
    
    If you enable Approval Routing for journal entries, you can only approve 25 journal entries at a time.
    
    If you use the Advanced Revenue Management (Essentials) feature, create a custom form for your system-generated revenue recognition and reclassification journal entries and exclude it from your workflows. Select the custom form in the accounting preferences Default Revenue Recognition Journal Entry Form and Default Reclassification Journal Entry Form.
    
-   **Require Approvals on Journal Entries** - This accounting preference is on the **General** subtab of the Accounting Preferences page in the General Ledger section. When this preference is checked, journal entry approval is required before posting to your general ledger account. Someone with Journal Approval (Edit or Full) permission must approve a journal entry before the entry posts to your general ledger. If you have this Journal Approval permission, you can approve your own journal entries when entering them. For more information about this preference, see [Require Approvals on Journal Entries Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469586.html).
    
    The following permission levels are required to create, edit, or delete approved journals:
    
    -   Users must have the **Edit** level of the Journal Approval permission to edit an approved journal.
        
    -   Users must have the **Full** level of the Journal Approval permission to delete an approved journal.
        
    
    Note:
    
    With this preference enabled, journal entry reversals are approved when their corresponding journal entry is approved. A reversal won't be approved if its corresponding journal entry is also not approved. For more on approving reversals and their journal entries, see [Reversing Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1471552.html).
    

Journal entry transactions aren't posted until they're approved. You can select a posting period for a journal entry that is pending approval. You can't select a closed period. You can select an open and locked period only if your role includes the **Override Period Restrictions** permission.

You can unapprove an approved journal entry by editing the journal record and clearing the Approved box. Don't clear the Approved box if the journal entry is linked to a payment transaction. You must unapply the payment before you clear the Approved box.

For more information about approving journal entries, see [Approving Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163164516146.html).

### Related Topics

-   [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html)
-   [Journal Entries Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1468996.html)
-   [Journal Entry Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469391.html)
-   [Making Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469880.html)
-   [Reversing Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1471552.html)
-   [Viewing Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472027.html)
-   [Printing Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472381.html)
-   [Importing a Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472877.html)
-   [Journal Entries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475513.html)
-   [Bad Debt Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1481280.html)
-   [Writing Off Customer Overpayments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483085.html)
-   [Expense Allocation Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483457.html)
-   [Period End Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1531269686.html)
-   [Balancing Segments and Journals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157358611227.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
