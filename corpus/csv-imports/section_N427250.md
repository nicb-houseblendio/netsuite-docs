---
id: "section_N427250"
type: "section"
title: "Vendor Bill Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Vendor Bill Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N427250.html"
anchors: ["bridgehead_N427468", "bridgehead_N428372", "bridgehead_4314746116", "bridgehead_1495016439", "bridgehead_N428417", "bridgehead_N428430", "bridgehead_N428505", "bridgehead_4337775811", "bridgehead_4337777063", "bridgehead_N428538"]
sha256: "ae28329b40239574b979db17fb8a9318f26905f2d8b6700cffb5141e6c636401"
---

Vendor Bill transactions allow you to track paid and unpaid vendor bills, as well as pricing for particular products you buy. You enter bills when they arrive, and pay them when they're due. NetSuite can remind you when those bill payments are due.

Note:

To maintain performance, don't submit transactions that contain more than 5000 lines through CSV import.

For more details about vendor bills in NetSuite, see [Vendor Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2370131.html).

-   Vendor bill imports can include line-level items and expenses data. For imports with items data, but no expenses data, you can choose either the one file to upload or the multiple files to upload option. For imports with expenses data, it's best to choose the multiple files to upload option. For more information, see [Using Multiple Files for Vendor Bill Sublist Data](#bridgehead_N428372).
    
-   You must map external ID or internal ID to serve as a unique ID per record. The unique ID should be included in every line of the CSV files. For imports of new data, use external ID. On the Import Assistant's Field Mapping page, map the external ID field from your CSV files to the NetSuite Reference No. field, which serves as a transaction ID for Vendor Bill records. This mapping allows external IDs to be displayed on Vendor Bill forms in the NetSuite user interface.
    
-   Each imported Vendor Bill record should include a reference to a NetSuite Vendor record, mapped to the Vendor Bill's Vendor field. This reference must be a unique identifier; use internal ID or external ID, rather than a name reference. If you don't map a reference number field, reference number values are generated automatically.
    
-   If the Use Account Numbers preference has been enabled at _Setup > Accounting > Accounting Preferences_, imported values for the Account field should include both account number and name, for example: 11000 Accounts Payable. If this preference isn't enabled, values should be account name only, for example: Accounts Payable.
    
-   If the Multiple Currencies feature is enabled, you must map the Exchange Rate field. If your CSV file doesn't include values for this field, you can set it to a default value. Currency values are taken from referenced vendors. See [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html).
    
-   If the vendor bills you're importing contain values for the Amount, Tax Amount, and Gross Amount fields, Gross Amount must be equal to the sum of the Amount and Tax Amount values.
    
-   If you're using a customized vendor bill form, please note that the Gross Amount field should never precede the Amount field on such a form. Otherwise it may affect the import of vendor bills CSV files.
    
-   Note that vendor bills are typically used to bring in open payables, not to link to open purchase orders.
    

For details about fields that can be mapped in the vendor bill record, see the SOAP Schema Browser's [vendor bill](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/vendorbill.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for Vendor Bill imports:

