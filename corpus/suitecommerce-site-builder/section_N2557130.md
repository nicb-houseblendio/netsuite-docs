---
id: "section_N2557130"
type: "section"
title: "Dynamic Discounts"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Sample Scripts for Scriptable Cart > Dynamic Discounts"
parent: "section_N2553996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557130.html"
anchors: ["bridgehead_N2557178", "bridgehead_N2557586", "bridgehead_N2557722"]
sha256: "d746b90d5bd7d8a255eabf06696673bffbd2209be926141f5d3125e72a950d75"
---

Use SuiteScript to apply a discount to an order when the total in the shopping cart reaches or exceeds the threshold order amount that you set for each currency you use online.

There are two different approaches you can use:

-   Create a discount item for applying the discount to web orders.
    
    Reference this discount item in your script. The advantage of using this approach is that the discount is subtracted from the total amount in the cart, so the order subtotal is consistent between the cart and the order confirmation page. Also, the shopper can override the discount by entering a promotion code. This approach is used in the sample script provided here.
    
-   Create a promotion code to use in your script for applying the discount.
    
    Based on the total order amount in the shopping cart, your script changes whatever promotion code the shopper entered to the promotion code you created. The promotion code that triggers the discount is visible to shoppers, so they can share it.
    

## Setup {#bridgehead_N2557178}

Use the steps below to create the discount item and the custom records required to run the sample script.

1.  Create a discount item record. The value you enter in the **Rate** field is the discount amount applied to all orders that reach or exceed the threshold amount you set.
    
    -   Go to Lists > Accounting > Items > New.
        
    -   Select **Discount**.
        
    -   Enter a name for the discount, select an **Account**, and enter a value in the **Rate** field.
        
    -   Click **Save**.
        
2.  Create a new custom record type to track the order amount required to receive a discount for each currency you use on your web store.
    
    1.  Go to Customization > Lists, Records, & Fields > Record Type > New.
        
    2.  In the **Label** field, enter a name for this custom record.
        
    3.  In the **ID** field enter **\_threshold**.
        
        Note:
        
        After you save the custom record, the value for ID automatically changes to **custrecord\_threshold**. The sample script depends on this value for ID.
        
    4.  Check the following boxes on the Custom Record Type page: **Include Name**, **Use Permissions**, and **Show Notes**. Clear all other check boxes.
        
    5.  On the Permissions subtab set permissions as described below. Note that your script will rely upon the permissions you set here to access information in the custom records.
        
        -   Select **Shopper** in the **Role** column; set the **Level** column to **View**. Click **Done**.
            
        -   Select **Customer Center** in the **Role** column; set the **Level** column to **View**. Click **Done**.
            
3.  Click **Save**.
    
4.  On the **Fields** subtab, click **New Fields** to add two new fields to this custom record.
    
    1.  The first field is **Threshold Currency** this is a list field where you can select each currency exposed in your web store. Later, you will link this field to the threshold amount an order must exceed to receive the discount.
        
        -   In the **Label** field, enter **Threshold Currency**.
            
        -   In the **ID** field, enter **\_currencyid**.
            
            Note:
            
            After you save the new field, the value for ID automatically changes to **custrecord\_currencyid**. The sample script depends on this value for ID.
            
        -   In the **Type** list, select **List/Record**.
            
        -   For **List/Record**, select **Currency**.
            
            Note:
            
            Currency only displays as an option in this list if you use the Multiple Currencies feature.
            
        -   Check the **Store Value** box and the **Show in List** box.
            
        -   On the **Validation & Defaulting** subtab, check the **Mandatory** box.
            
        -   On the **Access** subtab, set **Default Access** Level to **Edit**. Also set the **Default Level** for **Search/Reporting** to **Edit**.
            
        -   Click **Save**.
            
    2.  The second field on the custom record is **Discount Threshold**. This field will contain the order total amount required in the shopping cart to receive the discount.
        
        -   In the **Label** field, enter **Discount Threshold**.
            
        -   In the **ID** field, enter **\_discount\_threshold**.
            
            Note:
            
            After you save the new field, the value for ID automatically changes to **custrecord\_discount\_threshold**. The sample script depends on this value for ID.
            
        -   In the **Type** list, select **Currency**.
            
        -   Check the **Store Value** box and the **Show in List** box.
            
        -   On the **Validation & Defaulting** subtab, check the **Mandatory** box.
            
        -   On the **Access** subtab, set **Default Access Level** to **Edit**. Also set the **Default Level for Search/Reporting** to **Edit**.
            
        -   Click **Save**.
            
