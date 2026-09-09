---
id: "section_N2532617"
type: "section"
title: "sitesettings"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > sitesettings"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2532617.html"
anchors: []
sha256: "8f75778527b5dde78778d384c5f1ab09295211b2153fb65ff1d7e673922d88a7"
---

| Field Name | Field Type | Description | In Get Functions? | In Set Functions? |
| --- | --- | --- | --- | --- |
| analytics | JSON [analyticssettings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2516176.html) object | Analytics settings | yes | no |
| checkout | JSON [checkoutsettings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2516589.html) object | Checkout settings | yes | no |
| cookiepolicy | string | Returns the URL for the cookie policy file in the NetSuite file cabinet. | yes | no |
| currencies | Array of JSON objects with fields (internalid, name, isdefault, symbolplacement) | Ordered list of currencies supported by the site `isdefault` field is a Boolean, with a value of **T** for default currency, **F** for others. `symbolplacement` uses the constants: SYMBOL\_BEFORE\_NUMBER = 1 and SYMBOL\_AFTER\_NUMBER = 2 | yes | no |
| defaultshipcountry | string | Default ship to country | yes | no |
| defaultshippingmethod | string | Default shipping method | yes | no |
| displayname | string | Site name | yes | no |
| imagesizes | Array of JSON objects with image resize definitions (resizeid, resizeh, resizew) | Each object has the following properties:
-   maxwidth-maximum resized image width in pixels
-   maxheight-maximum resized image height in pixels
-   urlsuffix-suffix that should be added to the image URL to return a resized image
-   internalid-internal system ID of image resize definition.
-   name-value from the Image Resize ID field (image resize definition) as entered on the Web Site Setup page.

 | yes | yes |
| iswebstoreoffline | boolean | Retruns T or F depending on whether the web store is online or offline. | yes | no |
| iswsdk | boolean | Returns T or F depending on the settings of the WSDK checkbox on the site record (tab setup) and the WSDK feature settings for a site. | yes | no |
| languages | Array of JSON objects with fields (internalid, name, isdefault) | Ordered list of languages for the site isdefault field is a Boolean, with a value of T for default language, F for others | yes | no |
| loginallowed | string | Indicates whether login is allowed Value should be T or F. | yes | no |
| loginrequired | string | Indicates whether login is required to access the site Value should be T or F. | yes | no |
| order | JSON [ordersettings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2525697.html) object | Order settings | yes | no |
| paymentmethods | array of [paymentmethod](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2529580.html) objects | Payment methods | yes | no |
| pricesincludevat | string | Indicates whether prices include VAT Value should be T or F. | yes | no |
| registration | JSON [registrationsettings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2530643.html) object | Registration settings | yes | no |
| requireloginforpricing | string | Indicates whether login is required to display item prices Value should be T or F. | yes | no |
| requireshippinginformation | boolean | Indicates whether shipping information needs to be collected Value should be T or F. | yes | no |
| shipallcountries | string | Indicates whether shipping is supported to all countries Value should be T or F. | yes | no |
| shippingrequired | string | Indicates whether shipping is required for the site Value should be T or F. | yes | no |
| shiptocountries | Array of strings | Countries where shipping is supported | yes | no |
| showextendedcart | string | Indicates whether extended cart should be displayed Value should be T or F. | yes | no |
| showshippingestimator | string | Indicates whether shipping estimator should be displayed Value should be T or F. | yes | no |
| sitetype | string | Indicates the type of web site. Value should be ADVANCED or STANDARD. ADVANCED indicates the site is a SuiteCommerce, SuiteCommerce Advanced or SuiteCommerce InStore site whereas STANDARD indicates it is a web site built with Site Builder. | yes | no |
| subsidiaries | Array of JSON objects with fields (internalid, name, isdefault) | Ordered list of subsidiaries for the site isdefault field is a Boolean, with a value of T for default subsidiary, F for others | yes |  |
| wsdkcancelcarturl | string | For use with an External Catalog Site (WSDK). Returns the Cancel Cart URL. | yes | no |
| wsdkcancelcheckouturl | string | For use with an External Catalog Site (WSDK). Returns the Cancel Checkout URL. | yes | no |
| wsdkcancelloginurl | string | For use with an External Catalog Site (WSDK). Returns the Cancel Login URL. | yes | no |
| wsdkcompletecheckouturl | string | For use with an External Catalog Site (WSDK). Returns the Complete Checkout URL. | yes | no |
| wsdkcompleteloginurl | string | For use with an External Catalog Site (WSDK). Returns the Complete Login URL. | yes | no |

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
