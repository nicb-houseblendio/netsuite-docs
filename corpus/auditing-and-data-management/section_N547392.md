---
id: "section_N547392"
type: "section"
title: "Using Auto-Generated Numbering for Transactions"
branch: "auditing-and-data-management"
category: "account-administration"
breadcrumb: "Account Administration > Auditing and Data Management > Avoiding Duplicates > Using Auto-Generated Numbering for Transactions"
parent: "chapter_4470654298"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N547392.html"
anchors: ["procedure_N547416"]
sha256: "0c3504c85f3bb73d4b1f846907421bf04fbcc47a5374ab0fb8769cfc5f5dcf73"
---

When enabled, the auto-generated numbering feature prevents assigning duplicate numbers to transactions in NetSuite. This ensures that the number can't be edited and can't be duplicated. Auto-generated numbering for transactions is enabled by default and can't be disabled. For information about this feature, see [Set Auto-Generated Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N252198.html).

#### To have transaction numbers generated when forms are saved: {#procedure_N547416}

1.  An administrator can go to _Setup > Company > Auto-Generated Numbers_.
    
2.  Click the **Transactions** subtab.
    
3.  To ensure that no duplicate transaction numbers are used, clear the box in the **Allow Override** column for each transaction.
    
4.  Click **Save**.
    
    When you create a transaction, the number field reads **To be generated**. When you return to the transaction, the generated number shows in this field. For example, if you create an invoice, the Invoice # field reads **To be generated**. When you save the invoice, a number is assigned. If you return to the invoice at _Transactions > Sales > Create Invoices > List_, you can view the number for the invoice.
    

Warning:

You can't auto-generate numbers for journals if you enable the Always Allow Per-line Classifications on Journals preference.

Warning:

You should never override auto-generated numbers to delete any part of a default prefix or suffix on transaction numbers. Doing this may damage data used in transaction searches.

Important:

In a OneWorld account with auto-generated numbering, you can define subsidiary-specific prefixes for transaction numbers in subsidiary records. This ensures each subsidiary's transaction has its own numbering sequence. See [Using Subsidiary-Specific Transaction Auto-Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N275081.html).

### Related Topics

-   [Avoiding Duplicates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4470654298.html)
-   [Avoiding Duplicate Transaction Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N546911.html)
-   [Duplicate Number Warnings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N547300.html)
-   [Avoiding Duplicate Processing of Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4431121865.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
