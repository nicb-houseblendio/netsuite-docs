---
id: "section_N423495"
type: "section"
title: "Purchase Order Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Purchase Order Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N423495.html"
anchors: ["bridgehead_N423766", "bridgehead_N423795", "bridgehead_N424018", "bridgehead_4314739910", "bridgehead_N424056", "bridgehead_3705049304", "bridgehead_N424100", "bridgehead_N424176", "bridgehead_N424203", "bridgehead_N424485", "bridgehead_N425645"]
sha256: "92618f480afefa73b3b4e81fbe382a9604c19c29f405eee3360b1e6a6ab79a14"
---

NetSuite Purchase Order transactions authorize vendors to provide goods or services to your company, and express a commitment to receive and pay for them. These transactions have no accounting impact until orders are received.

For more details about Purchase Orders in NetSuite, see [Purchase Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2399585.html).

Note:

Purchase Order imports aren't available unless the Purchase Orders feature is enabled in your account. To enable this feature, go to _Setup > Company > Enable Features_ and on the Transactions subtab, check the Purchase Orders box.

-   Purchase order imports can include line-level items and expenses data. For imports with items data, but no expenses data, you can choose either the one file to upload or the multiple files to upload option. For imports with expenses data, you **must** choose the multiple files to upload option. For more information, see [Using Multiple Files for Purchase Order Sublist Data](#bridgehead_N424018).
    
-   By default, the NetSuite fields available for purchase order import mapping are those available on your preferred purchase order form. Fields can be mapped for the import job if they're displayed (not hidden) and not disabled on your preferred form. To make different fields available, you can specify the standard drop ship or another purchase order form on the Import Options page. For information, see [Custom Form Specification for Purchase Order Imports](#bridgehead_N423766).
    
-   You can't import drop ship purchase orders and other purchase orders at the same time; you must use separate import jobs. To import drop ship purchase orders, you must specify the standard drop ship purchase order form, or a custom drop ship form, as the Custom Form advanced option on the Import Options page, so that the Ship To field is available for mapping.
    
-   You must map either external ID or internal ID to serve as a unique ID per record. The unique ID should be included in every line of the CSV files. For imports of new data, use external ID.
    
-   On the Import Assistant's Field Mapping page, map the external ID field from your CSV files to the NetSuite Order # field, which serves as a transaction ID for Purchase Order records. This mapping allows external IDs to be displayed on Purchase Order forms in the NetSuite user interface.
    
-   Each imported Purchase Order record should include a reference to a NetSuite Vendor record, mapped to the Purchase Order's Vendor field. This reference must be a unique identifier; you should use the vendor record's internal ID or external ID, rather than a name reference.
    
-   By default, Billing Address and Shipping Address fields for Purchase Order records are copied from linked Vendor records, but these fields are available for mapping in the Import Assistant so that their values can be set by CSV files' field values instead.
    
-   If the Multiple Currencies feature is enabled, you must map the Exchange Rate field. If your CSV file doesn't include values for this field, you can set it to a default value. Currency values are taken from referenced vendors. See [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html).
    
-   The creation of multiple Purchase Orders, required by a Sales Order containing drop ship or special order items, will fail if the Sales Order is set to Closed prior to their creation.
    

For details about fields that can be mapped in the purchase order record, see the SOAP Schema Browser's [purchase order](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/purchaseorder.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for Purchase Orders imports:

-   [Custom Form Specification for Purchase Order Imports](#bridgehead_N423766)
    
-   [Supported Purchase Order Sublist Data Imports](#bridgehead_N423795)
    
-   [Using Multiple Files for Purchase Order Sublist Data](#bridgehead_N424018)
    
-   [Supported Purchase Order Subrecord Data Imports](#bridgehead_4314739910)
    
-   [Importing Purchase Orders with Billed-Back Items and Expenses](#bridgehead_N424056)
    
-   [Importing Purchase Orders with Serial or Lot-Numbered items](#bridgehead_3705049304)
    
-   [Importing Purchase Orders when Advanced Taxes is Enabled](#bridgehead_N424100)
    
-   [Working with Closed Purchase Orders](#bridgehead_N424176)
    
-   [Sample Purchase Order Single CSV File Format](#bridgehead_N424203)
    
-   [Sample Purchase Order Multiple CSV File Format](#bridgehead_N424485)
    
-   [Using Import Assistant for Purchase Orders Mass Update](#bridgehead_N425645)
    

## Custom Form Specification for Purchase Order Imports {#bridgehead_N423766}

By default the Field Mapping page for a purchase order import displays the NetSuite fields from your preferred purchase order form as available for mapping. The default form for your role may not include all the fields you need to import. To ensure that the appropriate fields are available for mapping, you can select any purchase order form that's available to your role, in the Advanced Options area of the Import Assistant's Import Options page. For more information, see [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html).

Warning:

If you specify a drop ship purchase order form, all records in the imported file should be drop ship purchase orders. You can't import both drop ship purchase orders and other purchase orders at the same time.

## Supported Purchase Order Sublist Data Imports {#bridgehead_N423795}

The Purchase Order import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Items | You must import at least one line item for all new records, and you must map required fields for this sublist on the Field Mapping page. See [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690). Selectively updatable based on Line/Order Line or Item key field. See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html). |
| Expenses | When the Allow Expenses on Purchase Orders preference is enabled. Expenses data must be in a separate CSV file. |

If you use classes, departments, or locations, you can set these values either for an entire purchase order, or per individual item/expense lines.

If the Item Options feature is enabled in your account, you can import values for custom transaction item options along with Items sublist data. Transaction item options must first be set up at _Customization > Lists, Records, & Fields > Transaction Item Options > New_, with one of the following Applies To settings: Purchase, All Items. For details, see [Importing Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N430392.html).

If the Item Options feature is enabled in your account, you can import values for custom transaction item options along with Items sublist data. Transaction item options must first be set up at Customization > Lists, records, & fields, > Transaction item options. Click New. Include one of the following Applies To settings: Purchase, All Items. For details, see [Importing Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N430392.html).

For imports that update existing Purchase Order records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

Important:

For non-keyed sublists, you shouldn't update main transaction fields and sublist fields during the same import job.

## Using Multiple Files for Purchase Order Sublist Data {#bridgehead_N424018}

For purchase order imports that include items data but no expenses data, you can choose the one file to upload option, and include all data in a single CSV file, or you can choose the multiple files to upload option, and include mainline data in one file and items data in another file.

For imports that include expenses data, you **must** use the multiple files to upload option, with one file for mainline data, and one for expenses data. If you're also importing items data, it should be in a third file.

If you choose the multiple files option, be sure to include the external ID or key field values in the sublist files as well as in the main file.

For a multiple files upload example, see [Sample Purchase Order Multiple CSV File Format](#bridgehead_N424485).

## Supported Purchase Order Subrecord Data Imports {#bridgehead_4314739910}

The Purchase Order import supports the import of the following subrecord data:

| Subrecord | Notes |
| --- | --- |
| Billing Address | By default, the subrecord Address field is read-only, and data from other subrecord fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |
| Items - Inventory Detail | When Advanced Bin/Numbered Inventory Management feature enabled. |
| Shipping Address | By default, the subrecord Address field is read-only, and data from other subrecord fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |

## Importing Purchase Orders with Billed-Back Items and Expenses {#bridgehead_N424056}

If you're importing purchase orders with items or expenses that need to be billed back to customers, you can set the value of the Billable field to 'TRUE' and include a value for the Customer field, for each of these item or expense lines.

## Importing Purchase Orders with Serial or Lot-Numbered items {#bridgehead_3705049304}

If you're importing purchase orders with serial or lot-numbered items, you need to define serial or lot numbers in the Serial/Lot Numbers field for each item.

-   You must enter a number for each serialized item; for example, if the Quantity field has a value of 2, you must enter two numbers.
    
-   You can separate multiple numbers with spaces, commas, or Returns.
    

## Importing Purchase Orders when Advanced Taxes is Enabled {#bridgehead_N424100}

If the Advanced Taxes feature is enabled, you can include values for the Tax Code and Tax Amount fields for purchase order item and expense lines as needed in CSV files. Tax codes should be set up in NetSuite before the import. Note that other tax-related values for line items and expenses are calculated by the system.

The Advanced Taxes feature is required for NetSuite OneWorld accounts. For information about working with taxes in OneWorld, see [Nexuses and Taxes in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269581.html). For general information about setting up tax codes, see [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html).

## Working with Closed Purchase Orders {#bridgehead_N424176}

You can import a purchase order as closed by setting its Items sublist records' Closed field values to 'TRUE'.

If these values aren't set in the CSV file itself, you can set a default value by adding the Items sublist's Closed field to the field mapping, clicking the edit icon, and selecting the Yes option button. For more information, see [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html).

You can use an import to update closed purchase orders by setting the Closed field value for one or more items in an order to 'FALSE'.

## Sample Purchase Order Single CSV File Format {#bridgehead_N424203}

The following table illustrates example column headers and data snippets in a single file upload of purchase orders. This file includes data for purchase order header fields and item lines. Note that in this case, the same purchase order number can be repeated in multiple rows.

| External ID | Vendor | PO Number | Date | Item |
| --- | --- | --- | --- | --- |
| EXT2003 | American Computers | 2003 | 7/28/2009 | Computer Systems : Desktop : HP Compaq d230 |
| EXT2003 | American Computers | 2003 | 7/28/2009 | Computer Systems : Laptop : Compaq Evo n800c |
| EXT2004 | American Computers | 2004 | 7/28/2009 | Accessories : Standard Keyboard |

## Sample Purchase Order Multiple CSV File Format {#bridgehead_N424485}

The following tables illustrate example column headers and data snippets in a multiple file upload of purchase orders, including items and expenses data. Note that External ID is the key column that would be specified on the Import Assistant File Mapping page.

**Primary File:**

Each row of the primary file must include a unique identifier, which in this case the external ID.

| External ID | Vendor | PO # | Date |
| --- | --- | --- | --- |
| EXT2003 | American Computers | 2003 | 7/28/09 |
| EXT2004 | American Computers | 2004 | 8/3/09 |

**Linked File - Items:**

The items file can include multiple rows with the same purchase order external ID.

| External ID | Item | Quantity | Amount |
| --- | --- | --- | --- |
| EXT2003 | Computer Systems : Desktop : HP Compaq d230 | 1 | 800 |
| EXT2003 | Computer Systems : Laptop : Compaq Evo n800c | 1 | 1200 |

**Linked File - Expenses:**

The expenses file can include multiple rows with the same purchase order external ID.

| External ID | Account | Amount | Memo | Customer | Billable |
| --- | --- | --- | --- | --- | --- |
| EXT2003 | 6150 Office Expense | 350 | laptop repair | 107 Fabre Art Gallery | Yes |
| EXT2003 | 6150 Office Expense | 20 | laptop part | 107 Fabre Art Gallery | Yes |
| EXT2004 | 6150 Office Expense | 60 | misc. | \- | No |

## Using Import Assistant for Purchase Orders Mass Update {#bridgehead_N425645}

You can do a mass update of existing Purchase Order data by creating a Transaction saved search with a filter of Type is Purchase Order, changing the data externally, then using the Import Assistant to import modified data, using the Update data handling option. For more information, see [Creating Transaction Saved Searches for Reimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N432599.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
