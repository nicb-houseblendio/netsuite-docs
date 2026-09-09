---
id: "section_N1703982"
type: "section"
title: "Life Cycle for Sales Order with Revenue Commitment"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments > Advanced Revenue Commitments Overview > Life Cycle for Sales Order with Revenue Commitment"
parent: "section_N1703735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1703982.html"
anchors: []
sha256: "564944316f7a6b37f668085135c6b8b164b0ab1c7cd16064a406e47ecbc1d787"
---

Important:

The functions discussed in this topic require the Revenue Commitments feature to be enabled.

This example illustrates how Deferred Revenue and Unbilled Receivables account balances are affected by revenue reclassification, based on the rate of billing and revenue recognition activity.

-   **Total Billing < Total Revenue Recognition** - creates positive unbilled receivable and zero deferred revenue posting
    
-   **Total Billing > Total Revenue Recognition** - creates positive deferred revenue posting and zero unbilled receivable posting
    

A sales order is created for $1,200. Revenue is recognized quarterly based on the milestones completed. The customer is billed quarterly in equal amounts of $300. The following table shows the billing and revenue recognition postings for the order:

| Activity | Q1 | Q2 | Q3 | Q4 |
| --- | --- | --- | --- | --- |
| Revenue Recognition | $400 | $450 | $800 | $1200 |
| Billing | $300 | $600 | $900 | $1200 |
| Billing to Revenue Recognition Ratio | < | \> | \> | \> |

The account balances for Deferred Revenue and Unbilled Receivables for each quarter are shown in the following table. When the order is fully billed and the revenue recognized in full at the end of Q4, the account balances for Deferred Revenue and Unbilled Receivables are both 0.

| Account | Q1 | Q2 | Q3 | Q4 |
| --- | --- | --- | --- | --- |
| Deferred Revenue | 0 | 150 | 100 | 0 |
| Unbilled Receivable | 100 | 0 | 0 | 0 |

All amounts are accumulated balances and are calculated at the sales order level. If a sales order has multiple line items that follow different revenue recognition and billing schedules, revenue reclassification calculates a single combined amount for Deferred Revenue or Unbilled Receivable. If order lines use different deferred revenue and revenue accounts, the reclassification process uses the accounts specified on the sales order for the Deferred Revenue Reclassification Account, and Foreign Currency Adjustment Revenue Account, if multiple currencies are involved. For information about creating reclassification journal entries, see [Reclassifying Deferred Revenue for Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707946.html).

### Related Topics

-   [Advanced Revenue Commitments Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1703735.html)
-   [Calculating Foreign Currency Adjustment for Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1704597.html)
-   [Line Level Deferred Revenue Reclassification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3752066884.html)
-   [Adopting Line Level Deferred Revenue Reclassification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3758129615.html)
-   [Billing Additional Items on Orders with Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1706812.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
