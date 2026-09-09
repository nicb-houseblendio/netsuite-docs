---
id: "section_N411251"
type: "section"
title: "Estimate Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Estimate Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N411251.html"
anchors: ["bridgehead_N411406", "bridgehead_4314737080", "bridgehead_N411638", "bridgehead_N411664"]
sha256: "55dee26745ef98ad2af66d38a7359c2c50bb9fecf6d5ba21f59288c98f39dcce"
---

NetSuite Estimates transactions, also known as Quotes, include items proposed for customer purchase, along with price levels, probabilities of closing, and expiration dates. Estimates can be provided to customers for review, and also can be used for sales forecasting, management, and reporting. Estimates can be attached to Opportunity records, and later can be converted to sales orders.

Note:

Estimate imports aren't available unless the Estimates feature is enabled in your account. To enable this feature, go to _Setup > Company > Enable Features_ and on the Transactions subtab, check the Estimates box.

-   You can import Estimate transaction data in a single CSV file, or in multiple files-for example, with transaction header data in one file and item-level data in other files. Estimate transactions can be uniquely identified by internal ID or external ID. The unique ID should be included in every line of the CSV files.
    
-   For imports of new data, use the external ID as a unique identifier. On the Import Assistant's Field Mapping page, map the external ID field from your CSV files to the NetSuite Estimate # field, which serves as a transaction ID for Estimate records. This mapping allows external IDs to be displayed on Estimate forms in the NetSuite user interface.
    
-   You can link an Estimate record to an Opportunity record by including the Opportunity record's identifier as the Estimate's 'Opportunity' field value. This identifier can be an internal ID, external ID, or transaction ID.
    
-   Each imported Estimate record should include a reference to a NetSuite customer record, mapped to the Estimate's Customer field. This reference must be a unique identifier; use the customer record's internal ID or external ID, rather than a name reference.
    

For details about fields that can be mapped in the estimate record, see the [estimate](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/estimate.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for Estimate imports:

-   [Supported Estimate Sublist Data Imports](#bridgehead_N411406)
    
-   [Supported Estimate Subrecord Data Imports](#bridgehead_4314737080)
    
-   [Importing Currency Values for Estimates](#bridgehead_N411638)
    
-   [Using Import Assistant for Estimates Mass Updates](#bridgehead_N411664)
    

## Supported Estimate Sublist Data Imports {#bridgehead_N411406}

The Estimate import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Items | You must import at least one line item for all new records, and you must map required fields for this sublist on the Field Mapping page. See [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690). Selectively updatable based on Line/Order Line or Item key field. See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html). |
| Partners | when Multi-Partner Management feature enabled selectively updatable based on Internal ID, External ID, or Partner |
| Sales Team | when Team Selling feature enabled |

If the Item Options feature is enabled in your account, you can import values for custom transaction item options along with Items sublist data. Transaction item options must first be set up at _Customization > Lists, Records, & Fields > Transaction Item Options > New_, with one of the following Applies To settings: Sale, All Items. For details, see [Importing Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N430392.html).

For imports that update existing Estimate records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

Important:

For non-keyed sublists, you shouldn't update main transaction fields and sublist fields during the same import job.

## Supported Estimate Subrecord Data Imports {#bridgehead_4314737080}

The Estimate import supports the import of the following subrecord data:

| Subrecord | Notes |
| --- | --- |
| Items - Inventory Detail | when Advanced Bin / Numbered Inventory Management feature enabled |

## Importing Currency Values for Estimates {#bridgehead_N411638}

When the Multiple Currencies feature is enabled, the import of Currency field values is supported for newly created estimates. The Currency value for an estimate must be one of the currencies defined for the transaction's customer, on the Customer Currencies sublist. See [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html) and [Setting Multiple Transaction Currencies for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383794.html#bridgehead_N385568).

If the Multiple Currencies feature is't enabled, the Currency field value for an estimate isn't editable.

## Using Import Assistant for Estimates Mass Updates {#bridgehead_N411664}

You can perform a mass update of existing Estimates data by exporting results for a Transaction saved search with a filter of 'Type is Estimate', changing data externally, then using the Import Assistant to import modified data, using the Update data handling option. For more information, see [Creating Transaction Saved Searches for Reimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N432599.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
