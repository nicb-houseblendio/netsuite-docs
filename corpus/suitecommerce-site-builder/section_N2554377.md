---
id: "section_N2554377"
type: "section"
title: "Creating Buy-One-Get-One-Free Coupons"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Sample Scripts for Scriptable Cart > Creating Buy-One-Get-One-Free Coupons"
parent: "section_N2553996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554377.html"
anchors: ["bridgehead_N2554399", "bridgehead_N2554483", "bridgehead_N2556976"]
sha256: "5648d3e23e3329de25ec799ed2253727a330a3ebcd610b21285da82e79f0c995"
---

Use the Scriptable Cart to create a buy-one-get-one-free sales promotion for the web store.

You can use SuiteScript to add a free item to the order when the shopping cart contains an item you identify as the trigger item. By entering the coupon code you specify in the script, the shopper triggers the addition of the free item to the shopping cart. The script becomes inactive when the coupon expires, or when the item is out of stock.

## Setup {#bridgehead_N2554399}

Use the steps below to create the promotion code and set up the item records required to run the sample script.

This sample script is triggered to add a free computer mouse to the order, when the shopper enters BOGO as the coupon code, and the computer system exists in the shopping cart.

To use the code sample successfully, you must complete the following setup steps.

1.  Create a promotion code named **BOGO**. Entering the coupon code will trigger the script to run.
    
    Go to _Commerce > Marketing > Upsell > Promotions_. For more information about entering promotion codes, see [Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4690873883.html).
    
2.  Select the item that must be in the shopping cart to receive the free item.
    
    Go to Lists > Items. Click **Edit** next to an item.
    
    This item's internal ID must be referenced in the script. In the code sample below, this is the Impressivo System (internal ID 5).
    
3.  Select an item to offer free of charge when the Impressivo System is added to the cart.
    
    Go to Lists > Items. Click **Edit** next to an item.
    
    Reference the internal ID for the free item in the script. The free item in the sample is a computer mouse (internal ID 59)
    

Note:

When you use SuiteScript to set quantity and price, you must set quantity first, and then set the price.

