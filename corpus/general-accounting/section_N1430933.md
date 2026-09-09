---
id: "section_N1430933"
type: "section"
title: "Revaluation Record Details"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Revaluation of Open Currency Balances > Generating Revaluations > Revaluation Record Details"
parent: "section_N1430227"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1430933.html"
anchors: []
sha256: "a3d9d10293cc58901a0b28b035a2eee54078413ef6a65ec6c9fc081421cbcc34"
---

The following information is available in the Details subtab for each unrealized gain/loss currency revaluation transaction at _Transactions > Financial > Revalue Open Currency Balances > List ( Administrator )_. You can also view this information from _Transactions > Financial > Revalue Open Currency Balances ( Administrator )_ after you run revaluation for a period. Click View in the Results column to view the information from the last time revaluation was run for an account.

-   For transactions included on the Open Receivables and Open Payables subtabs:
    
    -   **Type** - Type of transaction to be revalued, such as invoice or bill
        
    -   **Date** - Date of transaction
        
    -   **Payee** - Entity to receive payment or credit for the invoice
        
    -   **Currency** - Foreign currency used for the transaction
        
    -   **Transaction Exchange Rate** - Rate of the foreign currency to the base currency used on the transaction
        
    -   **Ending Exchange Rate** - Rate of the foreign currency to the base currency as of the last day of the posting period
        
    -   **Balance** - Foreign currency balance for open receivables or open payables as of the last day of the posting period. Any payments applied in the future periods are ignored.
        
    -   **Gain/Loss** - (Balance × Ending Exchange rate) - Base Currency Balance. To find the base currency balance, open the corresponding transaction. A positive number indicates a gain.
        
    -   **Prior Gain/Loss** - Accumulated gain/loss amount (in base currency) resulting from prior revaluations, as of the last day of the posting period
        
    -   **Net Gain/Loss** - Difference between Gain/Loss and Prior Gain/Loss (Gain/Loss - Prior Gain/Loss)
        
-   For lines shown on the Other Accounts subtab:
    
    -   **Account** - Name of the foreign currency account
        
    -   **Currency** - Foreign currency used for the account
        
    -   **Foreign Currency Balance** - Account balance denominated in foreign currency
        
    -   **Base Currency Balance** - Accumulated account balance in base currency based on historical transactions
        
    -   **Exchange Rate** - Rate of the foreign currency to the base currency as of the last day of the posting period
        
    -   **Net Gain/Loss** - (Foreign Currency Balance × Exchange Rate) - Base Currency Balance
        

### Related Topics

-   [Generating Revaluations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1430227.html)
-   [Foreign Currency Revaluation for Multiple Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4169300609.html)
-   [Classifications and Currency Revaluation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1430408.html)
-   [Viewing Revaluation Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1430727.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
