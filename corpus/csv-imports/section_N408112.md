---
id: "section_N408112"
type: "section"
title: "Credit Memo Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Credit Memo Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N408112.html"
anchors: ["bridgehead_N408230", "bridgehead_N408251", "bridgehead_N409034", "bridgehead_N410278", "bridgehead_N410388", "bridgehead_4314735859", "bridgehead_N410608"]
sha256: "f0312f3d2ae5aa4762f36a496412251a1a22abdba86f9c572bf08a64b85ad378"
---

A credit memo is a record of credit due to a customer. Credit memo amounts can be applied toward the charges for specific items and for specific transactions such as invoices. For information about using credit memos in NetSuite, see [Customer Credit Memos](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1311306.html).

Note:

Credit memo imports aren't available unless the A/R (Accounts Receivable) feature is enabled in your account. To enable this feature, go to _Setup > Company > Enable Features_ and on the Accounting subtab, check the A/R box.

Review the following guidelines for Credit Memo imports:

-   [Supported CSV File Formats for Credit Memo Imports](#bridgehead_N408230)
    
-   [Notes on Credit Memo Import Field Values](#bridgehead_N410278)
    
-   [Supported Credit Memo Sublist Data Imports](#bridgehead_N410388)
    
-   [Supported Credit Memo Subrecord Data Imports](#bridgehead_4314735859)
    
-   [Setting the Form for a Credit Memo Import](#bridgehead_N410608)
    

## Supported CSV File Formats for Credit Memo Imports {#bridgehead_N408230}

Credit memo records include Items and Apply sublists:

-   An items sublist stores data about the items returned by the customer under this credit memo.
    
-   An apply sublist contains unpaid open invoices to which the credit memo amount can be applied partly or in whole, decreasing the amount due to be paid by the customer. The invoices are referenced by their internal or external IDs.
    

Credit memo imports may also support the import of data for Partners and Sales Team sublists. See [Supported Credit Memo Sublist Data Imports](#bridgehead_N410388).

Note:

To maintain performance, don't submit transactions that contain more than 5000 lines through CSV import.

## Multi-File Format {#bridgehead_N408251}

Generally, a multi-file format is preferred for imports of transactions that support multiple sublists. In this format, body data is in a primary CSV file, Items sublist data is in a linked file, Apply sublist data is in another linked file, and data for any other sublists is in other linked files. The following tables illustrate sample data in a multi-file credit memo import.

CreditMemo.csv - primary file with body data:

| External ID | Customer | Location | Memo |
| --- | --- | --- | --- |
| CM-PT3-042601 | ABC Trucking | Biloxi | Returned Carburetors |
| CM-PT3-042602 | Happy Day Motors | Atlanta | Good Customer Credit |
| CM-PT3-042603 | Smithson Auto Body | Atlanta | Returned Alternators |

CreditMemoItems.csv - linked file with Items sublist data:

| External ID | Item | Quantity | Amount |
| --- | --- | --- | --- |
| CM-PT3-042601 | Carburetor MK60 | 10 | 2500.00 |
| CM-PT3-042601 | Carburetor MK65 | 5 | 1500.00 |
| CM-PT3-042603 | Alternator BS40 | 2 | 600.00 |
| CM-PT3-042603 | Alternator BS52 | 3 | 300.00 |

CreditMemoApply.csv - linked file with Apply sublist data:

| External ID | Apply | Payment |
| --- | --- | --- |
| CM-PT3-042601 | 115602 | 2500.00 |
| CM-PT3-042601 | 115603 | 1500.00 |
| CM-PT3-042601 | 115604 | 750.00 |
| CM-PT3-042602 | 115605 | 500.00 |
| CM-PT3-042603 | 115606 | 300.00 |
| CM-PT3-042603 | 115607 | 1200.00 |

## Single-File Format with Multiple Rows per Record {#bridgehead_N409034}

The credit memo import also supports a single-file format where you can include body data and data from multiple sublists in one primary file. This single file can contain multiple rows for each credit memo record; each row only must include the external ID value, so all data can be tied to the record. The following table illustrates a single CSV file that contains body data, Items sublist data, and Apply sublist data.

CreditMemoSingleFile.csv:

| External ID | Customer | Item | Quantity | Apply | Payment |
| --- | --- | --- | --- | --- | --- |
| CM-PT3-042601 | ABC Trucking | Carburetor MK60 | 10 | EXTINV02134 | 2500.00 |
| CM-PT3-042601 | \- | Carburetor MK65 | 3 | EXTINV02183 | 1500.00 |
| CM-PT3-042601 | \- | \- | \- | EXTINV02190 | 750.00 |
| CM-PT3-042602 | Happy Day Motors | \- | \- | EXTSO12456 | 500.00 |
| CM-PT3-042603 | Smithson Auto Body | Alternator BS40 | 2 | \- | \- |
| CM-PT3-042603 | \- | Alternator BS52 | 3 | EXTINV02199 | 300.00 |
| CM-PT3-042603 | \- | \- | \- | EXTINV02210 | 1200.00 |

In this sample:

-   External ID and Customer fields are body fields. External ID values are repeated in multiple rows to indicate links for sublist data. Other body field values don't need to be repeated in multiple rows.
    
-   Item and Quantity are Items sublist fields. Blank values for these fields indicate there's no data.
    
-   Apply and Payment are Apply sublist fields. Blank values for these fields indicate there's no data.
    

## Notes on Credit Memo Import Field Values {#bridgehead_N410278}

-   You must map external ID or internal ID to serve as a unique ID per record. The unique ID should be included in every line of the CSV files. For imports of new data, use external ID. On the Import Assistant's Field Mapping page, map the external ID field from your CSV files to the Credit # field, which serves as a transaction ID for credit memo records. This mapping allows external IDs to be displayed on credit memo forms in the NetSuite user interface.
    
-   Each imported credit memo record should include a reference to a NetSuite customer record, mapped to the credit memo's Customer field. This reference must be a unique identifier; use internal ID or external ID, rather than a name reference. If you don't map a reference number field, reference number values are generated automatically.
    
-   You don't have to map the required Date field. If you don't map the Date field, it's mapped automatically with default values of the current date.
    
-   If the Multiple Currencies feature is enabled, map the Exchange Rate field. If your CSV file doesn't include values for this field, you can set it to a default value. Currency values are taken from referenced customers. If your customers use currencies other than the currency in which your company manages its financials, map the Currency field. For more information, see [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html).
    
-   If the Use Account Numbers preference has been enabled at _Setup > Accounting > Accounting Preferences_, imported values for the Account field should include both account number and name, for example: 11000 Accounts Payable. If this preference isn't enabled, values should be account name only, for example: Accounts Payable.
    

For more details about fields that can be mapped in the credit memo record, see the SOAP Schema Browser's [credit memo](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/creditmemo.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Supported Credit Memo Sublist Data Imports {#bridgehead_N410388}

The Credit Memo import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Apply | Selectively updatable based on Apply or Line key field. |
| Items | Selectively updatable based on Order Line or Item key field. See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html). |
| Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Partner key field. |
| Sales Team | When Team Selling feature enabled. Selectively updatable based on Employee key field. |

To apply credit memos to invoices or other transactions, specify invoice numbers as Apply field values, in the Apply sublist. When you import this sublist's data, you can also set Line ID values to uniquely identify each Apply line, and Payment values to set the credit memo amounts to be applied to invoices.

For imports that update existing credit memo records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

## Supported Credit Memo Subrecord Data Imports {#bridgehead_4314735859}

The Credit Memo import supports the import of the following subrecord data:

| Subrecord | Notes |
| --- | --- |
| Billing Address | By default, the subrecord Address field is read-only, and data from other subrecord fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |
| Items - Inventory Detail | when Advanced Bin / Numbered Inventory Management feature enabled |
| Shipping Address | By default, the subrecord Address field is read-only, and data from other subrecord fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |

## Setting the Form for a Credit Memo Import {#bridgehead_N410608}

By default, the Field Mapping page for a credit memo import displays the NetSuite fields from your preferred credit memo form. You can select a different credit memo form in the Advanced Options area of the Import Assistant's Import Options page. See [Custom Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751044597.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Customer Credit Memos](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1311306.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)
-   [Credit Card Charge Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4676571596.html)
-   [Credit Card Refund Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4676571713.html)
-   [Credit Memo Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N408112.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
