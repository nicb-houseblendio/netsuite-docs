---
id: "section_N451889"
type: "section"
title: "Line Item Updates on Transactions Imports"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Tips for Successful CSV Imports > Sublist Data Import > Line Item Updates on Transactions Imports"
parent: "section_N439392"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html"
anchors: ["bridgehead_N451970", "bridgehead_N452045", "bridgehead_N452166"]
sha256: "c936a320925210d22eaf70be459b9abca467383169f37778f406ca6194743b2d"
---

The Import Assistant lets you update items data for the following types of transactions: Cash Sale, Estimate, Invoice, Opportunity, Purchase Order, Sales Order, Vendor Bill, Vendor Credit, and Vendor Return Authorization. You can modify data for existing line items and add line items to existing transactions.

The Items sublist for transactions uses either Line/Order Line or Item as a key field to determine how to update or add line items.

-   If a CSV file row includes values for both Line/Order Line and Item fields, Line/Order Line takes precedence over Item.
    
-   CSV file rows with key field values that match existing line item key field values are used to update existing line items. CSV file rows with non-matching key field values are added as new line items.
    
-   An error is returned if the import can't determine which lines to update. This error occurs if there are two existing lines with duplicate Item values and if there are two lines in the CSV file that match a single existing line.
    
-   You should use Line/Order Line as a key field. Because transactions may include multiple lines with the same Item value, using Item as the key may cause errors resulting from duplicate Item values.
    
-   If you import line items to update a transaction and these new line items have the same Line/Order Line values as existing transaction line items, the import results in the new line items overwriting the existing line items. To instead add the line items, map a column with null values to the Line/Order Line field for the import.
    
-   You can remove a line item from an existing transaction by exporting your data, removing the unnecessary line in your CSV file, then importing the file again. In this case, set the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) option to True.
    
-   For updates of existing transaction line items (based on matching key field values), by default only mapped field values overwrite existing line item field values; fields that are not mapped for import don't change. If you want all CSV file values to overwrite existing values, set the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) option to True. Generally, you don't want to overwrite sublists, as there are many values set at the time of transactions that you wouldn't want changed after the fact, such as Rate.
    

Important:

Even if you don't have values for Line/Order Line, you should include it as a column in your CSV file and map it on the Field Mapping page. If Line/Order Line is mapped, even if its values are blank in the CSV file, errors don't result from duplicate Item values.

Review the following examples to get an understanding of how to format a CSV file to update transaction item lines.

## CSV Data Example of Unsuccessful Transaction Line Item Update {#bridgehead_N451970}

-   Existing Sales Order Transaction Lines
    
    -   Item Y, Quantity 1
        
    -   Item Y, Quantity 2
        
-   CSV File for Import
    
    -   Item Y, Quantity 5
        
    -   Item Y, Quantity 5
        
    -   Item Y, Quantity 15
        

This data results in an error because the import is trying to use the Item value as the key, and it's not clear which transaction lines should be updated.

## CSV Data Example of Successful Transaction Line Item Addition {#bridgehead_N452045}

-   Existing Sales Order Transaction Lines
    
    -   Item Y, Quantity 1
        
    -   Item Y, Quantity 2
        
-   CSV File for Import
    
    -   Item Y, Quantity 5, Order Line (no value)
        
    -   Item Y, Quantity 5, Order Line (no value)
        
    -   Item Y, Quantity 15, Order Line (no value)
        
-   Updated Sales Order Transaction Lines
    
    -   Item Y, Quantity 1
        
    -   Item Y, Quantity 2
        
    -   Item Y, Quantity 5
        
    -   Item Y, Quantity 5
        
    -   Item Y, Quantity 15
        

The inclusion of the Order Line column in the CSV file prevents the error. Because the Order Line column doesn't have any values, CSV file lines are not matched with any existing line items, and are simply added.

The following example illustrates how you might structure your CSV import file. Because the order line ID isn't specified, this example adds another line item to the specified sales order.

| Customer | Date | Order Number | Item | Quantity | Order Line ID |
| --- | --- | --- | --- | --- | --- |
| Julie Homer | 13/7/2017 | 7 | Service Kit - Medium | 6 | \- |

## CSV Data Example of Successful Transaction Line Item Update {#bridgehead_N452166}

-   Existing Sales Order Transaction Lines
    
    -   Item Y, Quantity 1, Order Line 22
        
    -   Item Y, Quantity 2, Order Line 25
        
-   CSV File for Import
    
    -   Item Y, Quantity 5, Order Line 22
        
    -   Item Y, Quantity 5, Order Line 25
        
    -   Item Y, Quantity 15, Order Line (no value)
        
-   Updated Sales Order Transaction Lines
    
    -   Item Y, Quantity 6, Order Line 22
        
    -   Item Y, Quantity 7, Order Line 25
        
    -   Item Y, Quantity 15
        

The first two CSV file lines are matched to existing line items so the quantity amounts are added. The third CSV file line is not matched, so it's added as a new line item.

The following example illustrates how you might structure your CSV import file. Because the order line ID is specified, this example updates the matching line item in the specified sales order.

| Customer | Date | Order Number | Item | Quantity | Order Line ID |
| --- | --- | --- | --- | --- | --- |
| Julie Homer | 13/7/2017 | 7 | Service Kit - Medium | 8 | 4 |

Note:

You can create a saved transaction search to retrieve order line values for item lines, before setting up an import to update this data.

### Related Topics

-   [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html)
-   [Supported Sublist Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439528.html)
-   [Importing Sublist Data in a Single File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1493384282.html)
-   [Multiline Sublists for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1493796058.html)
-   [Required Fields for Sublist Import Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
