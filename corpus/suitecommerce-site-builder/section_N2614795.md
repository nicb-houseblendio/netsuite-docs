---
id: "section_N2614795"
type: "section"
title: "URL Parameters for Setting Values in Your OneWorld Web Store"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Website URL Parameters > URL Parameters for Setting Values in Your OneWorld Web Store"
parent: "section_N2611157"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2614795.html"
anchors: []
sha256: "9017292d8f1ef77543ef20ad439fc2997f2b8534583b3a12b04f222c185f1f13"
---

The table below shows the URL parameters you can use to set values in your OneWorld web store. These parameters are only used by backend processes and aren't shown in the user interface. If you use hosted pages in your website or have an external catalog site (WSDK), these parameters can help with customization.

Note that the URLs below need a value for the _c_ parameter (your NetSuite account number) and the _n_ parameter (the internal ID for the site if you use multiple websites). If you use a custom domain, omit the _c_ and _n_ parameters.

For more information about constructing a URL, see [Required Web Site URL Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611157.html#bridgehead_N2611392).

| URL | URL Parameter | Notes |
| --- | --- | --- |
| /app/site/backend/setshoppercurrency.nl | `selcurrency` | Sets the currency for the shopper's session. Pass the ID of the currency. |
| /app/site/backend/setshopperlanguagelocale.nl | `setshopperlanguage` | Sets the language displayed on the site for the current shopper's session. Use this parameter to pass language codes. For example: en\_US, en\_UK, or fr\_FR. Note: the language codes are not exposed in the NetSuite system. You may need to research which language code is appropriate. |
| /app/site/backend/setshoppersubsid.nl | `selsubsidiary` | Sets the subsidiary displayed in the website for the current shopper's session. The subsidiary must appear in the list of regions displayed on your web store in the Web Site Setup form. |
| /app/site/backend/intl/setshopperregioninfo.nl | `c` `n` `selsubsidiary` `selcurrency` `selshopperlanguage` | This URL supports multiple parameters including the standard `c` and `n` parameters for account and site. Use this backend URL to send multiple requests to be processed at one time.
-   Selsubsidiary - Use the internal ID of the subsidiary you want to set.
-   Selcurrency - Use the internal ID of the currency you want to set.
-   Selshopperlanguage - Use this parameter to pass a locale key. For example: en\_US, en\_UK, or fr\_FR.

Note: locale keys are not exposed in the NetSuite system. You may need to research which language code is appropriate. |

### Related Topics

-   [URL Parameters for Displaying Shopping Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611580.html)
-   [URL Parameters for Adding Items to the Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2612472.html)
-   [URL Parameters for Passing Marketing Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2613194.html)
-   [URL Parameters for Setting the Currency on your Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615184.html)
-   [Website URL Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611157.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
