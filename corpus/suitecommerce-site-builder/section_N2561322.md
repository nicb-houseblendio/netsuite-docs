---
id: "section_N2561322"
type: "section"
title: "Accepting Charitable Donations"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Sample Scripts for Scriptable Cart > Accepting Charitable Donations"
parent: "section_N2553996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561322.html"
anchors: ["bridgehead_N2561344", "bridgehead_N2561493", "bridgehead_N2561616"]
sha256: "47c4f5c942fbafa901555828fa9c302cd63f92cd369fe34b75f86608f123bc5f"
---

Use SuiteScript to accept charitable contributions on your website.

Create an item record for display on the web store as a charitable donation item. The shopper adds this item to the shopping cart and enters an amount of donation. After the item is added to the cart, the total amount of the order is recalculated to include the non taxable donation.

## Setup {#bridgehead_N2561344}

Use these steps to create the charitable donation item record and custom item options needed to run the sample script. You must finish the following steps to use the code sample successfully.

1.  Create a non-inventory item for sale. This will be the Charitable Contribution item displayed on the web store.
    
    1.  Go to Lists > Items > New. Click Non-inventory For Sale.
        
    2.  Check the **Display in Web Site** box.
        
    3.  On the **Pricing** subtab, set the base price to 0.00.
        
    4.  On the **Store** subtab, select a **Site Category** to display the item on your website.
        
        Note:
        
        By default, items that do not have a price specified on the item record, display a default message on the web store. To change this message, go to Commerce > Site Builder > Customize Text.
        
        On the **Messages** subtab, enter a custom message to replace the value in the **Default Text** column.
        
2.  Create a transaction item option custom field linked to the Charitable Contribution item you created in Step1.
    
    1.  Go to Customization > Lists, Records, & Fields > Transaction Item Options.
        
    2.  In the **Label** field, enter a name for this item option.
        
    3.  In the **ID** field, enter **\_contribution**.
        
        Note:
        
        After you save the transaction item option, the value for ID automatically changes to **custcol\_contribution**. The sample script depends on this value for ID.
        
    4.  On **Applies To** subtab, check the **Web Store** box, and the **Sale** box.
        
    5.  In the **Items** multiple select list, choose the item created in Step 1.
        

## Create the Code {#bridgehead_N2561493}

          `// BEGIN CUSTOM FUNCTIONS FOR CHARITABLE CONTRIBUTIONS  function customValidateLine(type) {` 
        

          `// All validations occur in the item tab.     if (type != 'item')    {       return true;    }` 
        

          `// Note that validation routines are called differently from other events, because the return // value of each function must be tested before going on to the next function. If any function // returns false, stop processing and return false.      if (!charity())    {       return false;    }` 
        

          `// All validations passed. Return true.     return true; } //END CUSTOM FUNCTIONS FOR CHARITY CONTRIBUTION` 
        

          `//CHARITY CONTRIBUTION  function charity() {` 
        

          `// Internal ID of the charity item record.     var charityId = 384;` 
        

          `// Ignore any items other than the charity item record.     if (charityId != nlapiGetCurrentLineItemValue('item', 'item'))    {       return true;    }      debug('Charity item detected');` 
        

          `// Validate that the amount in the custom field is greater than zero.     var contribAmount = nlapiGetCurrentLineItemValue('item','custcol_contribution');      debug('Contribution '+contribAmount+' read in');      if (isEmpty(contribAmount) || contribAmount <= 0)    {       alert('You must contribute an amount that is greater than zero!');       return false;    }      debug('Contribution valid - setting the item rate');` 
        

          `// Set the price of the line item to the contribution amount.     setCurrentLineRate(contribAmount);      return true; } //END CHARITY CONTRIBUTION` 
        

          `//BEGIN UTILITY FUNCTIONS  function isEmpty(val) {    return (val == null || val == ''); }   function isNotEmpty(val) {    return !isEmpty(val); }` 
        

          `// This function updates the rate and recalculates the value for amount.  function setCurrentLineRate(rate) {    nlapiSetCurrentLineItemValue('item', 'rate', rate, true, true);    var qty = parseInt(nlapiGetCurrentLineItemValue('item', 'quantity'));    var amount = qty * rate;    nlapiSetCurrentLineItemValue('item', 'amount', amount, true, true); } //END UTILITY FUNCTIONS` 
        

## Deploy Your Script to the Shopping Cart {#bridgehead_N2561616}

Test your script thoroughly before running it in the shopping cart. You must follow a series of steps to load the script into your NetSuite account, and then run the script for testing purposes.

For details, see [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html).

### Related Topics

-   [Using a Third-Party Tax Calculator](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554144.html)
-   [Creating Buy-One-Get-One-Free Coupons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554377.html)
-   [Dynamic Discounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557130.html)
-   [Offering Gift Wrap on the Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557809.html)
-   [Setting Quantity Limits for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2558716.html)
-   [Creating Time-Based Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2560375.html)
-   [Setting Default Location for Web Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561074.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
