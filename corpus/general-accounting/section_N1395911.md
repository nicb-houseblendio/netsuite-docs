---
id: "section_N1395911"
type: "section"
title: "Creating Currency Records"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Multiple Currencies > Creating Currency Records"
parent: "section_N1395463"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395911.html"
anchors: ["procedure_N1396351"]
sha256: "ca418e479fa86b70e7f7cc1583f3a84533ed2ac48e0e172cfc11f7b9c8c7da8a"
---

By default, NetSuite provides the following currencies with the Multiple Currencies feature:

| Country | Currency Name | Symbol/ Currency Code |
| --- | --- | --- |
| Canada | dollar | CAD |
| European Union | euro | EUR |
| Great Britain | pound | GBP |
| United States | dollar | USD |

Create additional currency records for any other currencies to be used for transactions. Each currency must have a name, default locale, ISO code, and default exchange rate. NetSuite supports all ISO 4217 standard currencies.

For instructions to view, edit, or delete existing currency records, see [Viewing and Editing Currency Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543618833.html).

#### To create a currency record: {#procedure_N1396351}

1.  Go to _Lists > Accounting > Currencies > New_.
    
2.  In the **Name** field, enter a unique name for the currency.
    
    Use a name that combines the country name or abbreviation as well as the name of the currency. For example, pesos are the currency in the Philippines, Uruguay, and Mexico. For Mexico, you might enter **Mexican peso**.
    
    The currency name you enter here becomes an option for the currency on customer, vendor, and other records. For more information, see [Assigning Currencies to Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397405.html) and [Assigning a Foreign Currency Price to a Sales Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2183023.html).
    
3.  In the **Default Locale** field, select a country to determine the currency format.
    
    The **ISO Code** field displays the three-letter International Standards Organization (ISO) currency code for the **Default Locale** you select. You receive a warning if you change the value to an unsupported ISO code. Non-standard ISO codes significantly slow down the exchange rate update process. To use the Currency Exchange Rate Integration feature, the currency record must have a valid ISO code.
    
    The **Format Sample** field displays the default currency format for the currency of the **Default Locale**. The currency format is the combination of the symbol, thousands separator, level of decimal precision, and negative symbol used to display amounts on transactions.
    
4.  In the **Default Exchange Rate** field, enter an exchange rate for this currency against the base currency of this company. If no exchange rates are entered for a currency and if the Currency Exchange Rate Integration feature is disabled, NetSuite uses the default exchange rate for transactions.
    
    If you use NetSuite OneWorld, enter the exchange rate for this currency against the base currency of the root parent subsidiary.
    
    If you use Multi-Book Accounting, enter the exchange rate for this currency against the base currency of the root subsidiary primary book currency.
    
    The exchange rate is equal to the base currency amount divided by the foreign currency amount.
    
    For example:
    
    -   If your company is located in Canada and you're defining the U.S. dollar, and the current exchange rate is 1.02 Canadian dollars to 1.00 U.S. dollar, the **Default Exchange Rate** for the U.S. dollar is 1.02/1.00, or 1.02.
        
    -   If your company is located in the U.S. and you're defining the Canadian dollar, and the current exchange rate is 1.02 Canadian dollars to 1.00 U.S. dollar, the **Default Exchange Rate** for the Canadian dollar is 1.00/1.02, or .98.
        
    
    This rate is the basis for rates in the Currency Exchange Rates table that are used in foreign currency transactions. If you use OneWorld, this rate also is the basis for rates in the Consolidated Exchange Rates table that are used in consolidated financial reporting. For more information, see [Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401566.html) and [Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404834.html).
    
5.  Complete other fields as needed. Some fields are displayed only when the Currency Exchange Rate Integration is enabled in your account. For information about these fields, see [Currency Record Fields for Currency Exchange Rate Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543620005.html).
    
    1.  **Is Base Currency** is displayed only on existing currency records for currency designated as the base currency for a subsidiary or as the currency at company level. The box is always checked. You can't edit this field on the currency record.
        
        For instructions to set a base currency, see [Setting a Base Currency](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397082.html) and, if you use NetSuite OneWorld, [Creating Subsidiary Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272471.html).
        
    2.  **Currency Precision** is populated when you save the currency record. The precision designates the number of digits to the right of the decimal point used in currency transactions. Precision can be zero or two. For more information, see [Currency Decimal Precision](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397831.html).
        
    3.  Clear the **Inactive** box to make the currency available, or check it to make the currency inactive. You can't make a currency inactive if any open transactions exist in that currency.
        
    4.  To customize the format for this currency, check the **Override Currency Format** box.
        
        -   In the **Symbol** field, enter the text and currency symbol you want to use for this currency. Include spaces if you want to separate the symbol from the currency value.
            
        -   In the **Symbol Placement** field, select to place the currency symbol before or after the number.
            
        
        The **Format Sample** field shows how currency amounts display on screen and on printed transactions using your customized currency format and personal Number Format preference. For more information, see [Customizing Currency Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1396253.html) and [Setting Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N475297.html)
        
6.  Click **Save**.
    

After you create records for the currencies to be used in your transactions, you can set up exchange rates between currencies. See [Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401566.html).

### Related Topics

-   [Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395463.html)
-   [Enabling the Multiple Currencies Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395677.html)
-   [Setting a Base Currency](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397082.html)
-   [Assigning Currencies to Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397405.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
