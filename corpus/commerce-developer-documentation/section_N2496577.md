---
id: "section_N2496577"
type: "section"
title: "Shopping Objects"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > Shopping Objects"
parent: "section_N2496227"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html"
anchors: []
sha256: "0ad39009a18d65f1797335b54359eff52548055a8b2e241618482b9938a9db59"
---

The Commerce API includes only one object that is globally accessible in the SuiteScript context, the webContainer object.

The following table lists the objects that are accessible after you have gotten a webContainer. The table also lists the calls you can use to get a reference to each object. You need a reference to a shopping object to call its methods.

| Object | Description | Call to get Object | For available methods, see: |
| --- | --- | --- | --- |
| shoppingSession | Tracks session context. | nlapiGetWebContainer().getShoppingSession() | [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html) |
| customer | Holds data for the logged in customer. | nlapiGetWebContainer().getShoppingSession().getCustomer() | [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html) |
| order | Holds shopping cart data and methods for placing the order. | nlapiGetWebContainer().getShoppingSession().getOrder() | [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html) |
| pageGenerator | Used to generate web pages. | nlapiGetWebContainer().getPageGenerator() | [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html) |
| standardTagLibrary | Implements web site tags. | nlapiGetWebContainer().getStandardTagLibrary() | [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html) |

Note the following:

-   These customer and order objects are different from NetSuite customer and order records, because they hold information within the given shopping session only.
    
-   To access a customer or an order, in addition to getting a webContainer, you also need to get a shoppingSession.
    
-   You can only use Commerce API shopping methods against Commerce API objects. You cannot use shopping methods against NetSuite records.
    
-   Shopping object methods support passing of primitive strings and JSON objects. See [Input Parameters/Return Values for Shopping Object Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497278.html).
    
-   The Commerce API includes JSON objects to support shopping object methods. For details about supported fields for JSON objects, see [JSON Object Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2512816.html).
    
-   For information about governance for shopping object methods, see [SSP Application Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538501.html).
    

### Related Topics:

-   [Input Parameters/Return Values for Shopping Object Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497278.html)
-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
