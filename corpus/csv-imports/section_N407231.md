---
id: "section_N407231"
type: "section"
title: "Cash Sale Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Cash Sale Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N407231.html"
anchors: ["bridgehead_N407381", "bridgehead_4314716176", "bridgehead_N407694", "bridgehead_N407925", "procedure_N407938", "bridgehead_N407966", "bridgehead_1502968327"]
sha256: "3a49c1e04c762106dbaad263d42995d0255ecb6217a1a271d8a7652c263fbd5e"
---

NetSuite Cash Sale transactions are records of sales for which immediate payment is received. You can use the cash sales import to import historical sales data.

For details about fields that can be mapped in the cash sale record, see the SOAP Schema Browser's [cash sale](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/cashsale.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for Cash Sale imports:

-   [Supported Cash Sale Sublist Data Imports](#bridgehead_N407381)
    
-   [Supported Cash Sale Subrecord Data Imports](#bridgehead_4314716176)
    
-   [Importing Currency Values for Cash Sale Transactions](#bridgehead_N407694)
    
-   [Charging Customer Credit Cards for Imported Cash Sales](#bridgehead_N407925)
    
-   [Using Import Assistant for Cash Sales Mass Update](#bridgehead_N407966)
    
-   [Cash Sale Import Example](#bridgehead_1502968327)
    

## Supported Cash Sale Sublist Data Imports {#bridgehead_N407381}

The Cash Sale import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Auth. Code | When Gift Certificates feature enabled. |
| Billable Time | Selectively updatable based on related transaction ID (\*\*\*doc). |
| Items | You must import at least one line item for all new cash sale records, and you must map required fields for this sublist on the Field Mapping page. See [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690). Selectively updatable based on Line/Order Line or Item key field. See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html). |
| Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Internal ID, External ID, or Partner. |
| Sales Team | When Team Selling feature enabled. |
| Shipment | When Multiple Shipping Routes feature enabled. |

If the Item Options feature is enabled in your account, you can import values for custom transaction item options along with Items sublist data. Transaction item options must first be set up at _Customization > Lists, Records, & Fields > Transaction Item Options > New_, with one of the following Applies To settings: Sale, All Items. For details, see [Importing Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N430392.html).

For imports that update existing Cash Sale records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

Important:

For non-keyed sublists, don't update main transaction fields and sublist fields during the same import job.

## Supported Cash Sale Subrecord Data Imports {#bridgehead_4314716176}

The Cash Sale import supports the import of the following subrecord data:

| Subrecord | Notes |
| --- | --- |
| Billing Address | By default, the subrecord Address field is read-only, and data from other subrecord fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |
| Items - Inventory Detail | When Advanced Bin / Numbered Inventory Management feature enabled. |
| Shipping Address | By default, the subrecord Address field is read-only, and data from other subrecord fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |

## Importing Currency Values for Cash Sale Transactions {#bridgehead_N407694}

When the Multiple Currencies feature is enabled, the import of Currency field values is supported for newly created cash sale transactions. The Currency value for a cash sale must be one of the currencies defined for the transaction's customer, on the Customer Currencies sublist. See [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html) and [Setting Multiple Transaction Currencies for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383794.html#bridgehead_N385568).

If the Multiple Currencies feature isn't enabled, the Currency field value for a cash sale isn't editable.

## Charging Customer Credit Cards for Imported Cash Sales {#bridgehead_N407925}

By default, imports of Cash Sale records don't cause charges to customer credit cards. If your NetSuite account has integrated credit card processing set up, you can set up a Cash Sale import to create charges to customer credit cards.

#### To set up a Cash Sale import to charge customer credit cards: {#procedure_N407938}

1.  On the Field Mapping page for a Cash Sale import, double-click the Charge Credit Card field to display it in the center pane.
    
2.  Click the edit icon and set the default value for the field to be Yes.
    
    If you don't map the Charge Credit Card field for a Cash Sales import, its value remains No, and no credit card charges occur.
    

## Using Import Assistant for Cash Sales Mass Update {#bridgehead_N407966}

You can perform a mass update of existing Cash Sales data by exporting Cash Sales saved search results, changing data externally, then using the Import Assistant to import modified data, using the Update data handling option. For more information, see [Creating Transaction Saved Searches for Reimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N432599.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

## Cash Sale Import Example {#bridgehead_1502968327}

The following example shows how you might structure a file for importing cash sale data.

| External ID | Customer | Date | Item | Quantity | Amount | Tax Code |
| --- | --- | --- | --- | --- | --- | --- |
| CS-1234 | Amy Johnson | 8/17/2017 | Model railway set - KHT15 | 2 | 1400 | VT-855 |
| CS-1235 | Zachary Hayes | 8/17/2017 | Model aircraft - BHY54 | 3 | 2500 | VT-97 |

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
