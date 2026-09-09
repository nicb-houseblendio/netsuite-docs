---
id: "section_N2554144"
type: "section"
title: "Using a Third-Party Tax Calculator"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Sample Scripts for Scriptable Cart > Using a Third-Party Tax Calculator"
parent: "section_N2553996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554144.html"
anchors: ["bridgehead_N2554171", "bridgehead_N2554183", "bridgehead_N2554353"]
sha256: "6d8766fb327d351acedfe89bdbf84c8c9d521a512bb5efaa205faa838b62ee70"
---

Using SuiteScript, you can send order information to a third-party remote server, and then override the tax settings on the sales order based on calculations returned by a third-party.

## Setup {#bridgehead_N2554171}

The only setup required for this sample script is to replace the sample URL in the script with the URL provided by your third-party tax calculator.

## Create the Code {#bridgehead_N2554183}

          `//BEGIN CUSTOM FUNCTIONS FOR THIRD-PARTY TAX  function customOnChange(type, name, linenum) {` 
        

          `// With third-party tax calculations, it is important to capture and override any tax setting. // The if statement below ensures that tax settings are overridden,but use this technique with // care, as the setTaxAmount() function also sets the tax. It is critical not to trigger a // changeField event in this function, so note that the nlapiSetFieldValue is called with the // appropriate flags.     if (name == 'promocode' || name == 'taxrate')    {       //alert('Onchange called for '+name);       setTaxAmount();    } }   function customRecalc(type, action) {` 
        

          `// In SuiteScript for the web store, action can only be 'commit' or 'remove.'     if (type == 'item')    {       setTaxAmount();    } }  // END CUSTOM FUNCTIONS FOR THIRD-PARTY TAX` 
        

          `// BEGIN THIRD PARTY TAX    function setTaxAmount() {` 
        

          `// Construct an array of values needed by the third-party tax provider to calculate tax.      var postArgs = new Array();    postArgs['zipCode'] = nlapiGetField('shipzip');    postArgs['saleTotal'] = nlapiGetField('subtotal');` 
        

          `//Replace the URL below with your third-party tax provider.      var response = nlapiRequestURL("http://www.thirdpartytaxcalculator.com", postArgs, null, null);    var body = response.getBody();` 
        

          `// Parse tax amount from the body. Your approach depends on the format of your third-party tax provider. // The current script only sets the tax rate of the sales order and does not change the taxable // status of either the customer or any of the items in the order. But, even though the taxable // flags are not overridden by this sample script, you can override these settings if necessary.      var taxRate = body;` 
        

          `// Note here not to use a field-changed event. Firing a field-changed //event may cause an infinite loop since a change to tax-rate will alter itself.      nlapiSetFieldValue('taxrate', taxRate, false /*fire field change*/, true /*synchronous*/); } // END THIRD-PARTY TAX` 
        

## Deploy Your Script to the Shopping Cart {#bridgehead_N2554353}

You should test your script thoroughly before running it in the shopping cart. You must follow a series of steps to load the script into your NetSuite account, and then run the script for testing purposes.

For details, see [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html).

### Related Topics

-   [Creating Buy-One-Get-One-Free Coupons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554377.html)
-   [Dynamic Discounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557130.html)
-   [Offering Gift Wrap on the Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557809.html)
-   [Setting Quantity Limits for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2558716.html)
-   [Creating Time-Based Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2560375.html)
-   [Setting Default Location for Web Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561074.html)
-   [Accepting Charitable Donations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561322.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
