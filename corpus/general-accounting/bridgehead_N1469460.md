---
id: "bridgehead_N1469460"
type: "bridgehead"
title: "Void Transactions Using Reversing Journals Preference"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Journal Entry Preferences > Void Transactions Using Reversing Journals Preference"
parent: "section_N1469391"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469460.html"
anchors: []
sha256: "c70b03ad4d6e36fc016fd31be5919316a4a79a173dd0440726bcaae6457755c7"
---

Enable the Void Transactions Using Reversing Journals preference to permit the creation of journal entries that void transactions on days or periods different from the original transaction dates.

To enable this preference, go to _Setup > Accounting > Accounting Preferences_. On the General subtab in the General Ledger section, check the Void Transactions Using Reversing Journals box. After you enable this preference, a reversing journal entry is created when you click the Void button on the following transactions:

-   Bill Payment
    
-   Payroll Liability Payment
    
-   Customer Refund
    
-   Tax Payment
    
-   Tax Liability Check
    

Note:

When you enable this preference, journal entry forms won't display the Void button. Disable this preference to display the Void button when you edit journal entry forms.

Warning:

A check transaction cannot be voided by a reversing journal entry with Canadian taxes.

Clicking Void on the transaction opens a Voiding Journal form. The journal entry lines autofill to show the reverse of the original transaction. The Void Of field provides a link to the original transaction. For more information about voiding, see [Voiding, Deleting, or Closing Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N563543.html).

Saving the Voiding Journal form sets the status of the original transaction to Voided. Then, when you view the original transaction, the Voided On date provides a link to the voiding journal entry.

Be aware of the following conditions:

-   After you void a transaction, you can't make any changes that have general ledger impact to the original transaction including changing the posting period.
    
-   For bill payments, customer refunds, or payroll liability checks you void, any linked transactions are reopened. For example, if you void a bill payment, the bill it paid would have an Open status.
    

Important:

When you enable the Void Transactions Using Reversing Journals preference, you can no longer void the following transactions: sales order, estimate, cash sale, invoice, return authorization, cash refund, and credit memo.

### Related Topics

-   [Journal Entry Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469391.html)
-   [Reversing Journal Entry Accounting Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497536981.html)
-   [Require Approvals on Journal Entries Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469586.html)
-   [Use Journal Entry Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4643680489.html)
-   [Class, Department, Location Journal Entry Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469649.html)
-   [Revenue Recognition Journal Entry Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4041556974.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
