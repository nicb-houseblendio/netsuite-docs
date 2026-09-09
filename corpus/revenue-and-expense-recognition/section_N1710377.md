---
id: "section_N1710377"
type: "section"
title: "VSOE with Foreign Currency Revenue Commitment Example"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments > Revenue Commitment Examples > VSOE with Foreign Currency Revenue Commitment Example"
parent: "section_N1710191"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1710377.html"
anchors: []
sha256: "1bca3b564b05db22a423a73d3896c34172112497c50739d2e3a271a3f35557e7"
---

Important:

The functions discussed in this topic require the Revenue Commitments feature to be enabled.

This example shows the revenue commitments process as of Version 2012 Release 2.

In this scenario, you have a sales order transacted in foreign currency. The lines of the order have different revenue recognition schedules, and vendor-specific objective evidence (VSOE) applies. The transaction currency is GBP and the base currency is USD.

The sales order has the following item details:

| Sales Order | Price | VSOE | Allocation | Recognition Schedule | Deferred Revenue Account | Revenue Account |
| --- | --- | --- | --- | --- | --- | --- |
| Line 1 | GBP 180 | GBP 100 | GBP 120 | 3 month | DR 1 | Rev 1 |
| Line 2 | GBP 60 | GBP 100 | GBP 120 | 2 month | DR 2 | Rev 2 |

The revenue commitment for the full sales order amount is created on January 10 and the exchange rate is 1.5 USD/GBP.

The order is billed in arrears based on milestones and billing generates 3 invoices.

All amounts shown are accumulated amounts as of that period. The rate of billing compared to rate of revenue recognition is calculated for the order total, not separately for each line item. Foreign currency translation amounts are rounded.

The following tables show how the amounts are calculated for the foreign currency revenue adjustment, and amounts for deferred revenue, revenue and unbilled receivables. They also show the GL impact for each month when revenue reclassification is run.

For each month, the FX adjustment amount is the amount required to adjust the previous month's FX adjustment to the current gain/loss amount.

This table shows how the amounts posted to the deferred revenue, revenue, and unbilled receivable accounts are determined. At the end of April the sales order is fully billed and recognized. The combined balance for the deferred revenue accounts and the balance for the unbilled receivable account for the order are 0, and $380 is posted to the revenue accounts.

| Invoice | Total Amt | Total Amt | Billing FX Rate | Total G/L | Deferred Revenue Accounts | Revenue Accounts | Un- billed Receivable |
| --- | --- | --- | --- | --- | --- | --- | --- |
|  | Trans | Base |  |  | DR 1 | DR 2 | DR | Rev 1 | Rev 2 | Rev |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Jan | £60 | $120 | 2 USD/GBP | $ 30 | $ 60 | $ (90) | $ 30 | $ 60 | $ 90 | $ 30 | $ 60 |
| Feb | £240 | $280 | 1 USD/GBP | $ 45.45 | $ 100 | $(120) | $ 45.45 | $120 | $180 | $ (45.45) | \- |
| Mar | £240 | $280 | No bill | $ 50 | $ 40 | $(120) | $ 80 | $180 | $180 | $ (50) | $30 |
| Apr | £240 | $380 | 5 USD/GBP | $ 20 | $140 | $(120) | $(20) | $180 | $180 | $ 20 | \- |

This table shows the G/L impact for the foreign currency revenue adjustment and revenue reclassification journal entries:

| Invoice | Total Rev Rec Amt | Total Rev Rec Base Currency | Total Billed Amount | Total Billed Base Curr | Total Gain/Loss | FX Adjustment | Reclassification |
| --- | --- | --- | --- | --- | --- | --- | --- |
| **Jan** |  | **First bill, 2 USD/GBP** |  | **$ 30** |  |  |
| Line 1 | £ 40 | $ 60 | £ 60 | $ 120 |  | Dr Def Rev $ 30 Cr Rev $ 30 | Dr UNAR $ 60 Cr Def Rev $ 60 |
| Line 2 | £ 60 | $ 90 | \- | \- |  |
| **Feb** |  | **Second bill, 1USD/GBP** | **$ (45.45)** |  |  |
| Line 1 | £ 80 | $ 120 | £ 160 | $ 220 |  | Dr Rev $ 60 Cr Def Rev $ 60 | Dr Def Rev$ 60 Cr UNAR $ 60 |
| Line 2 | £ 120 | $ 180 | £ 60 | $ 60 |  |
| **Mar** |  | **No bill** |  |  | **$ (50)** |  |  |
| Line 1 | £ 120 | $ 180 | £ 160 | $ 220 |  | Dr Rev $ 4.54 Cr Def Rev $ 4.54 | Dr UNAR $ 30 Cr Def Rev $ 30 |
| Line 2 | £ 120 | $ 180 | £ 60 | $ 60 |  |
| **Apr** |  | **Last bill, 5 USD/GBP** |  | **$ 20** |  |  |
| Line 1 | £120 | $ 180 | £180 | $ 320 |  | Dr Def Rev $ 70 Cr Rev $ 70 | Dr Def Rev$ 30 Cr UNAR $ 30 |
| Line 2 | £ 120 | $ 180 | £ 60 | $ 60 |  |

### Related Topics

-   [Revenue Commitment Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1710191.html)
-   [Base Currency Transaction Without Revenue Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3811804072.html)
-   [Base Currency Transaction with Revenue Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3811804909.html)
-   [Foreign Currency Transaction with Revenue Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3811805482.html)
-   [Revenue Commitment with One-Time Revenue Item Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1712809.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
