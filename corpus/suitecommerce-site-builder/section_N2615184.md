---
id: "section_N2615184"
type: "section"
title: "URL Parameters for Setting the Currency on your Website"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Website URL Parameters > URL Parameters for Setting the Currency on your Website"
parent: "section_N2611157"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615184.html"
anchors: []
sha256: "8974910f73c8042382b488453b23e4976bcc3717eb2707028ce9e7358d255824"
---

To set the currency for prices on your web store, ensure that you're using the Multiple Currencies feature and have set up currency records in your account.

For more information, see [Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395463.html).

Select the parameter you want to use, either `currencykey` or `currency`. Both give the same results.

-   Use `currencykey` in the URL and pass the internal ID of the currency record.
    
-   Use `currency` in the URL and pass the value from the Symbol column in the currency list.
    

For example, both URLs below display prices in Euros:

-   http://www.wolfeelectronics.com/Product-Catalog/Flat-ScreenTVs? `currencykey=4`
    
-   http://www.wolfeelectronics.com/Product-Catalog/Flat-ScreenTVs? `currency=EUR`
    

### Related Topics

-   [URL Parameters for Displaying Shopping Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611580.html)
-   [URL Parameters for Adding Items to the Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2612472.html)
-   [URL Parameters for Passing Marketing Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2613194.html)
-   [URL Parameters for Setting Values in Your OneWorld Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2614795.html)
-   [Website URL Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611157.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
