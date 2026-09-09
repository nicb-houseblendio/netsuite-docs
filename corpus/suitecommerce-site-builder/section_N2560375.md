---
id: "section_N2560375"
type: "section"
title: "Creating Time-Based Promotions"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Sample Scripts for Scriptable Cart > Creating Time-Based Promotions"
parent: "section_N2553996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2560375.html"
anchors: ["bridgehead_N2560394", "bridgehead_N2560911", "bridgehead_N2561050"]
sha256: "0c55290fde2b9bcac3f71bf6798827591c20c72aceba42298f55ea1725dddc54"
---

You can offer items online for a special sale price that is valid only for a set amount of time. The script you create recognizes the date and time when the sale price is no longer valid, and reverts the price displayed online back to the original.

## Setup {#bridgehead_N2560394}

Follow the setup steps below to create three custom item fields and three corresponding item option fields that display information about the discount to shoppers on your web store.

1.  Create three custom item fields.
    
    Go to Customization > Lists, Records, & Fields > Item Fields > New. In the sample script, custom item fields were created as follows:
    
    1.  Discount Price
        
        -   In the **Label** field, enter **Discount Price**.
            
        -   In the **ID** field, **enter \_discountprice**.
            
            Note:
            
            After you save the custom item field, the value for ID automatically changes to **custitem \_discountprice**. The sample script depends on this value for ID.
            
        -   Set **Type** to **Currency**
            
        -   Check the **Store Value** box.
            
        -   On the **Applies To** subtab, check the boxes next to the item type for which you will offer this discount.
            
        -   Click **Save**.
            
    2.  Discount Expiration Date
        
        -   In the **Label** filed, enter **Discount Expiration Date**.
            
        -   In the **ID** field, **enter \_discountexpirationdate**.
            
            Note:
            
            After you save the custom item field, the value for ID automatically changes to **custitem \_discountexpirationdate**. The sample script depends on this value for ID.
            
        -   Set **Type** to **Date**.
            
        -   Check the **Store Value** box.
            
        -   On the **Applies To** subtab, check the boxes next to the item type for which you will offer this discount.
            
    3.  Discount Expiration Time
        
        -   In the **Label** field, enter **Discount Expiration Time**.
            
        -   In the **ID** field, enter **\_discountexpirationtime**.
            
            Note:
            
            After you save the custom item field, the value for ID automatically changes to **custitem \_discountexpirationtime**. The sample script depends on this value for ID.
            
        -   Set **Type** to **Time of Day**.
            
        -   On the **Applies To** subtab, check the boxes next to the item type for which you will offer this discount.
            
2.  Create three transaction item options at Customization > Lists, Records, & Fields > Transaction Item Options.
    
    Note:
    
    Shoppers on your web store will see the fields you create below. Create field labels for these transaction item options and set the order in which they display so that they make sense to online shoppers.
    
    1.  Discount Price Column
        
        -   In the **Label** field, enter **Special Sale Price**.
            
        -   In the **ID** field, enter **\_discountprice**.
            
            Note:
            
            After you save the custom item option, the value for ID automatically changes to **custcol \_discountprice**. The sample script depends on this value for ID.
            
        -   Set the **Type** field to **Currency**.
            
        -   Check the **Store Value** box.
            
        -   On the **Applies to** subtab, check the **Sale** and **Web Store** boxes.
            
        -   On the **Display** tab, set **Display Type** to **Disabled**.
            
        -   On the **Sourcing & Filtering** subtab, set **Source List** to **Item**, and **Source From** to **Discount Price**.
            
        -   Click **Save**.
            
    2.  Discount Expiration Date
        
        -   In the **Label** field, enter **Special sale ends on**.
            
        -   In the **ID** field, enter **\_discountexpirationdate**.
            
            Note:
            
            After you save the custom item option, the value for ID automatically changes to **custcol \_discountexpirationdate**. The sample script depends on this value for ID.
            
        -   Set **Type** to **Date**.
            
        -   Check the **Store Value** box.
            
        -   On the **Applies to** subtab, check the **Sale** box, and the **Web Store** box.
            
        -   On the **Display** tab, set **Display Type** to **Disabled**.
            
        -   On the **Sourcing & Filtering** subtab, set **Source List** to **Item**, and **Source From** to **Discount Expiration Date**.
            
        -   Click **Save**.
            
    3.  Discount Expiration Time
        
        -   In the **Label** Field, enter **Discount expires at**.
            
        -   In the **ID** field, enter **\_discountexpirationtime**.
            
            Note:
            
            After you save the custom item option, the value for ID automatically changes to **custcol \_discountexpirationtime**. The sample script depends on this value for ID.
            
        -   Set the **Type** field to **Time of Day**.
            
        -   On the **Applies to** subtab, check the **Sale** box and the **Web Store** box.
            
        -   On the Display tab, set Display Type to Disabled.
            
        -   On the **Sourcing & Filtering** subtab, set **Source List** to **Item**, and **Source From** to **Discount Expiration Time**.
            
        -   Click **Save**.
            

