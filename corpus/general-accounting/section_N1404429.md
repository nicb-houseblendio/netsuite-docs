---
id: "section_N1404429"
type: "section"
title: "Currency Exchange Rate Integration"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Currency Exchange Rates > Currency Exchange Rate Integration"
parent: "section_N1401566"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404429.html"
anchors: []
sha256: "41d7fa4a9e2a3045131c9a5d10bce7f74e864a1f59ce2db04868ade44ff8d4ef"
---

The Currency Exchange Rate Integration feature automatically updates currency exchange rates by the specified provider one time each day for all accounts that use exchange rate integration. The automatic update occurs at approximately 6:00 a.m. in one of four available time zones. The updated rates reflect the latest exchange rates available as of 6:00 a.m. in your selected time zone. The time zones and representative cities in those time zones are as follows:

-   GMT - 5 hours = Eastern Time (U.S. & Canada), New York City, Toronto
    
-   GMT + 1 hour = Brussels, Copenhagen, Madrid, Paris
    
-   GMT + 9 hours = Osaka, Sapporo, Tokyo
    
-   GMT + 11 hours = Magadan, Solomon Is., New Caledonia
    

The Eastern Time (U.S. & Canada) time zone is the default. You can specify a different time zone on each base currency record to designate the time for updates to its foreign currency exchange rates.

The automatic update run time respects time zone changes for daylight savings time, and runs daily at approximately the same local system time. If you operate in a location that follows daylight savings time, the GMT time zone shown in the Recorded Date and Source Date columns on the Exchange Rate History page change. To open the Exchange Rate History page and view the currency rate updates for your account, go to Lists > Accounting > Currencies and then click History.

Some exchange rates may not update on certain days, depending on the underlying data sources and their market hours. For example, a currency pair's rate may remain the same on Saturday and Sunday, or on Sunday and Monday, depending on the base currency's time zone and the data source's market hours. If this causes any issues, you can manually update exchange rates. For more information, see [Updating Rates in the Currency Exchange Rates List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1403894.html).

If you create a currency after the automatic update occurs, the exchange rate for the currency doesn't get updated until the next automatic update. In this scenario, NetSuite uses the default exchange rate or the exchange rate entered on the transaction until the rates are updated.

You must define a base currency to trigger exchange rate integration. For information about creating a base currency, see [Setting a Base Currency](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397082.html).

After you enable the feature you must specify your exchange rate provider and determine the method used to obtain currency exchange rates. You must also specify anchor currencies, if needed. The following topics include instructions and additional information.

-   [Enabling the Currency Exchange Rate Integration Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4322310757.html)
    
-   [Integrated Exchange Rate Providers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4320491322.html)
    
-   [Methods for Obtaining Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4322231734.html)
    
-   [Anchor Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4322232861.html)
    

If you use the Currency Exchange Rate Types feature, be aware that rate provider integration works only with the default currency exchange rate type.

Note:

Currency exchange rates in Release Preview and sandbox accounts may differ from rates in production accounts.

### Related Topics

-   [Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401566.html)
-   [Currency Exchange Rates List Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1527609411.html)
-   [Currency Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157289938740.html)
-   [Setting Exchange Rates Directly on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404249.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
