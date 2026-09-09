---
id: "bridgehead_N1488569"
type: "bridgehead"
title: "Equity, Income Statement, and Inventory Accounts"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Setting Up Automated Intercompany Management > Account Types and Intercompany Transactions > Equity, Income Statement, and Inventory Accounts"
parent: "section_N1487157"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1488569.html"
anchors: []
sha256: "4acd4f5da6d6041332a90ed17219024587f5f76f3af6adf4f45729fa4d7a531f"
---

You can set up intercompany accounts for this group of account types. Transactions posted to these accounts can be candidates for intercompany elimination. When set up as intercompany accounts, these accounts do not have to be used exclusively for intercompany transactions. Check the **Eliminate Intercompany Transactions** box for all income and expense accounts associated with items used in intercompany transactions. If you do not check this box, transactions with those items are not candidates for elimination.

Open balances for foreign currency transactions posted to these accounts are never revalued.

Inventory accounts, created by checking the **Inventory** box for an Other Current Asset account belong to this group. However, you should use advanced intercompany journal entries to record intercompany inventory transfers. For information about advanced intercompany journal entries, see [Making Advanced Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4803443925.html).

Important:

The purpose of reversing intercompany elimination journals is to ensure that changes in balance sheet valuations are accurately reflected during the elimination process. This applies specifically to accounts that are periodically revalued using the current exchange rate. In contrast, equity accounts are valued using the historical consolidated exchange rate. They are not subject to periodic revaluation. Therefore, there is no need to reverse the elimination on a periodic basis because fluctuations in currency exchange rates do not impact these accounts. Instead, eliminating the transaction in the period it occurred is sufficient because no subsequent changes arise from currency fluctuations in future periods.

| Account Type | Eliminate Intercompany Transactions | Restricted to Intercompany Transactions | Reverse Elimination Automatically | Revalue Foreign Currency Open Balances |
| --- | --- | --- | --- | --- |
| Equity | Yes | No | No | Never |
| Income | Yes | No | No | Never |
| Other Income | Yes | No | No | Never |
| Expense | Yes | No | No | Never |
| Other Expense | Yes | No | No | Never |
| Cost of Goods Sold (COGS) | Yes Important: For arm's length intercompany inventory transfer, do NOT mark the COGS account as Elimination. | No | No | Never |
| Other Current Asset - Inventory | Yes | No | No | Never |

### Related Topics:

-   [Accounts Receivable and Accounts Payable](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1487235.html)
-   [Balance Sheet Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1489083.html)
-   [Other Account Types and Exceptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1489533.html)
-   [Intercompany Accounts for Cross-Subsidiary Purchases and Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4308408763.html)
-   [Account Types and Intercompany Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1487157.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
