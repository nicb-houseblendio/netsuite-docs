---
id: "section_N411794"
type: "section"
title: "Invoice Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Invoice Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N411794.html"
anchors: ["bridgehead_N414117", "bridgehead_4314738660", "bridgehead_N414430", "bridgehead_N414456", "bridgehead_1525951242"]
sha256: "5a3c1f18049ba0a0bf466726c14afc9cd7cf2c357a3714c5ff53715347cdb2a0"
---

NetSuite Invoice transactions are records of sales for which payment is not received at the time of delivery. Invoice records include the items sold, their prices, and payment terms.

You can use the invoice import to import historical sales data. If you're also importing customer payments, and you want to apply imported payments to imported invoices, you need to import invoices first, and include unique IDs, preferably external IDs. You can then reference invoices in your customer payment import file.

If the Use Account Numbers preference has been enabled at _Setup > Accounting > Accounting Preferences_, imported values for the Account field should include both account number and name, for example: 11000 Accounts Payable. If this preference isn't enabled, values should be account name only, for example: Accounts Payable.

Important:

A payment can be associated with an invoice through the internal ID or external ID only. The transaction ID is not unique and can't be used.

For details about fields that can be mapped in the invoice record, see the SOAP Schema Browser's [invoice](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/invoice.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for invoice imports:

-   [Supported Invoice Sublist Data Imports](#bridgehead_N414117)
    
-   [Supported Invoice Subrecord Data Imports](#bridgehead_4314738660)
    
-   [Importing Currency Values for Invoices](#bridgehead_N414430)
    
-   [Using Import Assistant for Invoices Mass Update](#bridgehead_N414456)
    

## Supported Invoice Sublist Data Imports {#bridgehead_N414117}

The Invoice import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Accounting Book Detail | Available when Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on Accounting Book key field. |
| Auth. Code | When Gift Certificates feature enabled. |
| Billable Expenses | When Projects and Advanced Billing are enabled. |
| Billable Time | Selectively updatable based on related transaction ID (\*\*\*doc). |
| Items | You must import at least one line item for all new records, and you must map required fields for this sublist on the Field Mapping page. See [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690). Selectively updatable based on Line/Order Line or Item key field. See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html). |
| Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Internal ID, External ID, or Partner. |
| Sales Team | When Team Selling feature enabled. |
| Shipment | When Multiple Shipping Routes feature enabled. |

If the Item Options feature is enabled in your account, you can import values for custom transaction item options along with Items sublist data. Transaction item options must first be set up at _Customization > Lists, Records, & Fields > Transaction Item Options > New_, with one of the following Applies To settings: Sale, All Items. For details, see [Importing Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N430392.html).

For imports that update existing Invoice records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

Important:

For non-keyed sublists, you shouldn't update main transaction fields and sublist fields during the same import job.

## Supported Invoice Subrecord Data Imports {#bridgehead_4314738660}

The Invoice import supports the import of the following subrecord data:

| Subrecord | Notes |
| --- | --- |
| Billing Address | By default, the subrecord Address field is read-only, and data from other subrecord fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |
| Items - Inventory Detail | When Advanced Bin/Numbered Inventory Management feature enabled. |
| Shipping Address | By default, the subrecord Address field is read-only, and data from other subrecord fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |

## Importing Currency Values for Invoices {#bridgehead_N414430}

When the Multiple Currencies feature is enabled, the import of Currency field values is supported for newly created invoices. The Currency value for an invoice must be one of the currencies defined for the transaction's customer, on the Customer Currencies sublist. See [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html) and [Setting Multiple Transaction Currencies for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383794.html#bridgehead_N385568).

If the Multiple Currencies feature isn't enabled, the Currency field value for an invoice isn't editable.

## Using Import Assistant for Invoices Mass Update {#bridgehead_N414456}

You can perform a mass update of existing Invoices data by exporting Invoices saved search results, changing data externally, then using the Import Assistant to import modified data, using the Update data handling option. For more information, see [Creating Transaction Saved Searches for Reimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N432599.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

## Invoice Import Example {#bridgehead_1525951242}

The following example shows how you might structure a file for importing cash sale data.

| External ID | Customer | Date | Posting Period | Location | Currency | Exchange Rate | Item | Amount |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Inv-00001 | Tim Mason | 5/10/2018 | May 2018 | Atlantic City | US USD | 1.00 | Travel Kit - Medium | 15 |
| Inv-00002 | Anne Woods | 5/11/2018 | May 2018 | San Mateo | US USD | 1.00 | Travel Kit - Small | 10 |

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235134.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