5.  Go to Customization > Lists, Records, & Fields > Record Types. Click on the custom record you created in Step 1.
    
6.  On the Custom Record Type page, click **View Records**.
    
7.  Click **New** at the bottom of the page to enter records for each currency available on your website.
    
    For example, if you use two currencies, USA and Euro, create two records for this custom record type each named for a different currency. On each record, select the appropriate currency in the Threshold Currency list. Next, in the Discount Threshold field, enter the amount shoppers must reach or exceed to receive the discount.
    

## Create the Code {#bridgehead_N2557586}

          `// BEGIN CUSTOM FUNCTIONS FOR DYNAMIC DISCOUNT  function customOnChange(type, name, linenum) {    if (name == 'promocode')    {       calculateDiscount();    } }   function customRecalc(type, action) {` 
        

          `// On the web store, action can only be 'commit' or 'remove'.     if (type == 'item')    {       calculateDiscount();    } }  // END CUSTOM FUNCTIONS FOR DYNAMIC DISCOUNT` 
        

          `// DYNAMIC DISCOUNT  function calculateDiscount() {` 
        

          `// ID of the discount that will be applied.    var discountId = 383;    var currencyId = nlapiGetFieldValue('currency');    var customerId = nlapiGetFieldValue('entity');        if (isEmpty(currencyId) || isEmpty(customerId) || customerId == '0')    {       return;    } //Load custom threshold record for this currency` 
        

          `debug('Loading threshold record for currency id '+currencyId);    var filter = new nlobjSearchFilter('custrecord_currencyid', null, 'is', currencyId);    var column = new nlobjSearchColumn('custrecord_discount_threshold');    var searchresults = nlapiSearchRecord('customrecord_threshold', null, filter, column);    var subtotal = parseFloat(nlapiGetFieldValue('subtotal'));    debug('Subtotal is '+subtotal);` 
        

          `// If there is no value for threshold associated with a currency or discount, remove the // discount line. if (isEmpty(searchresults))    {       debug('No threshold for this currency, removing discount');       nlapiSetFieldValue('discountitem', '');    }      if (isNotEmpty(searchresults))    {` 
        

          `// Get the threshold value and current subtotal. var threshold = searchresults[0].getValue('custrecord_discount_threshold');       debug('Threshold for this currency is '+threshold);` 
        

          `// If a threshold exists, and the promotion code does not exist, then add a promocode when the // threshold is exceeded. if (subtotal >= threshold)       {          debug('Our subtotal '+subtotal+' is over the threshold of '+threshold+' - adding discount');          nlapiSetFieldValue('discountitem', discountId);       }` 
        

          `// If a threshold value exists, and the promotion code exists, then remove the discount line // when the order total is below the threshold. if (subtotal < threshold)       {          debug('Subtotal below threshold of '+threshold+' - removing discount');          nlapiSetFieldValue('discountitem', '');       }    } }` 
        

          `// BEGIN UTILITY FUNCTIONS  function isEmpty(val) {    return (val == null || val == ''); }   function isNotEmpty(val) {    return !isEmpty(val); }   function getVal(colName, linenum) {    return nlapiGetLineItemValue('item',colName,linenum); }   function debug(val) {    nlapiLogExecution('DEBUG', val); } // END UTILITY` 
        

## Deploy Your Script to the Shopping Cart {#bridgehead_N2557722}

Test your script thoroughly before running it in the shopping cart. You must follow a series of steps to load the script into your NetSuite account, and then run the script for testing purposes.

For details, see [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html).

### Related Topics

-   [Using a Third-Party Tax Calculator](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554144.html)
-   [Creating Buy-One-Get-One-Free Coupons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554377.html)
-   [Offering Gift Wrap on the Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557809.html)
-   [Setting Quantity Limits for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2558716.html)
-   [Creating Time-Based Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2560375.html)
-   [Setting Default Location for Web Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561074.html)
-   [Accepting Charitable Donations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561322.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