## Create the Code {#bridgehead_N2554483}

          `// BEGIN CUSTOM FUNCTIONS FOR BOGO  function customInit(type) { //nlapiLogExecution('ERROR', 'Logging is working', 'Message from script using new execute log API'); return; }` 
        

          `// Note that the customOnChange function will trigger on a FieldChanged client event.  function customOnChange(type, name, linenum) { if (name == 'promocode') { bogo('commit'); } } function customRecalc(type, action) {` 
        

          `// In SuiteScript for the web store, action can only be 'commit' or 'remove.'  if (type == 'item') { bogo(action); } } // END CUSTOM FUNCTION FOR BOGO` 
        

          `// BEGIN BOGO  function bogo(action) {    var mouseId = 59;    var impressivoId = 5;    var promoEnabled = isNotEmpty(nlapiGetFieldText('promocode')) && nlapiGetFieldText('promocode') == 'BOGO';` 
        

          `// Verify the computer (Impressivo) and the free mouse exist in the list of items in the order.   var freeMouseLine = -1;    var freeMouseQty = 0;      var impressivoLine = -1;    var impressivoQty = 0;    var numItems = nlapiGetLineItemCount('item');` 
        

          `// Do not do any processing if adding a free mouse. if (nlapiGetCurrentLineItemValue('item', 'item') == mouseId &&       nlapiGetCurrentLineItemValue('item', 'rate') == 0 && action == 'commit')    {       debug('Adding free mouse - no processing');       return;    }` 
        

          `// Search the sales order for the trigger item and the free item. for (var line = 1; line <= numItems; line++)    {       var itemId = nlapiGetLineItemValue('item','item',line);       var itemQty = parseInt(nlapiGetLineItemValue('item', 'quantity', line));` 
        

          `// If a mouse is found with a rate of 0.00, this is the free mouse. if (itemId == mouseId && nlapiGetLineItemValue('item','rate',line) == 0)       {          freeMouseLine = line;          freeMouseQty = freeMouseQty + itemQty;       }` 
        

          `// If an Impressivo is found, remember the line number and quantity. if (itemId == impressivoId)       {          impressivoLine = line;          impressivoQty = impressivoQty + itemQty;       }    }    debug('Action '+action+' mouse line='+freeMouseLine+' qty='+freeMouseQty+' impressivo line='+impressivoLine+' qty='+impressivoQty);` 
        

          `// If the shopper enters the BOGO coupon, and the Impressivo is in the shopping cart, and the // free mouse is not in the shopping cart, add the mouse to the shopping cart free of charge. if (promoEnabled && impressivoLine > 0 && freeMouseLine < 0 && action == 'commit')    {       debug('Adding free mouse');` 
        

          `// Insert the mouse        nlapiSelectNewLineItem('item');       nlapiSetCurrentLineItemValue('item', 'item', mouseId, true, true);       nlapiSetCurrentLineItemValue('item', 'quantity', impressivoQty, true, true);       setCurrentLineRate(0);` 
        

          `var desc = nlapiGetCurrentLineItemValue('item','description');       nlapiSetCurrentLineItemValue('item','description', desc+' (FREE)', true, true);       desc = nlapiGetCurrentLineItemValue('item','description');       debug('New description is '+desc);       nlapiCommitLineItem('item');    }` 
        

          `// If the BOGO coupon is no longer valid, and the shopping cart contains the free mouse and     // the Impressivo computer, remove the free mouse. if (!promoEnabled && action == 'commit' && impressivoQty > 0 && freeMouseLine > 0)    {       debug('Selecting free mouse line');       nlapiSelectLineItem('item', freeMouseLine);       debug('Deleting free mouse on line '+freeMouseLine+' because of change in promo code');       nlapiRemoveLineItem('item', freeMouseLine);    }` 
        

          `// If the trigger item (Impressivo computer) is deleted from the cart, then remove the free mouse form the shopping cart.  if (action == 'remove' && impressivoLine < 0 && freeMouseLine > 0)    {       debug('Selecting free mouse line');       nlapiSelectLineItem('item', freeMouseLine);       debug('Deleting free mouse on line '+freeMouseLine+' because of deletion of the impressivo'); nlapiRemoveLineItem('item', freeMouseLine); }` 
        

          `// If the trigger item quantity does not match the free item quantity in the cart, then update // free item quantity to match the trigger item quantity.  if (action == 'commit' && impressivoLine > 0 && freeMouseLine > 0 && impressivoQty != freeMouseQty) { debug('Updating mouse quantity to '+impressivoQty); nlapiSelectLineItem('item', freeMouseLine); nlapiSetCurrentLineItemValue('item', 'quantity', impressivoQty, true, true); nlapiCommitLineItem('item'); } debug('Bogo script complete'); } function debug(msg) { alert(msg); } // END BOGO` 
        

          `// BEGIN UTILITY FUNCTIONS  function isEmpty(val) { return (val == null || val == ''); } function isNotEmpty(val) { return !isEmpty(val); } function getVal(colName, linenum) { return nlapiGetLineItemValue('item',colName,linenum); }` 
        

          `// This function updates the rate and also recalculates the correct value for amount.  function setCurrentLineRate(rate) { nlapiSetCurrentLineItemValue('item', 'rate', rate, true, true); var qty = parseInt(nlapiGetCurrentLineItemValue('item', 'quantity')); var amount = qty * rate; nlapiSetCurrentLineItemValue('item', 'amount', amount, true, true); }` 
        

          `// This function returns a map with the internal ID for the item as the //key  and the totalquantity for that item in the value. It sums items  //when the same item appears on different lines on the sales order.  //If passed a non-null filter value, item types that match the filter are excluded. function getItemMap(excludeFilter) { if (isNotEmpty(excludeFilter)) { debug('getItemMap called with filter '+excludeFilter); } var itemMap = new Array(); var numLines = nlapiGetLineItemCount('item'); for (var i=1; i<= numLines; i++) {` 
        

          `// Include only items that match the filter.  var itemType = nlapiGetLineItemValue('item','itemtype',i); if (isNotEmpty(excludeFilter) && itemType == excludeFilter) { debug('Ignoring line '+i+', itemType '+itemType+' excluded'); continue; } var itemId = nlapiGetLineItemValue('item','item',i); var nextQty = parseInt(nlapiGetLineItemValue('item','quantity',i)); debug('Item'+itemId+' of type '+itemType+' added to item map'); if (itemId in itemMap) {` 
        

          `// Add the quantities if other lines in the sublist include the same item.  nextQty = nextQty + parseInt(itemMap[itemId]); } debug('Item Id '+itemId+' has updated quantity to '+nextQty+' because of line #'+i); itemMap[itemId] = nextQty; } return itemMap; }` 
        

          `// This function rounds the input to two decimal places.  function roundOff(amount) {    return Math.round(amount*100000)/100000; } // END UTITLITY FUNCTIONS` 
        

## Deploy Your Script to the Shopping Cart {#bridgehead_N2556976}

Test your script thoroughly before running it in the shopping cart. You must follow a series of steps to load the script into your NetSuite account, and then run the script for testing purposes.

For details, see [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html).

.

### Related Topics

-   [Using a Third-Party Tax Calculator](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554144.html)
-   [Dynamic Discounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557130.html)
-   [Offering Gift Wrap on the Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557809.html)
-   [Setting Quantity Limits for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2558716.html)
-   [Creating Time-Based Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2560375.html)
-   [Setting Default Location for Web Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561074.html)
-   [Accepting Charitable Donations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561322.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
