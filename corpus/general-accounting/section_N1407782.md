---
id: "section_N1407782"
type: "section"
title: "Consolidated Exchange Rates on Reports"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Consolidated Exchange Rates > Consolidated Exchange Rates on Reports"
parent: "section_N1404834"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1407782.html"
anchors: ["bridgehead_N1408509"]
sha256: "62c8251d6a9d0b792437b90dfc91727f5feaeb8565485935798a5bbf010fdc4c"
---

The value you select in the Subsidiary Context list for a report determines the data and currency to be used for amounts. The currency is the base currency of the subsidiary you select.

For consolidated reports that include data from multiple subsidiaries, NetSuite uses consolidated rates to convert from child subsidiary base currency to parent subsidiary base currency. For information about subsidiary context, see [Subsidiary Context for Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278946.html) and [Subsidiary Context for a Financial Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2123544.html).

If you use Multi-Book Accounting, you can run consolidated reports for any accounting book for which consolidation is enabled. Use the Accounting Book list to choose the primary accounting book or a secondary accounting book that corresponds to the selected subsidiary context.

For reports that include both budgeted and actual amounts, you can use two sets of exchange rates: budget and consolidated. You can set budget exchange rates from the Budget Exchange Rates list page at _Lists > Accounting > Budget Exchange Rates_. For information, see [Budget Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1508302.html) and [Subsidiary-Specific Budget Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2125541.html).

The following example describes how consolidated exchange rates are applied to a report.

**Scenario:**

-   A company headquartered in the U.S. has a subsidiary in the United Kingdom. The U.K. subsidiary has a child subsidiary in Germany. In this case, there are two parents. Both parents require rates from the German subsidiary to consolidate balances. Rates are also needed between the U.K. and U.S. subsidiaries.
    
-   The rates specified between the U.K. and U.S. are direct. The rates between Germany and the U.S. are indirect. To derive the indirect rate for the Euro (the German subsidiary's base currency) to the U.S. dollar, you would multiply the exchange rate for Euros to British pounds (GBP) by the rate for the GBP to the U.S. dollar.
    
-   The global controller runs a Purchases by Vendor Summary report for the consolidated U.S. subsidiary. The following purchases were made so far this year:
    
    | Vendor | Period | Subsidiary | Transactions |
    | --- | --- | --- | --- |
    | Vendor 1 | Period 1 | U.S. | 100 USD |
    | Vendor 2 | Period 1 | U.K. | 50 GBP |
    | Vendor 2 | Period 2 | U.K. | 50 GBP |
    | Vendor 3 | Period 1 | German | 200 EU |
    | Vendor 3 | Period 2 | German | 200 EU |
    | Vendor 3 | Period 3 | German | 200 EU |
    
-   The following consolidated exchange rates apply:
    
    | Period | From Subsidiary | To Subsidiary | Current Rate |
    | --- | --- | --- | --- |
    | Period 1 | U.K. | U.S. | 2.00 |
    | Period 1 | German | U.S. | 3.00 |
    | Period 2 | U.K. | U.S. | 2.00 |
    | Period 2 | German | U.S. | 2.40 |
    | Period 3 | German | U.S. | 2.10 |
    

**Results:**

The report for the global controller is generated in U.S. dollars. The vendors have the following totals:

-   Vendor 1: $100
    
-   Vendor 2: $200 = 50 × 2 + 50 × 2
    
-   Vendor 3: $1,500 = 200 × 3 + 200 × 2.4 + 200 × 2.1
    

## Consolidated Report Amounts vs. Subsidiary Report Amounts {#bridgehead_N1408509}

Because consolidated exchange rates are different from currency exchange rates, amounts from subsidiary-level reports often don't match consolidated reports. When you calculate the adjustment on a per-transaction basis, differences between orders of magnitude affect the results.

A reasonable average exchange rate usually doesn't result, for example, from consolidating all income statements across multiple periods. Thus, the net income in a yearly consolidated income statement may not match the net incomes in yearly subsidiary-level reports.

To get clarity on these differing amounts, you can:

-   Add the **Amount (Current Rate)** field to the report to see the values as calculated with only the current exchange rate across all transactions. You can then see a direct conversion of any item in the report from one exchange rate to another.
    
-   Add the **Translation Adjustment** field to the report to see the amount adjusted in a certain total.
    

Note:

Transaction saved searches that include values calculated based on consolidated exchange rates may not match the general ledger impact of these same transactions. The values in the saved search are translated to the base currency using the appropriate consolidated rate type for the account. The impact in the general ledger is posted using the currency exchange rate at the time of the transaction.

### Related Topics

-   [Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404834.html)
-   [Consolidated Exchange Rates vs. Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405239.html)
-   [Consolidated Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405625.html)
-   [Viewing Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405950.html)
-   [Editing Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1406714.html)
-   [Calculating Consolidated Exchange Rates Automatically](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1406908.html)
-   [Search for Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1408952.html)
-   [Consolidated Exchange Rate Types for Transaction Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1409190.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
