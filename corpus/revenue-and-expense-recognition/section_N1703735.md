---
id: "section_N1703735"
type: "section"
title: "Advanced Revenue Commitments Overview"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments > Advanced Revenue Commitments Overview"
parent: "chapter_N1701780"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1703735.html"
anchors: []
sha256: "63fdcadc217914178761e95493998ad0fcd6aeca65629cb6a9bc92d44964b3d1"
---

Important:

The functions discussed in this topic require the Revenue Commitments feature to be enabled.

With revenue commitments, billing a sales order and recognizing the revenue from that sale can happen at different times and at different exchange rates if multiple currencies are involved. The relationship of the timing of billing and revenue recognition determines the impact on the general ledger during the order's life cycle. At the end of the order's life cycle, the order is fully billed, income is fully recognized, and the balances for the unbilled receivable account and deferred revenue account are zero. Before that point, the account balances for unbilled receivables and deferred revenue are determined by the rate at which the billing and revenue recognition has occurred.

-   **Billing rate slower than revenue recognition rate:** If the total revenue recognized for a sales order exceeds the total amount billed, then the excess revenue recognition amount generates a positive unbilled receivables balance. All amounts are compared in base currency and the excess revenue posts to the unbilled receivable account.
    
-   **Billing rate faster than revenue recognition rate:** If the total amount billed for an order exceeds the total revenue recognized, then the exceeding billing amount generates a positive deferred revenue balance. All amounts are compared in base currency and the excess billing posts to the deferred revenue account.
    

Note:

The revenue commitment is a non-posting transaction. It serves as the placeholder for the revenue recognition schedule that generates the posting revenue recognition journal entries.

In addition, if foreign currency rates differ at the time of billing and revenue recognition, an adjustment is required at the end of each accounting period to align the revenue recognition exchange rate with the effective billing exchange rate. The excess amount of foreign currency gain or loss for the overlapping portion of the billed and recognized amounts for the transaction posts directly to the revenue account.

For more information about the revenue commitments process, see:

-   [Life Cycle for Sales Order with Revenue Commitment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1703982.html)
    
-   [Calculating Foreign Currency Adjustment for Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1704597.html)
    
-   [Billing Additional Items on Orders with Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1706812.html)
    

### Related Topics

-   [Using Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1701780.html)
-   [Setting Up the Revenue Commitments Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1702000.html)
-   [Revenue Commitments Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1703512.html)
-   [Creating Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707026.html)
-   [Creating Revenue Recognition Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707738.html)
-   [Reclassifying Deferred Revenue for Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707946.html)
-   [Creating Revenue Commitment Reversals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1709562.html)
-   [Revenue Commitment Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1710191.html)
-   [Revenue Reclassification Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1717186.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
