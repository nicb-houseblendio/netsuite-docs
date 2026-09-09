---
id: "section_N1395677"
type: "section"
title: "Enabling the Multiple Currencies Feature"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Multiple Currencies > Enabling the Multiple Currencies Feature"
parent: "section_N1395463"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395677.html"
anchors: ["procedure_N1395697"]
sha256: "431fcf73cbd054375da7b342b0ef116970c8c00c396e7a12d72d23e91d4c8017"
---

The Multiple Currencies feature lets you create transactions with customers and vendors in currencies other than your company's base currency.

To enable the Multiple Currencies feature, you must have the Enable Features permission. This feature provides support for transactions with customers and vendors that use currencies other than the currency in which your company manages its financial reporting.

NetSuite relies on accounting periods to properly post open balance revaluation for multiple currencies at the end of each month. If you currently use calendar months instead of accounting periods, enable the Accounting Periods feature to use the Multiple Currencies feature effectively. See [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html).

Enabling the Multiple Currencies feature does the following:

-   Adds a Currencies subtab to prospect, customer, and vendor records under the Financial subtab
    
-   Changes the Currency field on customer and vendor records to Primary Currency
    
-   Enables editing of the Primary Currency field on sales and purchase transactions
    
-   Lets you define purchase and sales prices in multiple currencies on item records
    

#### To enable the Multiple Currencies feature: {#procedure_N1395697}

1.  Go to _Setup > Company > Enable Features_.
    
2.  On the **Company** subtab, check the **Multiple Currencies** box.
    
    You can also enable the **Currency Exchange Rate Integration** feature now if you want to automatically update exchange rates one time each day. For more information, see [Currency Exchange Rate Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404429.html).
    
3.  Click **Save**.
    

After you enable the feature, ensure that the base currency for your company is marked **Yes** on the Currencies page at _Lists > Accounting > Currencies_. In NetSuite OneWorld, each subsidiary must also have a base currency.

Important:

Make any changes to base currency before you do anything else in NetSuite. You can't change the base currency after a record has been saved that includes a currency amount or link. For instructions, see [Setting a Base Currency](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397082.html).

To use a currency not included in the default list on the Currencies page, you must first define the new currency. NetSuite supports all ISO 4217 standard currencies. For instructions, see [Creating Currency Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395911.html).

The Multiple Currencies feature includes capabilities that were historically separate features. The Multi-Currency Customers and Multi-Currency Vendors features have been combined in the Multiple Currencies feature.

If your account supports multiple currencies as separate features, clear the Multi-Currency Customers and Multi-Currency Vendors boxes before you clear the Multiple Currencies box to disable the feature. You can't disable these features if there are associated records or transactions.

### Related Topics

-   [Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395463.html)
-   [Creating Currency Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395911.html)
-   [Setting a Base Currency](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397082.html)
-   [Assigning Currencies to Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397405.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
