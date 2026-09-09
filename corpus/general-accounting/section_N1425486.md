---
id: "section_N1425486"
type: "section"
title: "Realized Exchange Rate Gains and Losses Report"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Accounting for Fluctuation in Exchange Rates for Closed Transactions > Realized Exchange Rate Gains and Losses Report"
parent: "section_N1425038"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425486.html"
anchors: []
sha256: "b77866b7a375cefe793d91a07e7149b59097611e35ead635375befc60346f331"
---

Use the Realized Exchange Rate Gains and Losses report to view the realized gain and loss by transaction for a period of time. The report presents each source transaction, the associated payment transaction, and the realized gain or loss for the transaction reported in the base currency. From the report you can drill down to the source invoice or vendor bill and the applied payment. From the transaction detail you can drill down to view the general ledger impact.

Use this report in your month-end process to provide an audit trail of the transactions with realized gain or loss for the period. The Realized Gain/Loss account is included as Other Expense on the Income Statement.

Note:

The exchange rates shown in this report are rounded to 2 decimal places. To view the complete exchange rate used to calculate the base currency amounts, drill down to the source transaction.

The Realized Exchange Rate Gains and Losses report lists transactions that have been closed and that posted a difference to the Realized Gain/Loss account. Only revaluation of currency amounts on paid transactions is reflected in this report.

This report groups transactions by Accounts Payable and Accounts Receivable, and then by entity name in alphabetical order. The transaction order within each entity name group is chronological by posting date for the realized gain/loss. The following columns are standard:

-   **Name** - Name of the entity (customer, vendor, or project)
    
-   **Subsidiary** - Subsidiary for the transaction
    
-   **Source Trans Number** - The number of the source transaction (invoice, vendor bill, or journal that functions as a bill or invoice). For vendor bills, the number shown is the reference number if the bill has one. If the bill doesn't have a reference number, the internal ID is displayed.
    
-   **Source Accounting Period** - Period in which the source transaction was posted
    
-   **Source Trans Date** - Date of the source transaction
    
-   **Source Trans Type** - Invoice, vendor bill, or journal that functions as a bill or invoice
    
-   **Source Account** - The account to which the source transaction posted
    
-   **Source Exchange Rate** - The exchange rate on the source transaction
    
-   **Pmt Trans Number** - The number of the payment transaction (bill payment, payment, credit memo, customer deposit, or journal applied as a payment)
    
-   **Pmt Accounting Period** - Period in which the payment transaction posted
    
-   **Pmt Trans Date** - Date of the payment transaction
    
-   **Pmt Trans Type** - Bill payment, payment, credit memo, customer deposit, or journal applied as a payment
    
-   **Pmt Exchange Rate** - The exchange rate on the payment transaction
    
-   **Transaction Currency** - The currency of the source and payment transactions
    
-   **Applied Amount** - The payment amount applied to the source transaction in the transaction currency
    
-   **Applied Amount (Base)** - The payment amount applied to the source transaction converted to the base currency using the payment exchange rate
    
-   **Realized Gain/Loss Trans Number** - The number of the transaction that includes the posting for realized gain or loss
    
-   **Realized Gain/Loss Posting Period** - Period in which the realized gain or loss posted
    
-   **Realized Gain/Loss Posting Date** - Date of the realized gain/loss transaction
    
-   **Realized Gain/Loss** - Amount of the realized gain or (loss) in the base currency
    

#### To see the Realized Exchange Rate Gains and Losses report:

1.  Go to _Reports > Financial > Realized Exchange Rate Gains and Losses ( Administrator )_.
    
2.  Adjust the values for **Period**, **From**, and **To** as needed.
    
3.  Use the following additional filters as needed:
    
    -   Use the **Subsidiary Context** filter if you want to filter the report by subsidiary.
        
    -   Use the **Accounting Book** filter if you're using multi-book accounting and have access to multiple accounting books.
        
4.  Click **Refresh** to apply your filters.
    
    A message appears indicating that your report is loading. The status bar indicates the progress as your report loads. Click Cancel Report to stop the report from loading.
    

### Related Topics

-   [Accounting for Fluctuation in Exchange Rates for Closed Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425038.html)
-   [Applied Payments and Realized Gain/Loss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425327.html)
-   [Rounding Gain/Loss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4030214366.html)
-   [Examples for the Realized Exchange Rate Gains and Losses Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1425819.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
