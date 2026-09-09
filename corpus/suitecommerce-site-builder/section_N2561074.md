---
id: "section_N2561074"
type: "section"
title: "Setting Default Location for Web Orders"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Sample Scripts for Scriptable Cart > Setting Default Location for Web Orders"
parent: "section_N2553996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561074.html"
anchors: ["bridgehead_N2561113", "bridgehead_N2561125", "bridgehead_N2561298"]
sha256: "7f35eebbd7af7dd22a2401737daae6873c61002ef914ad7da72c542bdb5eb40f"
---

You can set a default location on web store orders to offer accurate shipping estimates online. The sample script assigns a location to each order based on the items available in stock.

The sample script uses a function that implements a basic algorithm to determine which location should appear on the sales order. The quantities available in each location are compared to the quantities requested for the items on the sales order. If there are no locations with enough quantity available, then the location you specify in the script is selected for the order.

Note:

You must create a User Event script deployment record for the customBeforeSubmit() function. All other custom functions can exist on a Client Event script record if you are working with record-level scripts. If you are working with form-level scripts enter the custom functions on the Custom Code subtab on the custom transaction record, and create a User Event script for the BeforeSubmit function. For more information, see [Using Record-Level Scripts in the Shopping Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553295.html#bridgehead_N2553473).

## Setup {#bridgehead_N2561113}

The sample script does not require any custom fields or records. This script requires that you create a record-level script of type User Event to define the BeforeSubmit function.

## Create the Code {#bridgehead_N2561125}

          `// BEGIN CUSTOM FUNCTIONS FOR SETTING LOCATIONS FOR WEB ORDERS // This custom function is run immediately before a sales order is saved.  function customBeforeSubmit() {    debug('Before Submit is called');    return chooseLocation(); } //END CUSTOM FUNCTIONS FOR SETTING LOCATION` 
        

          `//BEGIN LOCATION  function chooseLocation() {` 
        

          `// Get entire quantities of all inventoried items in the sales order. Note that optional filtering // criteria is used when calling the getItemMap() function to exclude noninventory items.   var itemMap = getItemMap('NonInvtPart'); var numLines = nlapiGetLineItemCount('item'); var goodLocations = new Array(); var badLocations = new Array();` 
        

          `// Get available quantities for each location of each item on the order.     for (itemId in itemMap)    {       debug('Loading record for item id '+itemId);       var rec = nlapiLoadRecord('inventoryitem', itemId);       debug('Item record '+itemId+' loaded - getting location count');       var locCount = rec.getLineItemCount('locations');       debug('Starting loop for '+locCount+' locations');       for (var i=1; i <= locCount; i++)       {          var locId = rec.getLineItemValue('locations', 'location', i);          var onhand = rec.getLineItemValue('locations', 'quantityavailable', i);` 
        

          `// Current quantity of item is stored under itemMap[itemId] if there is enough quantity // available for this order at this location, add it to the good location list.            if (itemMap[itemId] <= onhand)          {             debug('Location '+locId+' has '+onhand+' available - added to good list');             goodLocations[locId] = true;          }` 
        

          `// If there is not enough quantity for the item, then add this location to the bad location list.           if (itemMap[itemId] > onhand)          {             debug('Location '+locId+' has '+onhand+' available - added to bad list');             badLocations[locId] = true;          }       }    }` 
        

          `// Take any bad locations out of the good list.     for (locId in badLocations)    {       delete goodLocations[locId];    }      var finalLocation = 1;   // default in the case of no good locations found      for (goodLoc in goodLocations)    {       debug('Location '+goodLoc+' can provide for all items in the sales order - setting location to this');       finalLocation = goodLoc;       break;    }      nlapiSetFieldValue('location', finalLocation, true, true);    return true;   } // END LOCATION` 
        

          `// BEGIN UTILITY FUNCTIONS  function isEmpty(val) {    return (val == null || val == ''); }   function isNotEmpty(val) {    return !isEmpty(val); }` 
        

          `// This function will return a map with the internal IDs for the item as the key and the total // quantities for that item in the value. It will sum up any items in the items sublist on the sales // order. If passed a non-null filter value, will exclude item types that match the filter.   function getItemMap(excludeFilter) {    if (isNotEmpty(excludeFilter))    {       debug('getItemMap called with filter '+excludeFilter);    }      var itemMap = new Array();    var numLines = nlapiGetLineItemCount('item');      for (var i=1; i<= numLines; i++)    {` 
        

          `// Include only items that match the filter.        var itemType = nlapiGetLineItemValue('item','itemtype',i);       if (isNotEmpty(excludeFilter) && itemType == excludeFilter)       {          debug('Ignoring line '+i+', itemType '+itemType+' excluded');          continue;       }         var itemId = nlapiGetLineItemValue('item','item',i);       var nextQty = parseInt(nlapiGetLineItemValue('item','quantity',i));         debug('Item '+itemId+' of type '+itemType+' added to item map');         if (itemId in itemMap)       {` 
        

          `// Add the quantities together if other line items in the items sublist on the sales order exist // with the same item.            nextQty = nextQty + parseInt(itemMap[itemId]);       }         debug('Item Id '+itemId+' has updated quantity to '+nextQty+' because of line #'+i);       itemMap[itemId] = nextQty;    }      return itemMap; }   function debug(val) {    nlapiLogExecution('AUDIT', val); } // END UTILITY FUNCTIONS` 
        

## Deploy Your Script to the Shopping Cart {#bridgehead_N2561298}

Test your script thoroughly before running it in the shopping cart. You must follow a series of steps to load the script into your NetSuite account, and then run the script for testing purposes.

For details, see [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html).

### Related Topics

-   [Using a Third-Party Tax Calculator](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554144.html)
-   [Creating Buy-One-Get-One-Free Coupons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554377.html)
-   [Dynamic Discounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557130.html)
-   [Offering Gift Wrap on the Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557809.html)
-   [Setting Quantity Limits for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2558716.html)
-   [Creating Time-Based Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2560375.html)
-   [Accepting Charitable Donations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561322.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
