---
id: "section_N3769505"
type: "section"
title: "Custom Record Type"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Customization > Custom Record Type"
parent: "chapter_N3768661"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3769505.html"
anchors: ["bridgehead_N3769526", "bridgehead_N3771401", "bridgehead_N3771438", "bridgehead_N3771526", "bridgehead_N3771545", "bridgehead_N3771564", "bridgehead_N3771583"]
sha256: "14e20bd3aab24fb8661cbcb876f8951dda7f7f55c64c00e94598718667a671d2"
---

For custom record types, fields on the body and subtabs (Numbering, Permissions, Links, and Managers) can be set on add or update of a new Custom Record Type. Fields on the Fields, Forms, Online Forms, Child Records, and Parent Records subtabs can only be set on update to an existing custom record.

For information about working with custom records types in the UI, see [Creating Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2876492.html).

The custom record type record is defined in the [setupCustom (customization)](https://webservices.netsuite.com/xsd/setup/v2025_2_0/customization.xsd) XSD.

## Supported Operations {#bridgehead_N3769526}

The following operations can be used with custom record types.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getCustomizationId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3493817.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3771401}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [custom record type](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customrecordtype.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Working with Custom Record Sublists {#bridgehead_N3771438}

The SOAP Schema Browser includes all sublists associated with the custom record record type. See the following information for usage notes regarding specific Custom Record sublists. Usage notes are not provided for every sublist type.

-   [CustomRecordTypeChildren](#bridgehead_N3771526)
    
-   [CustomRecordTypeForms](#bridgehead_N3771545)
    
-   [CustomRecordTypeOnlineForms](#bridgehead_N3771564)
    
-   [CustomRecordTypeParents](#bridgehead_N3771583)
    

## CustomRecordTypeChildren {#bridgehead_N3771526}

This is a **read-only** list that returns all custom records that define the current record as it's parent.

## CustomRecordTypeForms {#bridgehead_N3771545}

This is a **read-only** list that returns the forms that have been created for use with the current record type. A single default form is automatically created for any new record type.

## CustomRecordTypeOnlineForms {#bridgehead_N3771564}

This is a **read-only** list that returns all online forms that have been created for the current custom record type.

## CustomRecordTypeParents {#bridgehead_N3771583}

This is a read-only list that returns the parent records this record is a child of.

To have the entries set here active, you must set the _usePermission_ field to TRUE for the record type definition.

### Related Topics

-   [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3768661.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
