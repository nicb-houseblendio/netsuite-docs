---
id: "section_N1401566"
type: "section"
title: "Currency Exchange Rates"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Currency Exchange Rates"
parent: "chapter_N1395057"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401566.html"
anchors: []
sha256: "5517006947a13ac912ef19bec259af196527598a981a2df414cb7d4b179ab0cc"
---

After you've created currency records in NetSuite and defined a base currency, you need to set up exchange rates between the base currency and foreign currencies to apply to transactions. If you use NetSuite OneWorld and defined a different base currency per subsidiary, set up different exchange rates between each base currency and its foreign currencies. Exchange rates for a base currency apply to all subsidiaries that use the same base currency.

Currency exchange rates are used to convert foreign currencies to base currencies, providing default rates for transactions in currencies other than the base currency. Exchange rates are expressed in terms of base currency units per foreign currency (source) unit.

Exchange rates are stored in the Currency Exchange Rates list page at _Lists > Accounting > Currency Exchange Rates_. For information about this page, see [Currency Exchange Rates List Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1527609411.html).

You can update exchange rates in four ways.

-   You can manually update a rate between two currencies by adding a new rate for the same two currencies with a different effective date. See [Updating Rates in the Currency Exchange Rates List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1403894.html).
    
-   You can set a rate to be automatically updated one time each day by the Currency Exchange Rate Integration feature. Currency Exchange Rate Integration doesn't overwrite a rate if one is already stored for the same currency pair and effective date. See [Currency Exchange Rate Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404429.html).
    
-   You can import currency exchange rates from an external system using the Import Assistant. The exchange rate values must be in a CSV file to import them into NetSuite. See [Currency Exchange Rates Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N359131.html).
    
-   You can set the exchange rate on the individual transactions. The default exchange rate for transactions is determined by one of the other methods of setting and updating exchange rates. See [Setting Exchange Rates Directly on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404249.html).
    

### Related Topics

-   [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html)
-   [Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395463.html)
-   [Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404834.html)
-   [Foreign Currency Revaluation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1409370.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
