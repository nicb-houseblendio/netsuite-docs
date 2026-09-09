---
id: "bridgehead_N1432098"
type: "bridgehead"
title: "Revaluation in Reopened Periods"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Revaluation of Open Currency Balances > Revaluation Examples > Revaluation in Reopened Periods"
parent: "section_N1431203"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1432098.html"
anchors: []
sha256: "f62f6de0402c982d7d03151078a1015fc4b9f021235f65827872d5df230a2ad0"
---

In this example, after you've revalued and closed January, February, and March, you reopen January. You then post a journal that increases the balance of a British pounds **foreign currency account** for a U.S. based subsidiary. When you reopen January, the accounting periods of February and March are automatically reopened.

After posting the change to January, you must complete the revaluation for all three periods again to be able to re-close them. Revaluations for February and March take into account the posting change and the revaluation of previous periods. These revaluations adjust accounts accordingly, as if the new posting had been originally made before the first set of revaluations.

This example for foreign currency accounts includes the following details:

-   Initial transactions:
    
    |  | Foreign Currency Amount | Base Currency Amount | Exchange Rate |
    | --- | --- | --- | --- |
    | January Journal | £50 | $75 | 1.5 |
    | February Journal | £50 | $100 | 2.0 |
    | March Journal | £50 | $150 | 3.0 |
    
-   Initial period close revaluations:
    
    | Period | Foreign Currency Balance | Base Currency Balance | Exchange Rate | Net Gain/Loss |
    | --- | --- | --- | --- | --- |
    | January | £50 | $75 | 2.0 | $25 |
    | February | £100 | $175 | 3.0 | $125 |
    | March | £150 | $325 | 4.0 | $275 |
    
-   Account balances in foreign currency and base currency (cumulative), plus ending exchange rate, after period close:
    
    | Period | Foreign Currency Balance | Base Currency Balance | Ending Exchange Rate |
    | --- | --- | --- | --- |
    | January | £50 | $100 | 2.0 |
    | February | £100 | $300 | 3.0 |
    | March | £150 | $600 | 4.0 |
    

-   New transaction after reopening January, February, and March:
    
    |  | Foreign Currency Amount | Base Currency Amount | Exchange Rate |
    | --- | --- | --- | --- |
    | January Journal 2 | £50 | $100 | 2.0 |
    
-   Rerun Period Close Revaluations for all three periods.
    
    No new currency revaluation is created for January because the new journal has the same exchange rate as the period end. For the other periods, new currency revaluation transactions are created to account for the changed foreign currency balance.
    
    | Period | Foreign Currency Balance | Base Currency Balance | Exchange Rate | Net Gain/Loss |
    | --- | --- | --- | --- | --- |
    | January (initial only) | £50 | $75 | 2.0 | $25 |
    | February (initial) | £100 | $175 | 3.0 | $125 |
    | February (rerun) | £150 | $400 | 3.0 | $50 |
    | March (initial) | £150 | $325 | 4.0 | $275 |
    | March (rerun) | £200 | $700 | 4.0 | $100 |
    
-   Foreign currency account balance (cumulative) with new transaction and after revaluation is rerun:
    
    | Period | Foreign Currency Balance | Base Currency Balance | Ending Exchange Rate |
    | --- | --- | --- | --- |
    | January | £100 | $200 | 2.0 |
    | February | £150 | $450 | 3.0 |
    | March | £200 | $800 | 4.0 |
    

### Related Topics

-   [Revaluation Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1431203.html)
-   [Revaluation of Invoice with No Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1431303.html)
-   [Revaluation of Invoice with Partial Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1431690.html)
-   [Revaluation of Advanced Intercompany Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1436722.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
