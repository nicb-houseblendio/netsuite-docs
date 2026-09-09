---
id: "section_N1477786"
type: "section"
title: "Intercompany Clearing Account"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Journal Entries in OneWorld > Enabling Intercompany Time and Expenses > Intercompany Clearing Account"
parent: "section_N1476983"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1477786.html"
anchors: []
sha256: "45bd092684bb188f0987ebc50f8889f849f332278d3bf57517065dd580f74be9"
---

The Intercompany Time and Expense feature enables the transfer of time, expense, or both charges from one subsidiary to another. If this feature is enabled in your account, an intercompany clearing account is automatically created when the first intercompany transaction occurs. The intercompany clearing account is used to offset the transfer of expenses from the originating subsidiary (employee's subsidiary) to the related subsidiary (customer's subsidiary). This system-generated account enables the balancing of debits and credits in each subsidiary.

Note that when you enable this feature, the intercompany clearing account prevents you from modifying the subsidiaries associated with all account types except Bank.

This is an account of the Other Current Asset type. By default, it doesn't have an account number. You can change the name. You can't make other changes, merge, delete, or inactivate the intercompany clearing account. You can't create other accounts of this type.

Important:

When NetSuite released the Intercompany Time and Expenses feature, the first set of accounts created were named Intercompany Payable/Receivable XXX, where XXX denoted the currency ISO code. In a later release, NetSuite OneWorld introduced the Intercompany Clearing XXX account. This new account replaced the Intercompany Payable/Receivable Account for new accounts because the existing accounts were being used by the Intercompany Elimination feature. The change applied to only new accounts. Existing accounts were not renamed. Still later, NetSuite OneWorld introduced new intercompany clearing accounts for payable and receivable that aren't currency locked. These new clearing accounts are used for intercompany transactions. All existing currency-locked intercompany clearing accounts (the Intercompany Payable/Receivable accounts) are now child accounts of the new clearing account. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html) and [Intercompany Elimination Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html).

The intercompany account associated with a subsidiary is used for transactions where that subsidiary is the originating subsidiary. This ensures that adjusting journal entries are all in the base currency of the originating subsidiary. For example, the following intercompany adjustment journal entries illustrate the transfer of expenses entered by a Canadian employee working for a U.K. customer, to be charged to the U.K. subsidiary:

| Subsidiary | Account | Debit | Credit |
| --- | --- | --- | --- |
| Canadian Subsidiary | Intercompany Clearing CA Dollars | 3,395.24 |  |
| Canadian Subsidiary | Expense Account |  | 3,395.24 |
| U.K. Subsidiary | Expense Account | 3,395.24 |  |
| U.K. Subsidiary | Intercompany Clearing CA Dollars |  | 3,395.24 |

Automated intercompany adjustments use Intercompany Clearing accounts. See [Creating Intercompany Adjustments for Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1478200.html).

You also can use Intercompany Clearing accounts in journal entries you create to manually adjust for intercompany time or expenses.

If an account already exists with the default name used by a system-generated intercompany payable/receivable account, the system generates a new account. It also appends a number to the name so that it's unique.

### Related Topics

-   [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html)
-   [Creating Intercompany Adjustments for Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1478200.html)
-   [Example Intercompany Adjustment Scenario](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1478633.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
