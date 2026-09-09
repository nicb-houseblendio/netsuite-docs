---
id: "section_N1404249"
type: "section"
title: "Setting Exchange Rates Directly on Transactions"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Currency Exchange Rates > Setting Exchange Rates Directly on Transactions"
parent: "section_N1401566"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404249.html"
anchors: ["procedure_N1404280"]
sha256: "2dddd158479c36fb22679fd441175ff64b9bf80a6cd9949107d8587bdf6b3802"
---

The default exchange rate for a transaction is based on the currency selected on the related entity (such as customer or vendor) record and the transaction date. This default is the rate in the Currency Exchange Rates list for the selected currency effective as of the transaction date. For more information, see [Currency Exchange Rates List Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1527609411.html).

If you want to use an exchange rate other than the default, you may be able enter this other exchange rate directly on the transaction record. To change the exchange rate, you need the list permission Currency at the Edit level.

The exchange rate is the number of transaction (or source) currency units that equal one base currency unit. For example, if the transaction currency is Japanese yen and the base currency is U.S. dollars, you need the number that converts Japanese yen to 1 U.S. dollar. If the transaction amount is ¥10,000 and the exchange rate is 0.0001, the base currency amount is $1.

Note:

If you use the Currency Exchange Rate Types feature, you can set only the default currency exchange rate type.

#### To manually set the exchange rate on a transaction: {#procedure_N1404280}

1.  Create a new transaction, or edit an existing one, and complete the required fields.
    
2.  Change the default value of the **Exchange Rate** field as needed. The location of this field varies by transaction as follows:
    
    -   **Purchase orders** - on the **Items** subtab
        
    -   **Vendor bills** - in the Primary Information section of the bill
        
    -   **Sales orders and invoices**\- on the **Accounting** subtab
        
    
    You can enter a number with up to 15 digits to the left of the decimal or up to 8 digits to the right of the decimal. For more information, see [Exchange Rate Field Limitations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1527609411.html#bridgehead_N1401684).
    
3.  If the Currency Exchange Rate Integration feature isn't enabled, a popup window prompts you on whether to make the value you entered the new default exchange rate.
    
    -   Click **OK** to create a new currency exchange rate between the transaction currency and the base currency, effective as of the current date.
        
    -   Click **Cancel** to apply this exchange rate to only this transaction.
        
4.  Complete the remaining fields.
    
5.  Click **Save**.
    

### Related Topics

-   [Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401566.html)
-   [Currency Exchange Rates List Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1527609411.html)
-   [Currency Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157289938740.html)
-   [Currency Exchange Rate Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404429.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
