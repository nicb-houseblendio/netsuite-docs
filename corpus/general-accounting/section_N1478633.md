---
id: "section_N1478633"
type: "section"
title: "Example Intercompany Adjustment Scenario"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Journal Entries in OneWorld > Enabling Intercompany Time and Expenses > Example Intercompany Adjustment Scenario"
parent: "section_N1476983"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1478633.html"
anchors: []
sha256: "9e0f6fbf8eccd46b638daff8455a81170e971973e4fb1879df10e885e2226572"
---

This example occurs in an account where the Intercompany Time and Expense feature is enabled and the Intercompany Expenses accounting preference is set to Allow and Auto Adjust.

Important:

When NetSuite released the Intercompany Time and Expenses feature, the first set of accounts created were named Intercompany Payable/Receivable XXX, where XXX denoted the currency ISO code. In a later release, NetSuite OneWorld introduced the Intercompany Clearing XXX account. This new account replaced the Intercompany Payable/Receivable Account for new accounts because the existing accounts were being used by the Intercompany Elimination feature. The change applied to only new accounts. Existing accounts were not renamed. Still later, NetSuite OneWorld introduced new intercompany clearing accounts for payable and receivable that aren't currency locked. These new clearing accounts are used for intercompany transactions. All existing currency-locked intercompany clearing accounts (the Intercompany Payable/Receivable accounts) are now child accounts of the new clearing account. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html) and [Intercompany Elimination Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html).

**Background**

Sara Peters, an employee assigned to the U.S. based subsidiary of this account provides consulting services to FinCo. Finco is a U.K. based customer associated with the U.K. subsidiary.

**Original Expense Report**

Sara Peters incurs the following billable expenses recorded in U.S. dollars and records them in an expense report transaction. These expenses are cross-subsidiary. They were incurred by an employee of the U.S. subsidiary during the time in which the employee worked for a customer of the U.K. subsidiary.

| Employee | Employee Subsidiary | Expense Category | Memo | Amount | Currency | Customer | Customer Subsidiary |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Sara Peters | U.S. | Travel | RT Airfare NY-London | 1,600.00 | USD | FinCo | U.K. |
| Sara Peters | U.S. | Lodging | 2 nts Hyatt | 800.00 | USD | FinCo | U.K. |
| Sara Peters | U.S. | Meals | 3 days | 600.00 | USD | FinCo | U.K. |

**Expense Report GL Impact**

After the expense report is approved by Accounting, the following amounts are posted to U.S. subsidiary accounts:

| Account | Amount (Debited) | Amount (Credited) | Name | Subsidiary |
| --- | --- | --- | --- | --- |
| Accounts Payable |  | 3,000.00 | Sarah Peters | U.S. |
| Travel | 1,600.00 |  | FinCo | U.S. |
| Lodging | 800.00 |  | FinCo | U.S. |
| Meals | 600.00 |  | FinCo | U.S. |

**Automated Intercompany Adjustment**

As part of the period close process in which the expenses occurred, the controller generates automated adjustments to transfer the impact of intercompany expenses. An adjustment with the following lines is generated, all amounts in U.S. dollars:

| Subsidiary | Account | Amount (Debited) | Amount (Credited) | Name |
| --- | --- | --- | --- | --- |
| U.S. | Intercompany Clearing USD | 1,600.00 |  |  |
| U.S. | Travel |  | 1,600.00 | FinCo |
| U.K. | Travel | 1,600.00 |  | FinCo |
| U.K. | Intercompany Clearing USD |  | 1,600.00 |  |
| U.S. | Intercompany Clearing USD | 800.00 |  |  |
| U.S. | Lodging |  | 800.00 | FinCo |
| U.K. | Lodging | 800.00 |  | FinCo |
| U.K. | Intercompany Clearing USD |  | 800.00 |  |
| U.S. | Intercompany Clearing USD | 600.00 |  |  |
| U.S. | Meals |  | 600.00 | FinCo |
| U.K. | Meals | 600.00 |  | FinCo |
| U.K. | Intercompany Clearing USD |  | 600.00 |  |

**Automated Adjustment GL Impact**

The following lines illustrate the automated adjustment's general ledger impact on U.S. and U.K. subsidiary accounts:

An exchange rate specified on the adjustment record translates the general ledger impact for the U.K. subsidiary from the U.S. subsidiary base currency (USD) to the U.K. subsidiary base currency (GBP). This rate is based on the last day of the period in which the adjustment occurred. In this example, it's 0.51056877.

| Account | Amount (Debited) | Amount (Credited) | Name | Subsidiary |
| --- | --- | --- | --- | --- |
| Intercompany Clearing USD | 1,600.00 |  |  | U.S. |
| Travel |  | 1,600.00 | FinCo | U.S. |
| Travel | 816.91 |  | FinCo | U.K. |
| Intercompany Clearing USD |  | 816.91 |  | U.K. |
| Intercompany Clearing USD | 800.00 |  |  | U.S. |
| Lodging |  | 800.00 | FinCo | U.S. |
| Lodging | 408.46 |  | FinCo | U.K. |
| Intercompany Clearing USD |  | 408.46 |  | U.K. |
| Intercompany Clearing USD | 600.00 |  |  | U.S. |
| Meals |  | 600.00 |  | U.S. |
| Meals | 306.34 |  |  | U.K. |
| Intercompany Clearing USD |  | 306.34 |  | U.K. |

### Related Topics:

-   [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html)
-   [Intercompany Clearing Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1477786.html)
-   [Creating Intercompany Adjustments for Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1478200.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
