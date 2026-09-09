---
id: "section_N362936"
type: "section"
title: "Location Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Classification Import Type > Location Import"
parent: "section_N360930"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N362936.html"
anchors: ["bridgehead_4086489213"]
sha256: "782784f44a6a204788fafe80997c5394abd250d717654c4259184cf6b5711e7f"
---

Locations can be used to categorize records according to geographic area. You can use the Import Assistant to set up and update location records in your NetSuite account.

Before you can import locations, an administrator, or another user with permission to enable features, must go to _Setup > Company > Enable Features_, and on the Company subtab, check the Locations box and click Save.

After you have imported location records successfully, you can review them at _Setup > Company > Locations_.

Note:

If you plan to import other record types that include fields referencing location values, complete the import of locations first.

Location body fields for which data can be imported include Name, External ID, Sublocation of (the parent location if any), whether the location is inactive, and a transaction prefix field you can use to make auto-generated transaction numbers independent per location. (Transaction prefix values can be up to 8 characters.) If you're using NetSuite OneWorld, the Subsidiary field is also available.

Important:

The location import supports the import of multiline sublists. When importing a file where the sublist data contains multiple lines for each sublist item, you should include an external ID for each location record to uniquely identify the record the sublist data belongs to. For more information, see [Multiline Sublists for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1493796058.html) and Import Format and Mapping Considerations in [Importing Sublist Data in a Single File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1493384282.html).

As of Version 2015 Release 2, fields formerly in the Address sublist for Location are mapped as body fields, and fields formerly in the Return Address sublist are structured as a subrecord. By default, the Address body field is read-only, and data from other related body fields is copied into it. If you map the Override body field and set it to Yes (meaning true), you can import data for the Address body field. Similarly, the Address field in the Return Address subrecord is read-only, and data from other related subrecord fields is copied into it. If you map the Override subrecord field and set it to Yes (meaning true), you can import data for the Address subrecord field.

## Supported Location Sublist Imports {#bridgehead_4086489213}

The Location import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Translation | When the Multi-Language feature is enabled. You can map multiple instances of this sublist to import translations for multiple languages. Selectively updatable based on the Language key field. |
| Business Hours | You can map multiple instances of this sublist to import more than one set of business hours. For information about setting up business hours, see [Defining Store Business Hours](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4817104906.html#bridgehead_4817113183). |

Every sublist on each record can optionally have a separate file. For imports that update existing Location records, handling of sublist data updates depends on the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

For more details about fields that can be mapped in the Location record, see the SOAP Schema Browser's [location](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/location.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Classification Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N360930.html)
-   [Class Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N362626.html)
-   [Custom Segment Value Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4358372117.html)
-   [Department Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N362786.html)
-   [Merchandise Hierarchy Node Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530005074.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
