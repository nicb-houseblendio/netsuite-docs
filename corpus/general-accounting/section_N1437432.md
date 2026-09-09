---
id: "section_N1437432"
type: "section"
title: "Unrealized Exchange Rate Gains and Losses Report"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Revaluation of Open Currency Balances > Unrealized Exchange Rate Gains and Losses Report"
parent: "section_N1428662"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1437432.html"
anchors: []
sha256: "922c7b122de5f5e26cb22a729b0c1006390b403d0217e389c556a90e37d9f0bf"
---

Use the Unrealized Exchange Rate Gains and Losses report to view the unrealized gain and loss by transaction for a period of time. The report displays each source transaction and the unrealized gain or loss for the transaction reported in the base currency. From the report you can drill down to the source invoice or vendor bill. From the transaction detail you can drill down to view the general ledger impact.

Use this report in your month-end process to provide an audit trail of the transactions with unrealized gain or loss for the period. The Unrealized Gain/Loss account is included as Other Expense on the Income Statement.

The Unrealized Exchange Rate Gains and Losses report lists open receivables and open payables that post a change in value to the Unrealized Gain/Loss account. Currency revaluation transactions generated for any non-equity balance sheet account with a foreign currency balance are also reflected in this report.

This report groups transactions by account beginning with Accounts Payable and Accounts Receivable, followed by other non-equity balance sheet accounts with transactions subject to revaluation. Within the accounts, transactions are grouped by entity name. The entity names are in alphabetical order, and the transactions within each entity group are in chronological order. The following columns are standard:

-   **Name** - Name of the entity (customer, vendor, or project) for Accounts Payable and Accounts Receivable. Unassigned is displayed for other accounts.
    
-   **Subsidiary** - Subsidiary from the transaction.
    
-   **Source Trans Number** - (Accounts Payable and Accounts Receivable only) The number of the source transaction (invoice, vendor bill, or journal that functions as a bill or invoice). For vendor bills, the number shown is the reference number if the bill has one. If the bill doesn't have a reference number, the internal ID is displayed.
    
-   **Source Trans Date** - (Accounts Payable and Accounts Receivable only) Date of the source transaction.
    
-   **Source Trans Type** - (Accounts Payable and Accounts Receivable only) Invoice, vendor bill, or journal that functions as a bill or invoice.
    
-   **Unrealized Gain/Loss Posting Period** - Period in which the currency revaluation transaction posted.
    
-   **Source Exchange Rate** - This column is used differently depending on the type of account. All numbers are rounded to two decimal places.
    
    -   For Accounts Payable and Accounts Receivable, this number is the exchange rate on the source transaction.
        
    -   For other non-denominated accounts and foreign currency accounts, for reversal lines, this number is the exchange rate at the end of the previous period. For lines that aren't reversals, the placeholder 1.00 is used.
        
-   **Ending Exchange Rate** - This column is used differently depending on the type of account. All numbers are rounded to two decimal places.
    
    -   For Accounts Payable and Accounts Receivable, this number is the exchange rate at the end of the period. If the revaluation is run prior to the end of a period, the exchange rate with the latest effective date in the period is used.
        
    -   For other non-denominated accounts and foreign currency accounts, for reversal lines, the placeholder 1.00 is used. For lines that aren't reversals, this number is the exchange rate at the end of the period. If the revaluation is run prior to the end of a period, the exchange rate with the latest effective date in the period is used.
        
-   **Currency** - (Accounts Payable and Accounts Receivable only) The currency of the source transaction.
    
-   **Foreign Currency Balance** - The foreign currency balance used to determine the net gain or loss.
    
-   **Net Gain/Loss** - (Foreign Currency Balance × Ending Exchange rate) - Base Currency Balance. The exchange rates for the calculation are prior to rounding. To find the non-rounded exchange rates and the base currency balance, open the corresponding revaluation record.For reversals, this number is the amount required to reverse the currency revaluation transaction from the previous period. No calculation is performed.
    
-   **Unrealized Gain/Loss Trans Number** - The number of the currency revaluation transaction
    
-   **Base Amount (Opening)** - This column is used differently depending on the type of account.
    
    -   For Accounts Payable and Accounts Receivable, this number ties to the balance for the transaction prior to the Net Gain/Loss for the row.
        
    -   For reversals for other non-denominated accounts and foreign currency accounts, this number ties to the account balance at the end of the previous period. For rows other than reversals, this number is the same as the Foreign Currency Balance.
        
-   **Base Amount (Adjusted)** - This column is used differently depending on the type of account.
    
    -   For Accounts Payable and Accounts Receivable, this number equals Base Amount (Opening) + Net Gain/Loss.
        
    -   For reversals for other non-denominated accounts and foreign currency accounts, this number is the same as the Foreign Currency Balance. For rows other than reversals, this number equals Foreign Currency Balance × Ending Exchange Rate.
        
-   **Reversal** - Reversal is displayed when the transaction line is the reversal of the prior period's currency revaluation transaction.
    

#### To see the Unrealized Exchange Rate Gains and Losses report:

1.  Go to _Reports > Financial > Unrealized Exchange Rate Gains and Losses ( Administrator )_.
    
2.  Adjust the values for **Period**, **From**, and **To** as needed.
    
3.  Use the following additional filters as needed:
    
    -   Use the **Subsidiary Context** filter if you want to filter the report by subsidiary.
        
    -   Use the **Accounting Book** filter if you're using multi-book accounting and have access to multiple accounting books.
        
4.  Click **Refresh** to apply your filters.
    
    A message appears indicating that your report is loading. The status bar indicates the progress as your report loads. Click Cancel Report to stop the report from loading.
    

### Related Topics

-   [Revaluation of Open Currency Balances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1428662.html)
-   [Types of Accounts That Can Be Revalued](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1428933.html)
-   [Generating Revaluations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1430227.html)
-   [Revaluation Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1431203.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
