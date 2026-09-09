---
id: "section_N2558716"
type: "section"
title: "Setting Quantity Limits for Customers"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Sample Scripts for Scriptable Cart > Setting Quantity Limits for Customers"
parent: "section_N2553996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2558716.html"
anchors: ["bridgehead_N2558759", "bridgehead_N2559892", "bridgehead_N2560351"]
sha256: "1d3b035a4a13e1f2910b6eca60c94884f23004626dc502d7f72e3c0448646bfc"
---

Use SuiteScript to restrict the quantity of an item that can be purchased over the lifetime of the customer.

The sample script provided here restricts the quantity of items based on the value in a custom field that you add to the item record. When a shopper adds an item that has an allotment amount to the cart, a custom record is created to track the quantity sold .

Note:

You must create a User Event script deployment record for the customAfterSubmit() function. All other custom functions can exist on a Client Event script record if you are working with record-level scripts. If you are working with form-level scripts enter the custom functions on the Custom Code subtab on the custom transaction record, and create a User Event script for the AfterSubmit function. For more information, see [Using Record-Level Scripts in the Shopping Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553295.html#bridgehead_N2553473).

## Setup {#bridgehead_N2558759}

Use the steps below to create custom fields and custom records required to run the sample script.

1.  Create a custom field to hold the allotment value on item records.
    
    1.  Go to Customization > Lists, Records, & Fields > Item Fields > New.
        
    2.  In the **Label** field, enter a name for the custom field. For example, **Item Allotment**.
        
    3.  In the **Type** field, select **Integer Number**.
        
    4.  Check the **Store Value** box.
        
    5.  On the **Applies To** subtab, select **Inventory Item**.
        
    6.  Click **Save**.
        
2.  Create custom transaction column field for displaying the Allotment value for each item on the transaction record.
    
    1.  Go to Customization > Lists, Records, & Fields > Transaction Column Fields > New.
        
    2.  In the **Label** field, enter a column name. For example, **Default Allotment**.
        
    3.  In the **Type** field, select **Integer Number**.
        
    4.  Check the **Store Value** box.
        
    5.  On the **Applies To** subtab, check the following boxes: **Sale Item**, **Store Item**, and **Hidden**.
        
    6.  On the **Sourcing & Filtering** subtab,
        
        -   Set the **Source List** to **Item**
            
        -   In the **Source From** field, select the custom field you created in Step 1.
            
    7.  On the Access subtab:
        
        -   Set **Default Access Level** to **Edit**.
            
        -   Set **Default Level for Search/Reporting** to **Edit**.
            
    8.  Click **Save**
        
3.  Create a custom record for tracking customer allotments.
    
    1.  Go to Customization > Lists, Records, & Fields > Record Types > New.
        
    2.  In the **Name** field, enter a name for this record. For example, **Allotments**.
        
    3.  In the **ID** field, enter **\_allotments.**
        
        Note:
        
        After you click save, the value for **ID** automatically changes to **custcol\_allotments**. The sample script depends on this value for ID.
        
    4.  Clear the **Include Name Field** box.
        
    5.  On the **Permissions** subtab, set the following values:
        
        -   In the **Role** column, select **Customer Center**, and then set **Level** to **Full**. Click **Add**.
            
        -   In the **Role** column, select **Shopper**, and then set **Level** to **Full**. Click **Add**.
            
        -   In the **Role** column, select **Administrator**, and then set **Level** to **Full** (for testing in the application). Click **Add**.
            
        -   Click **Save**.
            
4.  Create three new fields on the custom record.
    
    Go to Customization > Lists, Records, & Fields > Record Types. Click the **Custom Record** you created in Step 3.
    
    1.  On the **Fields** Subtab, click **New Field** to create a field for capturing the customer record internal ID.
        
        -   In the **Label** field, enter **Customer ID**.
            
        -   In the **ID** field, enter \_ **customer**.
            
            Note:
            
            After you click **Save**, the value for **ID** automatically changes to **custrecord\_customer**. The sample script depends on this value for ID.
            
        -   In the **Type** field, select **List/Record**.
            
        -   Check the **Store Value** box.
            
        -   Check the **Show in List** box.
            
        -   Click Save.
            
    2.  Click New Fields again to create a field for the item record internal ID.
        
        -   In the **Label** field, enter **Item ID**.
            
        -   In the **ID** field, enter \_ **item**.
            
            Note:
            
            After you click save, the value for ID automatically changes to **custrecord\_item**. The sample script depends on this value for ID.
            
        -   In the **Type** field, select **List/Record**.
            
        -   In the **List/Record** field, select **Item**.
            
        -   Check the **Store Value** box and the **Show in List** box.
            
        -   On the **Validation & Defaulting** subtab, check the **Mandatory** box.
            
        -   Click **Save**.
            
    3.  On the **Fields** Subtab, click **New Field** to create a field for keeping track of the number remaining in each customer's allotment.
        
        -   In the **Label** field, enter **Number Remaining**.
            
        -   In the **ID** field, enter **\_remaining**.
            
            Note:
            
            After you click save, the value for ID automatically changes to **custrecord\_remaining**. The sample script depends on this value for ID.
            
        -   In the **Type** field, select **Integer Number**.
            
        -   Check the **Store Value** box.
            
        -   Check the **Show in List** box.
            
        -   Click **Save**.
            

## Create the Code {#bridgehead_N2559892}

          `// BEGIN CUSTOM FUNCTIONS FOR ALLOTMENTS  function customValidateLine(type) {` 
        

          `// In web store scripts line inputs only needed to be validated on the item sublist.     if (type != 'item')    {       return true;    }` 
        

          `// Note that validation routines are called in a different way than other events because the // return value of each function must be tested before going on to the next function. If any // function returns false, then stop processing and return false.      if (!verifyAllotments())    {       return false;    }` 
        

          `// All validations passed. Return true.     return true; }` 
        

          `// This custom function will be run after a sales order is saved. Because only User Event scripts // have an afterSubmit event, you must create a separate User Event script record.   function customAfterSubmit() {    return updateAllotmentsOnSave(); } //END CUSTOM FUNCTIONS FOR ALLOTMENTS` 
        

          `//BEGIN ALLOTMENTS  function verifyAllotments() {` 
        

          `// Get current item and customer.     var custId = nlapiGetFieldValue('entity');    var itemId = nlapiGetCurrentLineItemValue('item', 'item');    debug('Customer ID: '+custId+', Item Id: '+itemId);` 
        

          `// First, check to see if this item has a value for the allotment custom field. If not, ignore the // validation and allow the line item to be entered. Not all items will have a value for allotment.     var allotmentDefault = nlapiGetCurrentLineItemValue('item','custcol_allotmentdefault');    debug('Allotment default for item '+itemId+' is '+allotmentDefault);    if (isEmpty(allotmentDefault))    {       debug('Empty allotment default - ignore validation');       return true;    }` 
        

          `// If the shopper has not logged in, the allotment record cannot be found. Set the value for the // number remaining in the allotment to the value in the Allotment custom field on the item. // Note that this sample script does not include an alert for shoppers about the allotment // quantity.     var remaining = allotmentDefault;        var allotmentRec = getAllotmentRecord(custId, itemId, allotmentDefault);    if (allotmentRec != null)    {` 
        

          `// When the shopper logs in, find the allotment record. Get the number remaining in the // allotment for this customer.        remaining = allotmentRec.getFieldValue('custrecord_remaining');    }` 
        

          `// Calculate the current total quantity for this item to check if it exceeds the customer's // allotted quantity.     var qty = parseInt(nlapiGetCurrentLineItemValue('item','quantity'));    var currentIndex = nlapiGetCurrentLineItemIndex('item');` 
        

          `// Because the order can contain multiple line items for the same line, look for the items in // other lines and add the quantities together to get an accurate count.     var numLines = nlapiGetLineItemCount('item');    for (var i=1; i<= numLines; i++)    {` 
        

          `// Skip the line currently selected because it was already counted.        if (i == currentIndex) { continue; }       var nxtItemId = nlapiGetLineItemValue('item','item',i);       if (nxtItemId == itemId)       {          qty = qty + parseInt(nlapiGetLineItemValue('item','quantity',i));       }    }      debug('Current quantity for item '+itemId+' is '+qty);      if (qty > remaining)    {` 
        

          `// If quantities are added that exceed the current allotments, refuse the entry.        alert('You are only allotted '+remaining+' of this item - please reduce your order');       return false;    }      return true; }` 
        

          `// This function is called when the sales order is saved.  function updateAllotmentsOnSave() {    var custId = nlapiGetFieldValue('entity');    var numLines = nlapiGetLineItemCount('item');    var allottedItemQty = new Array();    debug('Allotment update called for customer '+custId);` 
        

          `// First, get the total item count for each item.     var itemMap = getItemMap();` 
        

          `// Then construct a map of the current allotments for each item.     var allottedMap = new Array();      for (var i=1; i<= numLines; i++)    {       var defaultAllotment = nlapiGetLineItemValue('item', 'custcol_allotmentdefault', i);` 
        

          `// If this item doesn't have allotments, then skip it.        if (isEmpty(defaultAllotment))       {          debug('Line '+i+' has no default allotments. Skipping.');                   continue;       }         var itemId = nlapiGetLineItemValue('item','item',i);       if (!(itemId in allottedMap))       {` 
        

          `// If this item ID does not exist in the map, then load the allotment record.           debug('Getting allotment rec for item ID '+itemId);          var rec = getAllotmentRecord(custId, itemId, nlapiGetLineItemValue('item','custcol_allotmentdefault', i));          allottedMap[itemId] = rec;       }    }` 
        

// Now, update each custom record with the new value for the allotted number remaining.

          `// Now, update each custom record with the new value for the allotted number remaining.     for (itemId in allottedMap)    {       rec = allottedMap[itemId];       var remaining = rec.getFieldValue('custrecord_remaining');       var qty = itemMap[itemId];         if (qty > remaining)       {          alert('You are only allotted '+remaining+' of this item - please reduce your order');          return false;       }` 
        

          `// Set the record with the new quantity, and then save it.        var newQty = remaining - qty;       rec.setFieldValue('custrecord_remaining', newQty);       debug('Updating custom record to new qty = '+newQty+' for item ID '+itemId);       nlapiSubmitRecord(rec, true);    }      return true; }` 
        

          `// This function returns a custom record for allotments for this customer-item // combination. If an allotment record does not exist for this customer and item combination, it // will create one with the original allotment specified on the item record. If the  // customer ID is null or zero (0), the shopper has not logged in,and should not be given a // record. Instead, restrict the shopper to the default value until they log in.  function getAllotmentRecord(custId, itemId, allotmentDefault) {` 
        

          `// Before doing anything else, check for anonymous shoppers. If an anonymous shopper is // detected, return null for an allotment record. Any script that calls this function should check // for null values before proceeding to read the outgoing record.     if (isEmpty(custId) || custId == '0')    {       return null;    }` 
        

          `// Define two filters, one for item and one for the customer.     var filters = new Array();    filters[0] = new nlobjSearchFilter('custrecord_customer', null, 'anyOf', custId);    filters[1] = new nlobjSearchFilter('custrecord_item', null, 'anyOf', itemId);        try    {       var searchresults = nlapiSearchRecord('customrecord_allotments', null, filters, null);    }    catch (err)    {       debug('Error during allotment record retrieval: '+err.description);    }        var rec;      if (isEmpty(searchresults))    {       debug('No record found for item '+itemId+' and customer ID '+custId+' - creating a new one');` 
        

          `// If no records are found, then create a new record to track this customer-item combination.        rec = nlapiCreateRecord('customrecord_allotments');       rec.setFieldValue('custrecord_customer', custId);       rec.setFieldValue('custrecord_item', itemId);       rec.setFieldValue('custrecord_remaining', allotmentDefault);       nlapiSubmitRecord(rec);    }    else    {` 
        

          `// The record was found. Get the remaining quantity.        rec = nlapiLoadRecord(searchresults[0].getRecordType(), searchresults[0].getId());       debug('Custom record found; remaining '+rec.getFieldValue('custrecord_remaining')+' found for item '+itemId+' and customer ID '+custId);    }      return rec; }` 
        

          `// UTILITY FUNCTIONS  function isEmpty(val) {    return (val == null || val == ''); }   function isNotEmpty(val) {    return !isEmpty(val); }   function getVal(colName, linenum) {    return nlapiGetLineItemValue('item',colName,linenum); }` 
        

          `// This function returns a map with the internal ID for the item as the key and the total // quantity for that item in the value. It sums items when the same item appears on different // lines on the sales order. If passed a non-null filter value, item types that match the filter are // excluded.   function getItemMap(excludeFilter) {    if (isNotEmpty(excludeFilter))    {       debug('getItemMap called with filter '+excludeFilter);    }      var itemMap = new Array();    var numLines = nlapiGetLineItemCount('item');      for (var i=1; i<= numLines; i++)    {` 
        

          `// Include only items that match the filter.        var itemType = nlapiGetLineItemValue('item','itemtype',i);       if (isNotEmpty(excludeFilter) && itemType == excludeFilter)       {          debug('Ignoring line '+i+', itemType '+itemType+' excluded');          continue;       }         var itemId = nlapiGetLineItemValue('item','item',i);       var nextQty = parseInt(nlapiGetLineItemValue('item','quantity',i));         debug('Item '+itemId+' of type '+itemType+' added to item map');         if (itemId in itemMap)       {` 
        

          `// If other line items exist with the same item, then add the quantities together.           nextQty = nextQty + parseInt(itemMap[itemId]);       }         debug('Item Id '+itemId+' has updated quantity to '+nextQty+' because of line #'+i);       itemMap[itemId] = nextQty;    }      return itemMap; }   function debug(val) {    nlapiLogExecution('DEBUG', val); } //END UTILITY FUNCTIONS` 
        

## Deploy Your Script to the Shopping Cart {#bridgehead_N2560351}

Test your script thoroughly before running it in the shopping cart. You must follow a series of steps to load the script into your NetSuite account, and then run the script for testing purposes.

For details, see [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html).

### Related Topics

-   [Using a Third-Party Tax Calculator](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554144.html)
-   [Creating Buy-One-Get-One-Free Coupons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2554377.html)
-   [Dynamic Discounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557130.html)
-   [Offering Gift Wrap on the Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2557809.html)
-   [Creating Time-Based Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2560375.html)
-   [Setting Default Location for Web Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561074.html)
-   [Accepting Charitable Donations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2561322.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
