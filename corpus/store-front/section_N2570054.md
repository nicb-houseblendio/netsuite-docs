---
id: "section_N2570054"
type: "section"
title: "Analytics Preferences"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Getting Started > Prepare the Web Site Setup Record > Comprehensive Web Site Setup Reference > Analytics Preferences"
parent: "section_159499875581"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2570054.html"
anchors: []
sha256: "e0c49ce712272a83593acbc481552500300ee2b4a68a4c863aff9234e8f344f3"
---

Use the preferences described below to enter tracking pixels for web site analytics.

-   Site Builder customers, see [Using Tracking Pixels for Analytics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2653608.html) for more information about using third-party web analytics tools with NetSuite.
    
-   SuiteCommerce and SuiteCommerce Advanced customers, see [Google Analytics 4](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0104849037.html) for more information about setting up Google Analytics.
    

| Preference | Description | Applies To |
| --- | --- | --- |
| Addition to <head> | Enter data for the header in this field. You can enter a script to capture web analytics. For example: `<script src="http://www.google-analytics.com/urchin.js" type="text/javascript"> </script> <script type="text/javascript"> _uacct = "xxxxxxxx"; // your Google account id urchinTracker(); </script>` In this field, you can also add Meta Tag HTML to appear in the `<head>` section of all your web store pages. Note that Meta tags entered on Category and Tab pages are more effective for search engine optimization (SEO). For more information about SEO, see [Site Builder Search Engine Optimization (SEO)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2635817.html). | 
-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Analytics Click Attributes | Add attributes for the Add To Cart button in this field. You can capture analytics data before your shopper gets to the shopping cart. For example: onclick="handleLink(this.href); return false;" The code inside **handleLink()** should be implemented to reconstruct the URL such that shopper identification parameters needed for your analytics package are added to the href. | 

-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Analytics Submit Attributes | Add attributes for the Proceed to Checkout button in this field. You can capture analytics data when your shoppers go to checkout from the shopping cart. For example: onsubmit="handlePost(this); return true;" The code inside **handlePost ()** should be implemented to add fields to the form such that shopper identification parameters needed for your analytics package are posted with the form. | 

-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Order Tracking Script HTML | Enter any tracking HTML you want to use in the header of the order confirmation page, such as tracking code for Google Analytics®. This lets you track the number of orders you receive each day. Note: You can enter tracking code for Site Builder pages in fields on tab and category records. | 

-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Enable Google Analytics | Check this box to pass Google tracking cookies from shopping to checkout. This along with the fields on the Analytics subtab are required for cross-domain analytics tracking to integrate NetSuite with your Google Analytics account. Clear this box if Google Analytics Integration interferes with a custom solution you have already implemented for cross-domain tracking. | 

-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |

### Related Topics

-   [Web Site Setup Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2562624.html)
-   [Shopping Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2567548.html)
-   [Search Index Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159553756087.html)
-   [Field Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159553770489.html)
-   [Web Site Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518463563.html)
-   [Upsell Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2574968.html)
-   [Touch Point Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2576160.html)
-   [Domain Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159553835589.html)
-   [System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159553904637.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
