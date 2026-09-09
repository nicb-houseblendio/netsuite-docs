---
id: "section_N1406908"
type: "section"
title: "Calculating Consolidated Exchange Rates Automatically"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Consolidated Exchange Rates > Calculating Consolidated Exchange Rates Automatically"
parent: "section_N1404834"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1406908.html"
anchors: ["bridgehead_156987617457"]
sha256: "16d3fc4b10b8935e52fc498afe60ebf8b71b241b1a801909f4d15ca4acb089df"
---

If you can edit a consolidated exchange rate, you can choose to have NetSuite calculate the rate for you. NetSuite can check the transactions and currency exchange rates from which consolidated rates are derived and automatically update the consolidated exchange rates.

Your user role must have the Currency permission with the Full permission level to work with consolidated exchange rates.

When NetSuite calculates consolidated exchange rates, the results are derived from the currency exchange rates and transaction history in your account as follows:

-   **Current Rate** - The currency exchange rate in effect at the end of the period.
    
-   **Average Rate** - Weighted average based on transaction amounts for the period for all accounts with a General Rate Type of Average. The transaction amounts are multiplied by the currency exchange rates on the dates of the transactions. The weighted average equals the total of the transaction amounts multiplied by the currency exchange rates divided by the total transaction amount.
    
-   **Historical Rate** - Weighted average based on transaction amounts for the period for all accounts with a General Rate Type of Historical. The transaction amounts are multiplied by the currency exchange rates on the dates of the transactions. The weighted average equals the total of the transaction amounts multiple by the currency exchange rates divided by the total transaction amount.
    

For examples of the calculations, see [Consolidated Exchange Rate Automatic Calculation Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1407165.html).

## To have NetSuite calculate consolidated exchange rates automatically: {#bridgehead_156987617457}

-   Go to _Lists > Accounting > Consolidated Exchange Rates_. Rows for open periods that have direct rates include an Auto Calculate Rates icon ![Calculator icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/calculator.png) in the **Calculate** column. Click the icon to update rates in that row only, or click **Calculate** to update the rates for all subsidiaries to which you have access.
    

or

1.  From the Period Close Checklist, for the Calculate Consolidated Exchange Rates task, click **Calculate Consolidated Exchange Rates**.
    
2.  On the Consolidated Exchange Rates page, click **Calculate** to update rates for the period.
    
    NetSuite automatically calculates the rates for all the subsidiaries to which you have access but **only** those subsidiaries. Rates for other subsidiaries aren't updated.
    
    For information about closing accounting periods, see [Using the Period Close Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1455781.html).
    

### Related Topics

-   [Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404834.html)
-   [Consolidated Exchange Rates vs. Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405239.html)
-   [Consolidated Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405625.html)
-   [Viewing Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405950.html)
-   [Editing Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1406714.html)
-   [Consolidated Exchange Rates on Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1407782.html)
-   [Search for Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1408952.html)
-   [Consolidated Exchange Rate Types for Transaction Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1409190.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
