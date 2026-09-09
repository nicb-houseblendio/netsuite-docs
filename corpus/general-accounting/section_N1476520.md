---
id: "section_N1476520"
type: "section"
title: "Example of Intercompany Journal Entries"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Journal Entries in OneWorld > Making Intercompany Journal Entries > Example of Intercompany Journal Entries"
parent: "section_N1475891"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476520.html"
anchors: []
sha256: "a3db826265d8eb85496156676391ea1c1f3b5a0ae4e6c9416dec0a70b9037bef"
---

Note:

As of 2018.1, advanced intercompany journal entries replace legacy intercompany journal entries in new OneWorld accounts. For information, see [Making Advanced Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4803443925.html). This example is valid for both advanced and legacy intercompany journal entries.

The following journal entry records revenue for a sale from a U.S. subsidiary to a U.K. subsidiary:

| **Subsidiary** | Account | **Debit** | **Credit** |
| --- | --- | --- | --- |
| Wolfe U.S. | Intercompany Receivable | $100 |  |
| Wolfe U.S. | Sales |  | $100 |
| Wolfe U.K. | Intercompany Payable |  | $100 |
| Wolfe U.K. | Inventory | $100 |  |

Because the U.K. subsidiary uses British pounds (GBP) as its base currency, NetSuite revalues the transaction before posting it to the U.K. subsidiary's ledger. For this reason, from the perspective of the U.K. subsidiary, the general ledger impact of this transaction would show the revalued transaction in GBP, not U.S. dollars. This means the general ledger impact for Wolfe U.S. and Wolfe U.K. can differ.

To post an intercompany journal entry, the total debits and credits must balance by subsidiary for every transaction. Debit and credit amounts between subsidiaries can be different. When saving the intercompany journal entry in this case, NetSuite alerts you that the journal entry doesn't balance between subsidiaries. Click OK to save the journal entry.

In addition, to maintain balance in consolidated financials, you need to create elimination journal entries to reverse the effects of the intercompany transactions. With the Automated Intercompany Elimination feature enabled, elimination journal entries are automatically generated as part of the period close process. See [Automated Intercompany Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486393.html).

For instructions for making an intercompany journal entry, see [Making Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475891.html). For general information about OneWorld journal entries, see [Journal Entries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475513.html).

### Related Topics:

-   [Making Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475891.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