## Create the Code {#bridgehead_N2560911}

          `// BEGIN CUSTOM FUNCTIONS FOR TIME BASED DISCOUNT  function customValidateLine(type) {` 
        

          `// All validations occur in the item tab.     if (type != 'item')    {       return true;    }` 
        

          `// Note that validation routines are called differently from other events, because the return // value of each function must be tested before going on to the next function. If any function // returns false, stop processing and return false.     if (!applyTimedDiscount())    {       return false;    }` 
        

          `// All validations passed, so return true     return true; } // END CUSTOM FUNCTIONS FOR TIME BASED DISCOUNT` 
        

          `//BEGIN TIME BASED DISCOUNT  function applyTimedDiscount() {` 
        

          `// First get the current date and time.     var now = new Date();` 
        

          `// Next, get the expiration date and time from the current line.     var expDate = nlapiGetCurrentLineItemValue('item','custcol_discountexpirationdate');    var expTime = nlapiGetCurrentLineItemValue('item','custcol_discountexpirationtime');    var discountPrice = nlapiGetCurrentLineItemValue('item','custcol_discountprice');      if (isEmpty(expDate) || isEmpty(expTime) || isEmpty(discountPrice))    {` 
        

          `// If the information is incomplete, do not give a discount for this item.        return true;    }      var expDateTime = new Date(expDate+' '+expTime);      alert('Expiration date time is '+expDateTime);      if (now.getTime() < expDateTime.getTime())    {` 
        

          `// Override the current price with the discount price.        alert('Discount applies - set the new price of '+discountPrice);       setCurrentLineRate(discountPrice);    }` 
        

          `// If the promotion has ended, do not to throw an error. Instead, add the item at regular price // to the order.      return true; }` 
        

          `// UTILITY FUNCTIONS  function isEmpty(val) {    return (val == null || val == ''); }   function isNotEmpty(val) {    return !isEmpty(val); }` 
        

          `// This function will update the rate and also recalculate the correct value for amount.  function setCurrentLineRate(rate) {    nlapiSetCurrentLineItemValue('item', 'rate', rate, true, true);    var qty = parseInt(nlapiGetCurrentLineItemValue('item', 'quantity'));    var amount = qty * rate;    nlapiSetCurrentLineItemValue('item', 'amount', amount, true, true); }` 
        

## Deploy Your Script to the Shopping Cart {#bridgehead_N2561050}

NetSuite recommends that you test your script thoroughly before running it in the shopping cart. You must follow a series of steps to load the script into your NetSuite account, and then run the script for testing purposes.

For details, see [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html).

### Related Topics

-   [Using a Third-Party Tax Calculator](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554144.html)
-   [Creating Buy-One-Get-One-Free Coupons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554377.html)
-   [Dynamic Discounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557130.html)
-   [Offering Gift Wrap on the Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557809.html)
-   [Setting Quantity Limits for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2558716.html)
-   [Setting Default Location for Web Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561074.html)
-   [Accepting Charitable Donations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561322.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
