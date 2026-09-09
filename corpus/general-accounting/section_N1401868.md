---
id: "section_N1401868"
type: "section"
title: "Adding Rates to the Currency Exchange Rates List"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Currency Exchange Rates > Currency Exchange Rates List Page > Adding Rates to the Currency Exchange Rates List"
parent: "subsect_1527609411"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401868.html"
anchors: ["procedure_N1401891"]
sha256: "b6405fb6e88687559721e42886702f259665d3792c2ab9a7e38c5cfb23e3cc99"
---

In the Currency Exchange Rates list, you can specify an exchange rate between each base currency and each foreign currency. These exchange rates are applied to transactions.

This topic includes instructions to add the currency exchange rate manually. You can also integrate with rate providers to get automatic currency exchange rates. For information, see [Currency Exchange Rate Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404429.html).

#### To set the exchange rate for two currencies manually: {#procedure_N1401891}

1.  Go to _Lists > Accounting > Currency Exchange Rates > New_.
    
2.  In the **Base Currency** field, select the base currency for this exchange rate.
    
    If you use NetSuite OneWorld, you can select the base currency for any subsidiary that you can access. If you don't use NetSuite OneWorld, this field displays your base currency.
    
3.  Select a foreign currency in the **Currency** field.
    
    For example, if you're setting the exchange rate for the Euro to your base currency, the U.S. dollar, select the name of your base currency, **USA** in the **Base Currency** field and then select **Euro** in the **Currency** field.
    
    If the **Currency** list doesn't include the currency that you need, you can define a new currency. For more information, see [Creating Currency Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395911.html).
    
4.  If you have multiple currency exchange rate types, in the **Exchange Rate Type** field, select the rate type.
    
    This field appears on the page only when the Currency Exchange Rate Types feature is enabled. For information, see [Currency Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157289938740.html).
    
5.  In the **Exchange Rate** field, enter the exchange rate compared to the base currency.
    
    The exchange rate is the number of base currency units that equal one foreign currency unit. For example, if you want to set the value of a Euro to 1.357 U.S. dollar, enter **1.357** in the **Exchange Rate** field.
    
    You can enter a number with up to 15 digits to the left of the decimal or up to 8 digits to the right of the decimal. For more information see [Exchange Rate Field Limitations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1527609411.html#bridgehead_N1401684).
    
    For comparison purposes, this page also displays the current (previous) exchange rate and the date that rate became effective.
    
6.  Set the date this exchange rate becomes effective in the **Effective Date** field.
    
7.  Click **Save** or **Save & New**.
    

You can go to a transaction page or the Currency Revaluations page to see the impact of an exchange rate change on the value of a transaction.

### Related Topics

-   [Currency Exchange Rates List Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1527609411.html)
-   [Updating Rates in the Currency Exchange Rates List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1403894.html)
-   [Currency Exchange Rate History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157289920531.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
