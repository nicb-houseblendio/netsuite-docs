---
id: "section_N1397831"
type: "section"
title: "Currency Decimal Precision"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Multiple Currencies > Creating Currency Records > Currency Decimal Precision"
parent: "section_N1395911"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397831.html"
anchors: ["bridgehead_N1397923"]
sha256: "b7ce41508898e9d9bc87001eac5ecfd5cd16aae9a61a933df431256f68bd24ea"
---

The Currency Precision field on the currency record is read-only. If you need to change this field to a list through which you can change the precision from zero or two, contact NetSuite Customer Support. To view or edit a currency record, go to _Lists > Accounting > Currencies_ and click the Name link.

The decimal precision of a currency is displayed in the Currency Precision field on the Currency record. For example, the Currency Precision value for the Default Locale United States (English) is 2, for two decimal places. For the Japan (Japanese) local the Currency Precision value is 0. You can't edit the Currency Precision. If you need a different decimal precision, contact NetSuite Customer Support for assistance. The only values supported are 0 and 2.

Some currencies require the use of integers, without decimal fractions. For example, Japanese yen are usually displayed as ¥123, but not as ¥123.45. For this reason, customer-facing documents must display currency amounts in yen using integers. The NetSuite user interface generally displays these currencies as integers. See [Currencies Usually Expressed as Integers](#bridgehead_N1397923).

If the base currency of your company or subsidiary permits the use of decimal fractions, NetSuite displays amounts from foreign currency transactions in base currency amounts using two decimals places. Your customer can see the total amount of a transaction in a zero-precision foreign currency as an integer, but your company's records display the translated, base-currency amounts using two decimal places. For more information, see [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html) and [Setting a Base Currency](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397082.html).

For example, a company can use U.S. dollars as its base currency and price an item at $123.45 per unit. If the exchange rate is 93.4857 Japanese yen to the U.S. dollar, the line item amount displayed on an invoice to a Japanese customer for ten units of the item is ¥115,408, not ¥115,408.10. However, NetSuite displays the transaction amount for the ten units on the U.S. company's books, as $1,234.50. For more information, see [Setting Up Item Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181018.html).

Values in report results are rounded to the base currency precision. This rounding applies to currency values and non-currency values including formula column values.

Currency decimal precision is used for inventory costing calculations to maintain consistency between inventory costing and reporting. Values in report results are rounded to the base currency precision. This rounding applies to currency values and non-currency values, including formula column values.

## Currencies Usually Expressed as Integers {#bridgehead_N1397923}

NetSuite displays the following currencies as integers, without using decimal fractions.

| Country | Currency Name | Currency Code |
| --- | --- | --- |
| Belarus | Ruble | BYR |
| Cambodia | Riel | KHR |
| Chile | Peso | CLP |
| Iceland | Krona | ISK |
| Indonesia | Rupie | IDR |
| Iraq | Dinar | IQD |
| Japan | Yen | JPY |
| Lebanon | Pound | LBP |
| Paraguay | Guarani | PYG |
| South Korea | Won | KRW |
| Viet Nam | Dong | VND |

### Related Topics

-   [Creating Currency Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395911.html)
-   [Viewing and Editing Currency Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543618833.html)
-   [Customizing Currency Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1396253.html)
-   [Currency Record Fields for Currency Exchange Rate Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543620005.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
