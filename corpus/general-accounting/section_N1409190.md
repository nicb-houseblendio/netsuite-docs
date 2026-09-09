---
id: "section_N1409190"
type: "section"
title: "Consolidated Exchange Rate Types for Transaction Searches"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Consolidated Exchange Rates > Consolidated Exchange Rate Types for Transaction Searches"
parent: "section_N1404834"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1409190.html"
anchors: []
sha256: "a48b1bf63bfb945e53306b65eb5fe493ebc5c7b26f207f979328a7eb39650ec6"
---

You can select the type of consolidated exchange rate to apply to results for each transaction search. The consolidated exchange rate type you select applies to amount fields in base currency, such as Amount, Amount (Credit), and Amount (Debit).

The denomination of the base currency for base currency amounts depends on the search subsidiary context. All transactions are viewed from the perspective of a single subsidiary that may have other child subsidiaries under it. The subsidiary context depends on a combination of your subsidiary access and the subsidiaries of the transactions in your search results. Consequently, a base currency amount may not be in the currency of the subsidiary on the transaction.

The subsidiary context is the lowest level subsidiary in the subsidiary hierarchy that is a common parent to all the subsidiaries in the result set. If you're running a search and have limited subsidiary access, your result set includes only those subsidiaries to which you have access. For an example with a diagram, see [Currency for Multiple Subsidiary Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N279420.html).

By selecting the rate type for each search context, you can maintain consistency between search results and consolidated report data. This ensures that any custom KPIs and KPI scorecards based on transaction save searches align with financial reports.

Note:

Rate type selections apply only to custom KPIs based on saved searches, not to standard KPIs that are based on reports.

You can select the consolidated exchange rate type for transaction advanced searches and saved searches. The **Results** subtab for these searches includes a **Consolidated Exchange Rate** field with the following options:

-   **Average** - Uses the average consolidated exchange rate type between the transaction subsidiary and the context subsidiary for the period in which the transaction occurred.
    
-   **Current** - Uses the current consolidated exchange rate for the date or period selected to filter the search or custom KPI results, if any. Any date filter can determine the consolidated exchange rate applied to the amount fields, and the latest date takes precedence. If both a date and period are selected, the period takes precedence.
    
    If no period or date is selected, the current rate for the date you run the search or custom KPI is used.
    
-   **Historical** - Uses the historical consolidated exchange rate for the period in which the transaction occurred.
    
-   **Per-Account** - Uses the general rate type selected for each transaction's account, either average, current, or historical.
    
    This option is the default. With this option, different consolidated exchange rate types may be used within each set of search results.
    
-   **None** - Uses the transaction subsidiary's base currency. No consolidation occurs. Translation to the subsidiary's base currency uses the transaction currency exchange rate.
    

Note:

Transaction saved searches that include values calculated based on consolidated exchange rates may not match the general ledger impact of these same transactions. The values in the saved search are translated to the base currency using the selected consolidated rate type. The impact in the general ledger is posted using the currency exchange rate on the transaction. Consolidated exchange rates ensure that currency amounts translate properly from child to parent subsidiaries for consolidated reports.

### Related Topics

-   [Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404834.html)
-   [Consolidated Exchange Rates vs. Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405239.html)
-   [Consolidated Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405625.html)
-   [Viewing Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405950.html)
-   [Editing Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1406714.html)
-   [Calculating Consolidated Exchange Rates Automatically](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1406908.html)
-   [Consolidated Exchange Rates on Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1407782.html)
-   [Search for Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1408952.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
