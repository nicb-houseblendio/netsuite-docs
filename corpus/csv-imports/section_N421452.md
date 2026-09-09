---
id: "section_N421452"
type: "section"
title: "Opportunity Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Opportunity Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N421452.html"
anchors: ["bridgehead_N421668", "bridgehead_N423030", "bridgehead_N423051", "bridgehead_3705047133", "bridgehead_3705047541"]
sha256: "d216044705c86be9f8287a23118d3ca3c79c747fb1654d7f2f54c4b764e4635e"
---

NetSuite Opportunity transactions document negotiations with potential customers (Prospects). Opportunities are created upon customer contact, and are used for record keeping, sales forecasting, sales management, and sales reporting purposes. Each Opportunity record includes items in which the customer is interested, and can have attached estimates or sales orders, and attached activities such as tasks, events, and phone calls.

For more details about Opportunities in NetSuite, see [Opportunity Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1066171.html).

-   You can import Opportunity transaction data in a single CSV file, or in multiple files-for example, with transaction header data in one file and item-level data in other files. Opportunity transactions can be uniquely identified by internal ID or external ID. The unique ID should be included in every line of the CSV files.
    
-   For imports of new data, a key of external ID is preferred. On the Import Assistant's Field Mapping page, map the external ID field from your CSV files to the NetSuite Opportunity # field, which serves as a transaction ID for Opportunity records. This mapping allows external IDs to be displayed on Opportunity forms in the NetSuite user interface.
    
-   Each imported Opportunity record should include a reference to a NetSuite Customer record, mapped to the Opportunity's Company field. This reference must be a unique identifier; use the customer record's internal ID or external ID, rather than a name reference.
    
-   The Status field is required for imported Opportunity records. Status field values for customers can be entered at _Setup > Sales > Customer Statuses_. The Import Assistant Field Mapping page lets you set a default value for Status.
    
-   Other required fields are Probability, Date Created, and Expected Close. The user interface automatically calculates Probability based on Status; the Import Assistant does the same. Formatting for Date Created and Expected should match the Date Format set at _Setup > Company > General Preferences_.
    

Note:

If you're importing historical data for opportunities that have been previously closed, be sure to set Status field values to 'Closed Lost' or 'Closed Won'. The Close Date field value for all records imported with closed statuses are set to the date that the import job adds or updates the records. You can't modify Close Date field values to be any other date.

For details about fields that can be mapped in the opportunity record, see the SOAP Schema Browser's [opportunity](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/opportunity.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for Opportunity imports:

-   [Supported Opportunity Sublist Data Imports](#bridgehead_N421668)
    
-   [Using Import Assistant for Opportunities Mass Update](#bridgehead_N423030)
    
-   [Advanced Forecasting and Opportunities' Projected Total Values](#bridgehead_N423051)
    

## Supported Opportunity Sublist Data Imports {#bridgehead_N421668}

The Opportunity import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Items | Selectively updatable based on Line/Order Line or Item key field. See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html). |
| Opportunity | (Related Opportunities) |
| Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Internal ID, External ID, or Partner field. |
| Sales Team | When Team Selling feature enabled. |

If the Item Options feature is enabled in your account, you can import values for custom transaction item options along with Items sublist data. Transaction item options must first be set up at _Customization > Lists, Records, & Fields > Transaction Item Options > New_, with one of the following Applies To settings: Opportunity, All Items. For details, see [Importing Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N430392.html).

For imports that update existing Opportunity records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

Important:

For non-keyed sublists, you shouldn't update main transaction fields and sublist fields during the same import job.

## Using Import Assistant for Opportunities Mass Update {#bridgehead_N423030}

You can perform a mass update of existing Opportunity data by exporting Opportunity saved search results, changing data externally, then using the Import Assistant to import modified data, using the Update data handling option. For more information, see [Creating Transaction Saved Searches for Reimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N432599.html).

## Advanced Forecasting and Opportunities' Projected Total Values {#bridgehead_N423051}

Be aware of potential issues for imports of Opportunity records' Projected Total field values. When Opportunity transactions are added or updated in the user interface, this field's values are calculated based on Items sublist data and attached Estimates' data, but can be overridden by user entries.

For imports of Opportunity transactions, Projected Total field values are calculated in a variety of manners, depending on whether the imported Opportunities include Items sublist data, on whether your account has the Advanced Forecasting feature enabled and you have enabled the Multiple Sales Projected Amount Preference, and on whether the import is adding or updating NetSuite records.

Review the following scenarios and ensure that Projected Total field values are populated appropriately in your CSV files for Opportunity imports:

## When Advanced Forecasting Feature is Disabled {#bridgehead_3705047133}

-   For Adds:
    
    -   If CSV files don't include Items sublist data, Projected Total field values are required to avoid errors.
        
    -   If CSV files include Items sublist data but no Projected Total field values, these imported records' Projected Total field values are calculated to be the sum of items.
        
    -   If CSV files include both Items sublist data and Projected Total field values, the Projected Total field values are used to set values for imported records.
        
-   For Updates:
    
    -   If CSV files don't include Items sublist data or Projected Total field values, existing NetSuite Projected Total field values are not changed by the import.
        
    -   If CSV files include Items sublist data but no Projected Total field values, existing NetSuite Projected Total field values are updated to be the sum of all items, both preexisting and imported.
        
    -   If CSV files include Projected Total field values, these values replace imported records' preexisting Projected Total field values.
        

## When Advanced Forecasting Feature and Multiple Sales Projected Amount Preference are Enabled {#bridgehead_3705047541}

With Advanced Forecasting and Multiple Sales Projected Amount enabled, two additional fields are available relating to the Opportunity Projected Total field: a Range Low and Range High.

-   CSV files' Range Low field values must be lower than or equal to Projected Total field values. Range Low values represent Worst Case projected totals.
    
-   CSV files' Range High field values must be greater than or equal to Projected Total field values. Range High values represent Upside projected totals.
    
-   For Adds:
    
    -   If CSV files don't include Items sublist data, Projected Total field values are required to avoid errors.
        
    -   If CSV files don't include Items sublist data, do include Projected Total field values, and one or both of Range Low and Range High fields are missing, then field values for Range Low and Range High are set to Projected Total field value.
        
    -   If CSV files include Items sublist data but are missing Projected Total, Range Low, or Range High field values, any missing values are calculated to be the sum of items.
        
    -   Any values in CSV files for Projected Total, Range Low, and Range High are used to set imported records' field values, whether Items sublist data is included.
        
-   For Updates:
    
    -   If any of the values for an import file record's Projected Total, Range Low, or Range High field is the same as the existing record's field value, then all three fields' values are calculated based on the sum of items.
        
    -   If an import file record's Projected Total, Range Low, and Range High fields all have different values than the existing record's fields, then none of the field values are calculated based on the sum of items, and the Projected Total field value is set to the value submitted in the import file.
        
    -   If an import file record doesn't have a value for Projected Total, Range Low, or Range High, then all three fields' values are calculated based on sum of items, unless there's no change to Items sublist data.
        

The Advanced Forecasting feature is enabled at _Setup > Company > Enable Features_, on the CRM subtab's Sales section. For information about this feature, see [Advanced Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1047034.html).

The Multiple Sales Projected Amount Preference is enabled at _Setup > Sales > Sales Preferences_, on the Forecasts Subtab. For information about this preference, see [Forecasting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1046772.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Opportunity Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1066171.html)
-   [Advanced Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1047034.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
