---
id: "bridgehead_N1429362"
type: "bridgehead"
title: "Base Currency Adjustment Example"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Revaluation of Open Currency Balances > Types of Accounts That Can Be Revalued > Base Currency Adjustment Example"
parent: "section_N1428933"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1429362.html"
anchors: []
sha256: "df7992c5ffcce96a2ad7109374a535ce5e762de0bda8a93d5c2f437e7a4e76e6"
---

On March 20, a Canadian company issues a payroll advance to an employee in the United States. The Canadian to U.S. dollar exchange rate is 0.998.

**General Ledger Impact for Employee Advance on March 20**

|  | Transaction Currency U.S. Dollars | Base Currency Canadian Dollars |
| --- | --- | --- |
| Account | Debit | Credit | Debit | Credit |
| --- | --- | --- | --- | --- |
| Employee Advance | 2,000 |  | 1,996 |  |
| Accounts Payable |  | 2,000 |  | 1,996 |

On April 1, the employee advance account is reduced to 0 when payroll is recorded. The Canadian to U.S. dollar exchange rate is 0.992.

**General Ledger Impact for Employee Advance on April 1**

|  | Transaction Currency U.S. Dollars | Base Currency Canadian Dollars |
| --- | --- | --- |
| Account | Debit | Credit | Debit | Credit |
| --- | --- | --- | --- | --- |
| Payroll Expense | 2,000 |  | 1,984 |  |
| Employee Advance |  | 2,000 |  | 1,984 |

At the end of April, the transaction currency balance for Employee Advance is 0. However, due to the difference in exchange rates, the base currency account has a residual balance of 12.

Running currency revaluation at the end of April produces a base currency adjustment to clear the residual balance in the Employee Advance account.

**General Ledger Impact for Employee Advance at End of April**

|  | Base Currency |
| --- | --- |
| Account | Debit | Credit |
| --- | --- | --- |
| Matching Unrealized Gain/Loss | 12 |  |
| Employee Advance |  | 12 |

At this point, the transaction currency and base currency balances for the Employee Advance account are 0, and further currency revaluation isn't triggered for this account.

### Related Topics

-   [Types of Accounts That Can Be Revalued](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1428933.html)
-   [Residual Base Currency Balances and Base Currency Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1429248.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
