---
id: "section_N429795"
type: "section"
title: "Vendor Return Authorization Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Vendor Return Authorization Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N429795.html"
anchors: ["bridgehead_N430001", "bridgehead_N430206", "bridgehead_4314753745", "bridgehead_N430232", "bridgehead_N430244", "bridgehead_N430277"]
sha256: "39d2930dd8cc8e06e5c6a79f945c2d7cf96780892f8af4adf62a8b7ad76e304d"
---

A vendor return authorization is a non-posting transaction that tracks a return to a vendor, including the items to be returned, their quantities, the approval status, the shipment status, and the amount refunded or credited from the vendor. The vendor return process includes four steps: creating a vendor return authorization record, approving or canceling the authorization, shipping items authorized to be returned, and crediting an authorized vendor return.

Note:

To maintain performance, don't submit transactions that contain more than 5000 lines through CSV import.

For details about vendor return authorizations in NetSuite, see [Vendor Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2386193.html).

Note:

Vendor Return Authorization imports aren't available unless the Vendor Return Authorizations feature is enabled in your account. To enable this feature, go to _Setup > Company > Enable Features_ and on the Transactions subtab, check the Vendor Return Authorizations box.

-   Vendor return authorization imports can include line-level items and expenses data. For imports with items data, but no expenses data, you can choose either the one file to upload or the multiple files to upload option. For imports with expenses data, you **must** choose the multiple files to upload option. For more information, see [Using Multiple Files for Vendor Return Authorization Sublist Data](#bridgehead_N430206).
    
-   You must map external ID or internal ID to serve as a unique ID per record. The unique ID should be included in every line of the CSV files. For imports of new data, use external ID. On the Import Assistant's Field Mapping page, map the external ID field from your CSV files to the NetSuite Reference No. field, which serves as a transaction ID for Vendor Return Authorization records. This mapping allows external IDs to be displayed on Vendor Return Authorization forms in the NetSuite user interface.
    
-   Each imported Vendor Return Authorization record should include a reference to a NetSuite Vendor record, mapped to the Vendor Return Authorization's Vendor field. This reference must be a unique identifier; use internal ID or external ID, rather than a name reference. If you don't map a reference number field, reference number values are generated automatically.
    
-   If the Use Account Numbers preference has been enabled at _Setup > Accounting > Accounting Preferences_, imported values for the Account field should include both account number and name, for example: 11000 Accounts Payable. If this preference isn't enabled, values should be account name only, for example: Accounts Payable.
    
-   If the Multiple Currencies feature is enabled, you must map the Exchange Rate field. If your CSV file doesn't include values for this field, you can set it to a default value. Currency values are taken from referenced vendors. See [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html).
    

For details about fields that can be mapped in the Vendor Return Authorization record, see the SOAP Schema Browser's [vendor return authorization](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/vendorreturnauthorization.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for Vendor Return Authorization imports:

-   [Supported Vendor Return Authorization Sublist Data Imports](#bridgehead_N430001)
    
-   [Using Multiple Files for Vendor Return Authorization Sublist Data](#bridgehead_N430206)
    
-   [Supported Vendor Return Authorization Subrecord Data Imports](#bridgehead_4314753745)
    
-   [Importing Vendor Return Authorizations with Billed-Back Items and Expenses](#bridgehead_N430232)
    
-   [Importing Vendor Return Authorizations when Amortization is Enabled](#bridgehead_N430244)
    
-   [Using Import Assistant for Vendor Return Authorizations Mass Update](#bridgehead_N430277)
    

## Supported Vendor Return Authorization Sublist Data Imports {#bridgehead_N430001}

The Vendor Bill import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Items | You must import at least one line item for all new records, and you must map required fields for this sublist on the Field Mapping page. See [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690). Selectively updatable based on Line/Order Line or Item key field. See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html). |
| Expenses | Expenses data must be in a separate CSV file. Selectively updatable based on Line/Order Line key field. |
| Accounting Book Detail | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on Accounting Book key field. |

If you use classes, departments, or locations, you can set these values either for an entire vendor return authorization, or per individual item/expense lines.

If the Item Options feature is enabled in your account, you can import values for custom transaction item options along with Items sublist data. Transaction item options must first be set up at _Customization > Lists, Records, & Fields > Transaction Item Options > New_, with one of the following Applies To settings: Purchase, All Items. For details, see [Importing Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N430392.html).

For imports that update existing Vendor Return Authorization records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

## Using Multiple Files for Vendor Return Authorization Sublist Data {#bridgehead_N430206}

For vendor return authorization imports that include items data but no expenses data, you can choose the one file to upload option, and include all data in a single CSV file, or you can choose the multiple files to upload option, and include mainline data in one file and items data in another file.

For imports that include expenses data, you **must** use the multiple files to upload option, with one file for mainline data, and one for expenses data. If you're also importing items data, it should be in a third file.

For the multiple files option, be sure to include the external ID or key field values in the sublist files as well as in the main file.

## Supported Vendor Return Authorization Subrecord Data Imports {#bridgehead_4314753745}

The Vendor Return Authorization import supports the import of the following subrecord data:

| Subrecord | Notes |
| --- | --- |
| Items - Inventory Detail | When Advanced Bin/Numbered Inventory Management feature enabled |

## Importing Vendor Return Authorizations with Billed-Back Items and Expenses {#bridgehead_N430232}

If you're importing vendor return authorizations with items or expenses that need to be billed back to customers, you can set the value of the Billable field to 'TRUE' and include a value for the Customer field, for each of these item or expense lines.

## Importing Vendor Return Authorizations when Amortization is Enabled {#bridgehead_N430244}

If the Amortization feature is enabled, you're able to include amortization schedule, amortization start date, and amortization end date values in imported vendor return authorization items and expenses data. These values define how costs are allocated across a range of time and recognized in increments. Amortization schedules should be set up in NetSuite before the import. For information about setting up amortization in NetSuite, see [Expense Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1765678.html).

## Using Import Assistant for Vendor Return Authorizations Mass Update {#bridgehead_N430277}

You can perform a mass update of existing Vendor Return Authorization data by creating a Transaction saved search with a filter of Type is Vendor Return Authorization, changing data externally, then using the Import Assistant to import modified data, using the Update data handling option. For more information, see [Creating Transaction Saved Searches for Reimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N432599.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
