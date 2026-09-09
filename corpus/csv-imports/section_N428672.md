---
id: "section_N428672"
type: "section"
title: "Vendor Credit Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Vendor Credit Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N428672.html"
anchors: ["bridgehead_N428861", "bridgehead_N429095", "bridgehead_4314750325", "bridgehead_N429122", "bridgehead_N429135", "bridgehead_N429168"]
sha256: "b9e9626360f3b5a72d4ee45611c119718dbcefd7c243493c0052e7f1943c37fb"
---

Vendor Credit transactions create credits from vendors that can be applied to payables. For example, a vendor credit transaction may occur when items are returned to a vendor or when a discount is negotiated with a vendor.

Note:

To maintain performance, don't submit transactions that contain more than 5000 lines through CSV import.

For details about vendor credits in NetSuite, see [Vendor Credits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2391960.html).

-   Vendor credit imports can include line-level items, expenses, and apply data. For imports with items data, but no expenses or apply data, you can choose either the one file to upload or the multiple files to upload option. For imports with expenses or apply data, you **must** choose the multiple files to upload option. For more information, see [Using Multiple Files for Vendor Credit Sublist Data](#bridgehead_N429095).
    
-   You must map external ID or internal ID to serve as a unique ID per record. The unique ID should be included in every line of the CSV files. For imports of new data, use external ID. On the Import Assistant's Field Mapping page, map the external ID field from your CSV files to the NetSuite Reference No. field, which serves as a transaction ID for Vendor Credit records. This mapping allows external IDs to be displayed on Vendor Credit forms in the NetSuite user interface.
    
-   Each imported Vendor Credit record should include a reference to a NetSuite Vendor record, mapped to the Vendor Credit's Vendor field. This reference must be a unique identifier; use internal ID or external ID, rather than a name reference. If you don't map a reference number field, reference number values are generated automatically.
    
-   If the Use Account Numbers preference has been enabled at _Setup > Accounting > Accounting Preferences_, imported values for the Account field should include both account number and name, for example: 11000 Accounts Payable. If this preference isn't enabled, values should be account name only, for example: Accounts Payable.
    
-   If the Multiple Currencies feature is enabled, you must map the Exchange Rate field. If your CSV file doesn't include values for this field, you can set it to a default value. Currency values are taken from referenced vendors. See [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html).
    

For details about fields that can be mapped in the vendor credit record, see the SOAP Schema Browser's [vendor credit](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/vendorcredit.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for vendor credit imports:

-   [Supported Vendor Credit Sublist Data Imports](#bridgehead_N428861)
    
-   [Using Multiple Files for Vendor Credit Sublist Data](#bridgehead_N429095)
    
-   [Supported Vendor Credit Subrecord Data Imports](#bridgehead_4314750325)
    
-   [Importing Vendor Credits with Billed-Back Items and Expenses](#bridgehead_N429122)
    
-   [Importing Vendor Credits when Amortization is Enabled](#bridgehead_N429135)
    
-   [Using Import Assistant for Vendor Credits Mass Update](#bridgehead_N429168)
    

## Supported Vendor Credit Sublist Data Imports {#bridgehead_N428861}

The Vendor Credit import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Items | You must import at least one line item for all new records, and you must map required fields for this sublist on the Field Mapping page. See [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690). Selectively updatable based on Line/Order Line or Item key field. See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html). |
| Expenses | Expenses data must be in a separate CSV file. Selectively updatable based on Line/Order Line key field. |
| Apply | Apply data must be in a separate CSV file. Selectively updatable based on Apply or Line key field. |
| Accounting Book Details | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on Accounting Book key field. |

If you use classifications, you can set class, department, and location values per individual item/expense lines.

If the Item Options feature is enabled in your account, you can import values for custom transaction item options along with Items sublist data. Transaction item options must first be set up at _Customization > Lists, Records, & Fields > Transaction Item Options > New_, with one of the following Applies To settings: Purchase, All Items. For details, see [Importing Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N430392.html).

For imports that update existing Vendor Credit records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

## Using Multiple Files for Vendor Credit Sublist Data {#bridgehead_N429095}

For vendor bill imports that include items data but no expenses or apply data, you can choose the one file to upload option, and include all data in a single CSV file, or you can choose the multiple files to upload option, and include mainline data in one file and items data in another file.

For imports that include expenses and apply data, you **must** use the multiple files to upload option, with one file for mainline data, one for expenses data, and one for apply data, as needed. If you're also importing items data, it should be in its own separate file as well.

For the multiple files option, be sure to include the external ID or key field values in the sublist files as well as in the main file.

## Supported Vendor Credit Subrecord Data Imports {#bridgehead_4314750325}

The Vendor Credit import supports the import of the following subrecord data:

| Subrecord | Notes |
| --- | --- |
| Items - Inventory Detail | when Advanced Bin/Numbered Inventory Management feature enabled |

## Importing Vendor Credits with Billed-Back Items and Expenses {#bridgehead_N429122}

If you're importing vendor credits with items or expenses that need to be billed back to customers, you can set the value of the Billable field to 'TRUE' and include a value for the Customer field, for each of these item or expense lines.

## Importing Vendor Credits when Amortization is Enabled {#bridgehead_N429135}

If the Amortization feature is enabled, you're able to include amortization schedule, amortization start date, and amortization end date values in imported vendor credit items and expenses data. These values define how costs are allocated across a range of time and recognized in increments. Amortization schedules should be set up in NetSuite before the import. For information about setting up amortization in NetSuite, see [Expense Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1765678.html).

## Using Import Assistant for Vendor Credits Mass Update {#bridgehead_N429168}

You can perform a mass update of existing Vendor Credit data by creating a Transaction saved search with a filter of Type is Vendor Credit, changing data externally, then using the Import Assistant to import modified data, using the Update data handling option. For more information, see [Creating Transaction Saved Searches for Reimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N432599.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
