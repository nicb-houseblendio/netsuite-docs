---
id: "section_N359131"
type: "section"
title: "Currency Exchange Rates Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Accounting Import Type > Currency Exchange Rates Import"
parent: "section_N357752"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N359131.html"
anchors: []
sha256: "4392f8ba8b436e75c6e1468e2425b85f5463b28d8b86084e843bf900f8e72e43"
---

When the Multiple Currencies feature is enabled, you can use the Import Assistant to import currency exchange rates into NetSuite. Exchange rates are stored as a list in NetSuite, with each line in the list representing an exchange rate between a base currency and a foreign currency. For more information, see [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html).

NetSuite OneWorld accounts may have multiple base currencies, with different base currencies set for different subsidiaries. Accounts that are not OneWorld have a single base currency only. Note that exchange rates defined for a base currency in a OneWorld account apply to all subsidiaries using that base currency.

The Currency Exchange Rates import requires the following values for each rate to be imported:

-   **Currency** - the foreign currency to which the rate is applied
    
-   **Exchange Rate** - the number of base currency units that equal one foreign currency unit
    
-   **Effective Date** - the first date that the rate should be used
    
-   **Base Currency** - (OneWorld only) the base currency to which the rate is applied
    
    For accounts that aren't OneWorld, you don't have to define a base currency per rate, because the base currency is always the same.
    
-   **Exchange Rate Type** - (only when the Currency Exchange Rate Types feature is enabled) the currency exchange rate type associated with the exchange rate
    
    You can select the value in your Field Mapping if the import file doesn't include a value. The Import Assistant automatically selects the default currency exchange rate type. For information about the feature, see [Currency Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157289938740.html).
    

Update data handling isn't supported for this import, to be consistent with currency exchange rates functionality in the user interface. To update a rate between two currencies, add a record with the same base currency and foreign currency, the new exchange rate, and a new effective date. For example:

-   If NetSuite has the following exchange rate stored:
    

| Base Currency | Foreign Currency | Exchange Rate | Effective Date |
| --- | --- | --- | --- |
| US Dollar | Euro | 1.2287 | 7/1/2012 |

-   To change the rate, include a line like the following in your CSV import file, with a new exchange rate and a new effective date. When the import is completed, this new rate will be used from the new date in the future.
    

| Base Currency | Foreign Currency | Exchange Rate | Effective Date |
| --- | --- | --- | --- |
| US Dollar | Euro | 1.2298 | 8/1/2012 |

For more details about how currency exchange rates are handled in NetSuite, review the _Lists > Accounting > Currency Exchange Rates_ page, and see [Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401566.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, in this case Accounting, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [CSV Import Error Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4568635774.html)
-   [Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401566.html)

### Related Topics

-   [Accounting Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N357752.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
