---
id: "section_N363414"
type: "section"
title: "Notes Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Communications Import Type > Notes Import"
parent: "section_N363101"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363414.html"
anchors: []
sha256: "dbdcce7aad0cb2979c732af758cd3cd9af20707e9feb7eea172f5169cfd8ee4d"
---

The Notes import adds or updates Note records in NetSuite. Notes are used to attach information to other NetSuite records.

CSV file note records should include references to the NetSuite record to which they're attached. These reference values can be in one of the following fields (as shown on the Import Assistant Field Mapping page:

-   CRM/Support Record
    
-   Entity (for Customer or Contact records)
    
-   Item
    
-   Transaction (for Opportunity records)
    

The Date field on note records is a Date/Time type. CSV file values for this field can be include dates only or both dates and times. If a value is date-only, the time defaults to the current time (time of the import).

If you're doing a notes import for the addition of new notes, select the **Add** data handling option, rather than **Add or Update**.

If you need to import updates to existing note records, you should use an identifier of internal ID or external ID, to prevent duplication of records.

-   If you select the **Update** data handling option, you can use the Title as an identifier to match records and perform updates.
    
-   If you select the **Add or Update** data handling options, no Title lookups are performed, so in the absence of internal ID or external ID, multiple notes with the same title may be added.
    

For details about fields that can be mapped in the note record, see the SOAP Schema Browser's [note](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/note.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Communications Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363101.html)
-   [Messages Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363195.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
