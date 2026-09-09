---
id: "section_N2562624"
type: "section"
title: "Web Site Setup Preferences"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Getting Started > Prepare the Web Site Setup Record > Comprehensive Web Site Setup Reference > Web Site Setup Preferences"
parent: "section_159499875581"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2562624.html"
anchors: ["bridgehead_N2562815", "bridgehead_N2563071", "bridgehead_N2563304", "bridgehead_N2563575", "bridgehead_N2563821", "bridgehead_N2564261"]
sha256: "6ef1752c8e6ea32ddfbedbae583b23e91e6713976618ce1c99b0a458be4b96dc"
---

Use the **Setup** tab of the Set Up Web Site record to establish a foundation for your site. Select preferences based on the type of site you're creating.

Note:

Preferences are based on the type of site you're implementing.

Refer to the following tables for detailed descriptions of the preferences available:

-   [Website Basics](#bridgehead_N2562815)
    
-   [Home Page](#bridgehead_N2563071)
    
-   [Multi-Site Settings](#bridgehead_N2563304)
    
-   [Descriptive URLs](#bridgehead_N2563575)
    
-   [Preferences](#bridgehead_N2563821)
    
-   [Cookie Law Compliance](#bridgehead_N2564261)
    

## Website Basics {#bridgehead_N2562815}

| Preference | Description | Applies To |
| --- | --- | --- |
| Display Name | Create a name for your site to display in the heading of your site and in customer browsers. Don't use the special character `'` as part of the display name. | 
-   SuiteCommerce MyAccount
-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Internal Name | This is the name for your site that displays on lists in your NetSuite account. This name isn't exposed to external customers. Fill in this filed, even if the name is identical to your Display Name. | 

-   SuiteCommerce MyAccount
-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Take Website Offline for Maintenance | Check this box to temporarily take your site offline for maintenance. When you've finished making changes, clear this checkbox and your site becomes available for shoppers. | 

-   SuiteCommerce MyAccount
-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Inactive | Check the Inactive box to make the site inaccessible to users without deleting it. An inactive site still retains internal references to other areas of NetSuite. For more information, see [Making a Website Inactive](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1559227395.html). | 

-   SuiteCommerce MyAccount
-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Type | This field states the type of SuiteCommerce website being implemented. This can be SuiteCommerce, SuiteCommerce Advanced, SuiteCommerce MyAccount, or Site Builder. | 

-   SuiteCommerce MyAccount
-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |

## Home Page {#bridgehead_N2563071}

These preferences determine how your site's Home Page displays and behaves.

Site Builder customers, see [Setting Up Your Site Builder Home Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2578280.html) and [Website Hosting with Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2598224.html) for more information.

| Preference | Description | Applies To |
| --- | --- | --- |
| Default Hosting Root | Select the folder where you store HTML files for your web site. | 
-   SuiteCommerce MyAccount
-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Web Site Home Page Type | Choose one of the following:

-   **Web Site Tab** - Select Web Site Tab to have a NetSuite web site tab as your Home page.
-   **Hosted Web Page** - Select this if you want to use a hosted page as your Home page. This requires you to have enabled the Web Site Hosting feature.

 | 

-   Site Builder

 |
| Web Site Home Page | Select the NetSuite tab or hosted web page you want to use as the landing page when customers first visit your site. | 

-   Site Builder

 |

## Multi-Site Settings {#bridgehead_N2563304}

Note:

From 2020.2 onwards, the Multiple Website feature is automatically enabled for all accounts. You no longer need to enable it and it's no longer possible to disable it. However, you may need additional site licences to create more than one website.

The preferences you choose below determine the type of site you're creating. For more information, see [Creating Multiple Websites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2580798.html).

| Preference | Description | Applies To |
| --- | --- | --- |
| Price Level | This setting lets you display the same item on different sites with different price levels on each site. For more information, see [Multiple Website Online Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2581595.html). | 
-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Web Site Scope | Select the type of web site or store you want to operate. This setting lets you apply a different scope to each of your web sites. For example, you can operate one site as a full web store, and another as information only.

-   **Full Web Store** - Includes a shopping cart and checkout, allowing customers to purchase items. You must enable the Web Store feature to see this option.
-   **Information and Catalog, With Pricing** - Includes information and items from your account with the online price for each item but doesn't include the option to purchase.
-   **Information and Catalog** - Includes information and items from your account without prices or the option to purchase.
-   **Information Only** - Includes information from you account but does not publish item names, descriptions, or prices.

Important: If the SuiteTax feature is enabled, you can only set the Web Site Scope to 'Information and Catalog' or 'Information Only'. Site Builder web sites with pricing aren't compatible with SuiteTax. | 

-   Site Builder

 |

## Descriptive URLs {#bridgehead_N2563575}

The table below describes preferences associated with the Descriptive URLs feature.

Note:

You can change the preferences listed below at any time. Outside links based on descriptive URLs in a different format (for example, with or without file extensions) continue to execute a 301 redirect to the new format you set.

Site Builder customers, see [Descriptive URLs in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2637101.html) for more information.

| Preference | Description | Applies To |
| --- | --- | --- |
| Format | Choose from the following options for items in your web store:
-   /tab-name/category-name/item-name (Site Builder only)
-   /item-name

 | 

-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Use File Extension | Check this box to optimize descriptive URLs. This preference does the following: On an image file in the file cabinet, it includes the extension for the image file in the URL. For example, /Flat-Screen.jpg. The file extension is also added to item pages, and information item pages. On URLs that point to tabs and categories, it includes a trailing slash. For example, http://www.store.com/Home-Entertainment/TVs/. | 

-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Action for Unrecognized URLs | To handle unrecognized URLs, select one of the following options:

-   **Page Not Found** - Returns a Page Not Found (404) error for unrecognized URLs.
-   **Moved Permanently** - Redirects to the last valid descriptive URL for the item with 301 Moved Permanently status code.
-   **Return Search Results** - Redirects to a search results page on your site, based on keywords found in the URL.

 | 

-   Site Builder

 |

## Preferences {#bridgehead_N2563821}

Set general preferences for item display, sales, and credit card processing.

| Preference | Description | Applies To |
| --- | --- | --- |
| Scriptable Cart and Checkout | Check this box to run SuiteScript on the sales order form submitted during the Web store checkout. To use scriptable cart, you must customize a Standard Online Order form by adding your script to the transaction form. Check this box to activate your script during Web store checkout. Note: If you use terms for your customers, you must attach your checkout script to both a customized Online Order - Invoice form, and an Online Order - Cash Sales form. | 
-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Scripting Template (Credit Card) | In this field, select the sales order form to which you attached custom SuiteScript for use in the shopping cart. You can customize any of the following types of forms: Standard Sales Order - Cash Sale Standard Online Sales Order - Cash Sale (External) Note: If you use terms for your customers, you must attach your checkout script to a customized Online Order - Cash Sale form, and Online Order - Cash Sales form. | 

-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Scripting Template (Invoice) | In this field, select the sales order form to which you attached custom SuiteScript for use in the shopping cart. You can customize any of the following types of forms: Standard Sales Order - Invoice Standard Online Sales Order - Invoice (External) Note: If you use terms for your customers, you must attach your checkout script to a customized Online Order - Cash Sale form, and Online Order - Cash Sales form. | 

-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Show Uncategorized Items | Check this box so that items that aren't published to a category in your web site can display in search results. Shoppers who run a search on your site will see all items that meet their criteria that have the Display in Web Site box checked. This can be useful if you haven't assigned items to categories. Clear this box to only show items assigned to categories. | 

-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Credit Sales Reps for Web Store Orders | Check this box to count sales generated in your web store toward your sales reps' totals. For a sale to be credited to a sales rep, the sales rep must be selected on the customer's record before an order is placed. If you clear this box, sales generated in your web store aren't added to your sales reps' totals. | 

-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Default Customer Category | Select the customer category that should be automatically assigned to customer records created through the web site when customers register or make purchases. You can always edit the customer category on customer records. To create new customer categories, go to _Setup > Accounting > Accounting Lists > New_. | 

-   SuiteCommerce MyAccount
-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Enable Shipping Estimator In Cart | 

-   **In Site Builder websites**, check this box to give customers an estimate of shipping costs before they complete shipping information in checkout. The lowest estimated shipping cost is displayed by default. If you offer real-time rates, a customer can enter a zip code to receive an estimate. If the order qualifies for free shipping, 'Free Shipping' is displayed.
-   **In SuiteCommerce Advanced** websites, you can check this box if you do not have a default Shipping Method chosen. The Shipping Estimator shows the lowest shipping cost from available Shipping Methods.

 | 

-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |

## Cookie Law Compliance {#bridgehead_N2564261}

The EU Cookie Law, or EU e-Privacy Directive, requires that e-commerce merchants doing business in the European Union get informed consent from site visitors before placing cookies on their computers. Set your preferences for cookie law compliance.

| Preference | Description | Applies To |
| --- | --- | --- |
| Show Cookie Banner | Check this box to publish a banner requesting that shoppers comply with the use of cookies on your site. | 
-   SuiteCommerce MyAccount
-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |
| Cookie Policy | Select your cookie policy file stored in the file cabinet. Your cookie policy displays when shoppers click the link in the banner to learn more. | 

-   SuiteCommerce MyAccount
-   SuiteCommerce
-   SuiteCommerce Advanced
-   Site Builder

 |

### Related Topics

-   [Shopping Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2567548.html)
-   [Analytics Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2570054.html)
-   [Search Index Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159553756087.html)
-   [Field Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159553770489.html)
-   [Web Site Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518463563.html)
-   [Upsell Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2574968.html)
-   [Touch Point Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2576160.html)
-   [Domain Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159553835589.html)
-   [System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159553904637.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
