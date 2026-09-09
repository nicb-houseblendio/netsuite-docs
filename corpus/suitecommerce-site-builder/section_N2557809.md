---
id: "section_N2557809"
type: "section"
title: "Offering Gift Wrap on the Web Store"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Sample Scripts for Scriptable Cart > Offering Gift Wrap on the Web Store"
parent: "section_N2553996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557809.html"
anchors: ["bridgehead_N2557835", "bridgehead_N2558387", "bridgehead_N2558661"]
sha256: "b8aceac29ce35640e7f3d4a07c2de6ba051b96dc1691ddbf97952ec202ec6995"
---

The code sample below depends on a custom item field you create that contains the gift wrap price. When the shopper in the web store checks a box on an item record, the script adds a line item for gift wrap to the sales order.

Important:

Per line item taxing must be disabled to use scriptable cart for offering gift wrap in the web store. Note that when the charge for gift wrap is inserted into the sales order, a tax code is not specified for per line item taxing.

## Setup {#bridgehead_N2557835}

Use the steps below to create the custom fields, and the gift wrap item record required to run the sample script.

1.  Create a custom field on item records for giftwrap pricing.
    
    1.  Go to Customization > Lists, Records, & Fields > Item Fields > New.
        
    2.  In the Label field, enter **Gift Wrap Price**.
        
    3.  On the **Applies To** subtab, check the boxes for the item types you offer for sale online.
        
    4.  In the **Type** list, select **Currency**.
        
    5.  Click **Save**.
        
2.  Create a transaction item option on item records to show the value you enter in the Gift Wrap Price field.
    
    1.  Go to Customization > Lists, Records, & Fields > Transaction Item Options > New.
        
    2.  In the **Label** field, enter **Gift Wrap Cost**.
        
    3.  In the **ID** field, enter **giftwrapcost**.
        
        Note:
        
        After you save the transaction item option, the value for ID automatically changes to **custcolgiftwrapcost**. The sample script depends on this value for ID.
        
    4.  In the **Type** list, select **Currency**.
        
    5.  On the **Applies To** subtab:
        
        -   Check the **Sale** box.
            
        -   Check the **Web Store** box.
            
        -   In the **Items** list, select the items for which you offer gift wrap
            
    6.  On the **Display** subtab, set **Display type** to disabled. This step prevents shoppers on the web store shopper from changing the gift wrap price you set.
        
    7.  On the **Sourcing & Filtering** subtab:
        
        -   Set the **Source List** to **Item**.
            
        -   Select **Gift Wrap Price** in the **Source From** list.
            
    8.  Click **Save**.
        
3.  Create a second transaction item option to display a check box on the web store where shoppers can trigger the script by flagging an item for gift wrap.
    
    1.  Go to Customization > Lists, Records, & Fields > Transaction Item Options > New.
        
    2.  In the **Label** field, enter **Gift Wrap**.
        
    3.  In the **ID** field, enter **giftwrapped**.
        
        Note:
        
        After you save the transaction item option, the value for ID automatically changes to **custcolgiftwrapped**. The sample script depends on this value for ID.
        
    4.  Set the **Type** list to **Check box**.
        
    5.  On the **Applies to** subtab:
        
        -   Check the **Sale** box.
            
        -   Check the **Web Store** box.
            
        -   Select the items for which you offer gift wrap in the Items list.
            
    6.  Click **Save**.
        
4.  Create the gift wrap item record to be added to orders where the shopper checked the Gift Wrap box.
    
    1.  Go to Lists > Accounting > Items > New.
        
    2.  Select a **Non-inventory Item** type.
        
    3.  In the **Item Name/Number** field, enter **Gift Wrap**.
        
    4.  Check the **Display in Web Site** box. This is required so the gift wrap item can be added to the cart along with the item to be gift wrapped.
        
    5.  Enter a price on the item record.
        
    6.  Click **Save**.
        
        Note:
        
        Remember the internal ID number for this gift wrap item. You will use it in the Scriptable Cart code sample.
        
5.  Create a third transaction item option for the script to capture the internal ID for the gift wrap item record. This field is not visible to shoppers.
    
    1.  Go to Customization > Lists, Records, & Fields > Transaction Item Options > New
        
    2.  In the **Label** field, enter **Gift Wrap Item ID**.
        
    3.  In the **ID** field, enter **giftwrapitemid**.
        
        Note:
        
        After you save the transaction item option, the value for ID automatically changes to **custcolgiftwrapitemid**. The sample script depends on this value for ID.
        
    4.  Set the **Type** list to **Free-Form Text**.
        
    5.  On the **Applies to** subtab:
        
        -   Check the **Sale** box.
            
        -   Check the **Web Site** box.
            
        -   Check the **Hidden** box.
            
    6.  On the **Display** subtab, set **Display Type** to **Hidden**.
        
    7.  Click **Save**.
        