-   [Supported Vendor Bill Sublist Data Imports](#bridgehead_N427468)
    
-   [Using Multiple Files for Vendor Bill Sublist Data](#bridgehead_N428372)
    
-   [Supported Vendor Bill Subrecord Data Imports](#bridgehead_4314746116)
    
-   [Linking Purchase Orders to Vendor Bills](#bridgehead_1495016439)
    
-   [Importing Vendor Bills with Billed-Back Items and Expenses](#bridgehead_N428417)
    
-   [Importing Vendor Bills when Advanced Taxes is Enabled](#bridgehead_N428430)
    
-   [Importing Vendor Bills when Amortization is Enabled](#bridgehead_N428505)
    
-   [Sample Vendor Bill Single CSV File Format](#bridgehead_4337775811)
    
-   [Sample Vendor Bill Multiple CSV File Format](#bridgehead_4337777063)
    
-   [Using Import Assistant for Vendor Bills Mass Update](#bridgehead_N428538)
    

## Supported Vendor Bill Sublist Data Imports {#bridgehead_N427468}

The Vendor Bill import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Items | You must import at least one line item for all new records, and you must map required fields for this sublist on the Field Mapping page. See [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690). Selectively updatable based on Line/Order Line or Item key field. See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html). |
| Expenses | Expenses data must be in a separate CSV file. Selectively updatable based on Line/Order Line key field. |
| Accounting Book Detail | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on Accounting Book key field. |

If you use classes, departments, locations, or custom segments, you can set these values either for an entire vendor bill, or per individual item/expense lines.

If the Item Options feature is enabled in your account, you can import values for custom transaction item options along with Items sublist data. Transaction item options must first be set up at _Customization > Lists, Records, & Fields > Transaction Item Options > New_, with one of the following Applies To settings: Purchase, All Items. For details, see [Importing Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N430392.html).

For imports that update existing Vendor Bill records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

Important:

For non-keyed sublists, you shouldn't update main transaction fields and sublist fields during the same import job.

## Using Multiple Files for Vendor Bill Sublist Data {#bridgehead_N428372}

For vendor bill imports that include items data but no expenses data, you can choose the one file to upload option, and include all data in a single CSV file, or you can choose the multiple files to upload option, and include mainline data in one file and items data in another file.

For imports that include expenses data, it's best to use the multiple files to upload option, with one file for mainline data, and one for expenses data. If you're also importing items data, it should be in a third file.

For the multiple files option, be sure to include the external ID or key field values in the sublist files as well as in the main file.

Vendor bill CSV file formats are similar to those for purchase order CSV files. For examples, see: [Sample Purchase Order Single CSV File Format](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N423495.html#bridgehead_N424203), [Sample Purchase Order Multiple CSV File Format](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N423495.html#bridgehead_N424485).

## Supported Vendor Bill Subrecord Data Imports {#bridgehead_4314746116}

The Vendor Bill import supports the import of the following subrecord data:

| Subrecord | Notes |
| --- | --- |
| Items - Inventory Detail | When Advanced Bin/Numbered Inventory Management feature enabled. |
| Items - Landed Cost | When Landed Cost feature enabled. |

## Linking Purchase Orders to Vendor Bills {#bridgehead_1495016439}

The 2017.1 endpoint supports linking purchase orders to vendor bills in CSV import. This way you can populate a vendor bill with the items and expenses from one or more purchase orders.

Use the Purchase Order field on the field mapping page of the import assistant to map a purchase order to your vendor bill record. You can refer to purchase orders by name, external ID, or internal ID, and you can specify multiple purchase orders for the same vendor bill.

The Purchase Order field is a multi-select field. To specify multiple values, use multi-select value delimiters. For information about configuring delimiters, see [Custom Multi-Select Value Delimiter](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751045259.html).

Important:

If you map values to the Purchase Order field, you can't map values for the Expenses and Items sublists. If you try to map values both to the Purchase Order field and the Expenses or Items sublists, the following error message is displayed: "Please specify either purchase order list or item/expense list in the request but not both."

Note:

Partial billing of purchase orders isn't supported.

## Importing Vendor Bills with Billed-Back Items and Expenses {#bridgehead_N428417}

If you're importing vendor bills with items or expenses that need to be billed back to customers, you can set the value of the Billable field to 'TRUE' and include a value for the Customer field, for each of these item or expense lines.

## Importing Vendor Bills when Advanced Taxes is Enabled {#bridgehead_N428430}

If the Advanced Taxes feature is enabled, you're able to include tax codes and tax amounts in imported vendor bill items and expenses data. Tax codes should be set up in NetSuite before the import. Then you can include values for the Tax Code and Tax Amount fields for purchase order item and expense lines as needed. Note that other tax-related values for line items are calculated by the system.

The Advanced Taxes feature is required for NetSuite OneWorld accounts. For information about working with taxes in OneWorld, see [Nexuses and Taxes in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269581.html). For general information about setting up tax codes, see [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html).

## Importing Vendor Bills when Amortization is Enabled {#bridgehead_N428505}

If the Amortization feature is enabled, you're able to include amortization schedule, amortization start date, and amortization end date values in imported vendor bill items and expenses data. These values define how costs are allocated across a range of time and recognized in increments. Amortization schedules should be set up in NetSuite before the import. For information about setting up amortization in NetSuite, see [Expense Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1765678.html).

## Sample Vendor Bill Single CSV File Format {#bridgehead_4337775811}

The following table illustrates example column headers and data snippets in a single file upload of vendor bills. This file includes data for vendor bill header fields and item lines. Note that in this case, the same vendor bill number can be repeated in multiple rows.

| External ID | Vendor | Date | Item | Quantity | Location |
| --- | --- | --- | --- | --- | --- |
| VB1003 | American Computers | 4/21/2015 | Printer Accessories: Printer Cables | 10 | West Coast |
| VB1003 | \- | \- | Printer Accessories: Printer Ink Starter Pack | 15 | West Coast |
| VB1004 | Widget Works | 4/20/2015 | Office Supplies: 12-Pack Ball Point Pens | 25 | West Coast |

## Sample Vendor Bill Multiple CSV File Format {#bridgehead_4337777063}

The following tables illustrate example column headers and data snippets in a multiple file upload of vendor bills, including items and expenses data. Note that External ID is the key column that would be specified on the Import Assistant File Mapping page.

**Primary File:**

Each row of the primary file must include a unique identifier, in this case the external ID.

| External ID | Vendor | Date |
| --- | --- | --- |
| VB1003 | American Computers | 4/21/2015 |
| VB1004 | Widget Works | 4/20/2015 |

**Linked File - Items:**

The items file can include multiple rows with the same vendor bill external ID.

| External ID | Item | Quantity | Location |
| --- | --- | --- | --- |
| VB1003 | Printer Accessories: Printer Cables | 10 | West Coast |
| VB1003 | Printer Accessories: Printer Ink Starter Pack | 15 | West Coast |
| VB1004 | Office Supplies: 12-Pack Ball Point Pens | 25 | West Coast |

**Linked File - Expenses:**

The expenses file can include multiple rows with the same vendor bill external ID.

| External ID | Account | Amount | Memo | Customer | Billable |
| --- | --- | --- | --- | --- | --- |
| VB1003 | 6220 Repairs & Maintenance | 35 | installation | 107 Fabre Art Gallery | Yes |
| VB1004 | 6150 Office Expense | 5 | misc. | \- | No |

## Using Import Assistant for Vendor Bills Mass Update {#bridgehead_N428538}

You can perform a mass update of existing Vendor Bill data by creating a Transaction saved search with a filter of Type is Vendor Bill, changing data externally, then using the Import Assistant to import modified data, using the Update data handling option. For more information, see [Creating Transaction Saved Searches for Reimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N432599.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html), [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
