---
id: "section_N1403894"
type: "section"
title: "Updating Rates in the Currency Exchange Rates List"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Currency Exchange Rates > Currency Exchange Rates List Page > Updating Rates in the Currency Exchange Rates List"
parent: "subsect_1527609411"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1403894.html"
anchors: ["bridgehead_N1403913", "bridgehead_N1403925", "bridgehead_N1404042", "procedure_N1404063"]
sha256: "68d1953cc5737761c7e247e21616b925e8773d3a6955d7f7c16b78e5582bde86"
---

You can manually update rates in the Currency Exchange Rates list after they have been initially set up. If you prefer to have NetSuite update some or all exchange rates automatically one time each day, you can enable the Currency Exchange Rate Integration feature. Then, choose which exchange rates need to be updated automatically.

## Manually Updating Currency Exchange Rates {#bridgehead_N1403913}

To manually update an exchange rate between two currencies, you add a new exchange rate record with the same base currency and foreign currency. The effective date of the new exchange rate record must be later than the existing rate record.

Note:

If you enable the Currency Exchange Rate Integration feature, manually entered rates for the same currency pair and effective date aren't overwritten by rate providers. See [Setting Exchange Rates to Be Automatically Updated](#bridgehead_N1404042)

#### To manually update an exchange rate: {#bridgehead_N1403925}

1.  Go to _Lists > Accounting > Currency Exchange Rates > New_.
    
2.  In the **Base Currency** field, select the base currency for this exchange rate update.
    
3.  Select a foreign currency in the **Currency** field.
    
4.  If you have an **Exchange Rate Type** field, select the rate type.
    
    This field appears on the page only when the Currency Exchange Rate Types feature is enabled. For information, see [Currency Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157289938740.html).
    
5.  In the **Exchange Rate** field, enter the updated exchange rate.
    
    The exchange rate is the number of base currency units that equal one foreign currency unit. For example, if you want to set the value of a Euro to 1.357 U.S. dollar, you would enter **1.357** in the **Exchange Rate** field.
    
    You can enter a number with up to 15 digits to the left of the decimal or up to 8 digits to the right of the decimal. For more information, see [Exchange Rate Field Limitations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1527609411.html#bridgehead_N1401684).
    
    For comparison purposes, this page also displays the current (**Previous Effective Rate**) exchange rate and the date that rate became effective.
    
6.  Enter the date that this exchange rate becomes effective in the **Effective Date** field.
    
7.  Click **Save**.
    

## Setting Exchange Rates to Be Automatically Updated {#bridgehead_N1404042}

If the Currency Exchange Rate Integration feature is enabled, you can indicate on a currency record that its exchange rate with each base currency should be automatically updated each day. For information about enabling this feature and about automatic updates, see [Currency Exchange Rate Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404429.html).

If you use the Currency Exchange Rate Types feature, note that automatic updates work only with the default currency exchange rate type.

#### To automatically update exchange rates for a base currency: {#procedure_N1404063}

1.  Go to _Lists > Accounting > Currencies_.
    
2.  Click the name of a currency.
    
3.  On the Currency page, if the **Automatic Update** box is checked, NetSuite updates the exchange rate between this foreign currency and the base currency (or for NetSuite OneWorld, the base currency of each subsidiary).
    
    If you don't want a foreign currency's rates to be automatically updated, clear the box.
    
4.  On the record of a currency that has been defined as a base currency, the **Update Time Zone** field determines the time of the daily automatic exchange rate updates. These updates occur at 6 a.m. in the selected time zone.
    
    The default is U.S. Eastern time. You can select another time zone.
    
    If this currency is a base currency, the read-only **Is Base Currency** box is checked. If it isn't a base currency, the box is clear.
    
    Important:
    
    If you've enabled the use of cross currency triangulation, the Currency page also displays a checked, read-only **Is Anchor Currency** box. You can't delete a designated anchor currency that's used in an exchange rate calculation. For more information about anchor currencies, see [Exchange Rate Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html#bridgehead_4314469559).
    
5.  Click **Save**.
    

### Related Topics

-   [Currency Exchange Rates List Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1527609411.html)
-   [Adding Rates to the Currency Exchange Rates List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401868.html)
-   [Currency Exchange Rate History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157289920531.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