6.  Create a transaction body field to detect recursion of the `recalc` function. Using this flag allows new lines to be inserted into the item machine without triggering the script to run multiple times.
    
    1.  Customization > Lists, Records, & Fields > Transaction Body Field > New.
        
    2.  In the **Label** field, enter **processing**.
        
    3.  In the **ID** field, enter **processing**.
        
        Note:
        
        After you save the transaction item option, the value for ID automatically changes to **custbodyprocessing**. The sample script depends on this value for ID.
        
    4.  On the **Applies to** subtab, check the **Sale** box.
        
    5.  On the **Display** subtab, set **Display Type** to Hidden.
        
    6.  Click **Save**.
        

## Create the Code {#bridgehead_N2558387}

          `//BEGIN CUSTOM FUNCTIONS FOR GIFT WRAP  function customRecalc(type, action) {` 
        

          `// In Scriptable Cart, action can only be 'commit' or 'remove'.  if (nlapiGetFieldValue('custbodyprocessing') == "T") {return;} nlapiSetFieldValue('custbodyprocessing', "T"); if (type == 'item') {    try    {       recalcGiftWrap(action);    }    finally    {       nlapiSetFieldValue('custbodyprocessing',"F");  } } //END CUSTOM FUNCTIONS FOR GIFT WRAP` 
        

          `//BEGIN GIFT WRAP  function recalcGiftWrap(action) {    debug('Giftwrap recalc called for '+action);` 
        

          `// Substitute the internal ID for the gift wrap item you created in your account. var giftwrapId = 386;` 
        

          `// Array of gift wrapped items and their quantities. var wrappedItemsQty = new Array();` 
        

          `// Array of internal item IDs and their associated gift wrap prices and their corresponding gift  // wrap line numbers.    var wrapCost = new Array();    var itemDesc = new Array();    var wrapLines = new Array();    var numlines = nlapiGetLineItemCount('item');    debug('numlines = '+numlines);    for (var i=1; i <= numlines; i++)    {       var itemId = getVal('item', i);` 
        

          `// If a line with gift wrap is found, then note the line and go to the next line.   if (itemId == giftwrapId)       {          var relatedItemId = getVal('custcolgiftwrapitemid', i);          wrapLines[relatedItemId] = i;          continue;       }         if (isEmpty(getVal('custcolgiftwrapcost', i)))       {` 
        

          `// Ignore any items with no gift wrap cost.           debug("ignoring line "+i+", giftwrapcost is "+getVal('custcolgiftwrapcost', i));          continue;       }` 
        

          `// Store the gift wrap cost and description for this item.     wrapCost[itemId] = getVal('custcolgiftwrapcost', i);` 
        

          `// This item has a gift wrap cost, so accumulate it in our map.        var lineQty = parseInt(getVal('quantity', i));` 
        

          `// Count this row as zero if the gift wrap check box is false and remove any gift wrap items that are not needed.        if (getVal('custcolgiftwrapped',i) == 'F') { lineQty = 0; }         if (itemId in wrappedItemsQty)` 
        

          `// Accumulate the quantity.        {          wrappedItemsQty[itemId] = wrappedItemsQty[itemId] + lineQty;       }       else       {          wrappedItemsQty[itemId] = lineQty;` 
        

          `// Initialize.        }       debug('Accumulated giftwrap qty for item '+itemId+' is '+wrappedItemsQty[itemId]);    }` 
        

          `// Look at each giftwrapped item and make sure that the quantities are correct. for (var nxtItem in wrappedItemsQty)    {       var numWrapsNeeded = wrappedItemsQty[nxtItem];       debug(numWrapsNeeded+' wraps needed for item '+nxtItem);` 
        

          `// If a row exists for an item that includes gift wrap, check if it needs to be updated.        if (nxtItem in wrapLines)       {          var giftWrapLineNum = wrapLines[nxtItem];          var numWrapsCurrent = getVal('quantity', wrapLines[nxtItem]);` 
        

          `// Update the quantity on the gift wrap item if needed.           if (numWrapsCurrent != numWrapsNeeded)          {             debug('Update to '+numWrapsNeeded+ ' giftwraps needed for item ID '+nxtItem+' line '+giftWrapLineNum);             nlapiCommitLineItem('item');             nlapiSelectLineItem('item',giftWrapLineNum);             nlapiSetCurrentLineItemValue('item', 'quantity', numWrapsNeeded,true); debug('Current Gift Wrap Quantity is ' + nlapiGetCurrentLineItemValue('item','quantity'));             nlapiCommitLineItem('item');          }       }       else if (numWrapsNeeded > 0)` 
        

          `// If a gift wrap item does not exist, but it is needed, insert it.    {          debug('Insert '+numWrapsNeeded+' giftwraps found for item ID '+nxtItem);          nlapiSelectNewLineItem('item');          nlapiSetCurrentLineItemValue('item', 'item', giftwrapId, true , true);` 
        

          `// Set quantity first, and rate second, because changing quantity automatically updates the rate.           nlapiSetCurrentLineItemValue('item', 'quantity', numWrapsNeeded, false , true);          setCurrentLineRate(wrapCost[nxtItem]);          nlapiSetCurrentLineItemValue('item', 'custcolgiftwrapitemid', nxtItem, false, true);          nlapiCommitLineItem('item');       }    }` 
        

          `// Finally, look for orphan gift wrap items and delete them.     for (var nxtItem in wrapLines)    {       if (!(nxtItem in wrappedItemsQty))       {          var line = wrapLines[nxtItem];          debug('Orphan giftwrap found for item '+nxtItem+' on line '+line);          nlapiSelectLineItem('item', line);          nlapiRemoveLineItem('item', line);       }    } } // END GIFT WRAP` 
        

          `// BEGIN UTILITY FUNCTIONS  function isEmpty(val) { return (val == null || val == ''); } function isNotEmpty(val) { return !isEmpty(val); } function getVal(colName, linenum) { return nlapiGetLineItemValue('item',colName,linenum); }` 
        

          `// This function updates the rate and also recalculates the correct value for amount.  function setCurrentLineRate(rate) {    nlapiSetCurrentLineItemValue('item', 'rate', rate, true, true);    var qty = parseInt(nlapiGetCurrentLineItemValue('item', 'quantity'));    var amount = qty * rate;    nlapiSetCurrentLineItemValue('item', 'amount', amount, true, true); }` 
        

          `// This function returns a map with the internal ID for the item as the key and the total // quantity for that item in the value. It sums items when the same item appears on different // lines on the sales order. If passed a non-null filter value, item types that match the filter are // excluded.  function getItemMap(excludeFilter) {    if (isNotEmpty(excludeFilter))    {       debug('getItemMap called with filter '+excludeFilter);    }    var itemMap = new Array();    var numLines = nlapiGetLineItemCount('item');    for (var i=1; i<= numLines; i++)    {` 
        

          `// Include only items that match the filter.        var itemType = nlapiGetLineItemValue('item','itemtype',i);           if (isNotEmpty(excludeFilter) && itemType == excludeFilter)       {          debug('Ignoring line '+i+', itemType '+itemType+' excluded');          continue;       }              var itemId = nlapiGetLineItemValue('item','item',i);       var nextQty = parseInt(nlapiGetLineItemValue('item','quantity',i));       debug('Item '+itemId+' of type '+itemType+' added to item map');              if (itemId in itemMap)       {` 
        

          `// Add the quantities if other lines in the list machine include the same item.           nextQty = nextQty + parseInt(itemMap[itemId]);       }              debug('Item Id '+itemId+' has updated quantity to '+nextQty+' because of line #'+i);       itemMap[itemId] = nextQty;    }    return itemMap; }` 
        

          `// This function rounds the input to two decimal places.  function roundOff(amount) {    return Math.round(amount*100000)/100000; } function debug(msg) { alert(msg); } // END UTITLITY FUNCTIONS` 
        

## Deploy Your Script to the Shopping Cart {#bridgehead_N2558661}

Test your script thoroughly before running it in the shopping cart. You must follow a series of steps to load the script into your NetSuite account, and then run the script for testing purposes.

For details, see [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html).

### Related Topics

-   [Using a Third-Party Tax Calculator](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554144.html)
-   [Creating Buy-One-Get-One-Free Coupons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554377.html)
-   [Dynamic Discounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557130.html)
-   [Setting Quantity Limits for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2558716.html)
-   [Creating Time-Based Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2560375.html)
-   [Setting Default Location for Web Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561074.html)
-   [Accepting Charitable Donations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561322.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
