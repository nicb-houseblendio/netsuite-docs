---
id: "section_N426302"
type: "section"
title: "Sales Order Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Sales Order Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N426302.html"
anchors: []
sha256: "742176798ab14601f4c9022805f9bcd601f23b8d48ab26793dc5bed04c641aa0"
---

NetSuite Sales Order transactions record a commitment to sell items or services to a customer, including the items to be sold and their prices. Sales orders can be converted from existing estimate transactions, or created as new transactions. Sales orders can be attached to opportunity transactions.

For more details about Sales Orders in NetSuite, see [Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1215966.html).

Note:

Sales Order imports aren't available unless the Sales Orders feature is enabled in your account. To enable this feature, go to _Setup > Company > Enable Features_ and on the Transactions subtab, check the Sales Orders box.

-   You can import Sales Order transaction data in a single CSV file or in multiple files-for example, with transaction header data in one file and item-level data in other files.
    
-   By default, the NetSuite fields available for sales orders import mapping are those available on the standard sales order form. Fields can be mapped for the import job if they're displayed (not hidden) and not disabled on your preferred form. To make different fields available, you can specify a custom sales order form on the Import Options page. For information, see [Custom Form Specification for Sales Order Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698171281.html).
    
-   You must map external ID or internal ID to serve as a unique ID per record. The unique ID should be included in every line of the CSV files.
    
-   For imports of new data, use external ID. On the Import Assistant's Field Mapping page, map the external ID field from your CSV files to the NetSuite Order # field, which serves as a transaction ID for Sales Order records. This way, external IDs show up on Sales Order forms in NetSuite.
    
-   You can link a Sales Order record to an Opportunity record by including the Opportunity record's unique identifier as the Sales Order's 'Opportunity' field value. This identifier can be an internal ID, external ID, or transaction ID.
    
-   Each imported Sales Order record should include a reference to a NetSuite Customer record, mapped to the Sales Order's Customer field. This reference must be a unique identifier; use the customer record's internal ID or external ID, rather than a name reference.
    
-   By default, Billing Address and Shipping Address fields for Sales Order records are copied from linked Customer records, but these fields are available for mapping in the Import Assistant, so their values can be set by CSV files' field values instead.
    
-   The Billing Schedule field available for Sales Orders imports can be set to reference existing NetSuite billing schedules only.
    
-   The Commitment Confirmed field is available only for updating a Sales Order record and not when adding a new one. For the Add operation, the field isn't available on the field mapping page. For the Update and the Add or Update operations, the field is available, but its value is ignored when adding a new record.
    

For details about fields that can be mapped in the sales order record, see the SOAP Schema Browser's [sales order](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/salesorder.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for sales order imports:

-   [Custom Form Specification for Sales Order Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698171281.html)
    
-   [Supported Sales Order Sublist Data Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698170486.html)
    
-   [Supported Sales Order Subrecord Data Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698169967.html)
    
-   [Setting Imported Sales Orders' Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698169438.html)
    
-   [Setting Sales Orders to Closed](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698168976.html)
    
-   [Importing Currency Values for Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698168642.html)
    
-   [Charging Custom Credit Cards for Imported Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698168054.html)
    
-   [Using Import Assistant for Sales Orders Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698166132.html)
    
-   [Sales Order Import Multi-File Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698175690.html)
    

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
