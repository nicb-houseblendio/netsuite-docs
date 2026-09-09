---
id: "section_N3772486"
type: "section"
title: "CRM Custom Field"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Customization > CRM Custom Field"
parent: "chapter_N3768661"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3772486.html"
anchors: ["bridgehead_N3772504", "bridgehead_N3772708", "bridgehead_N3772749", "bridgehead_N3772761"]
sha256: "a98bee9135c750f77ef5d168638f3848d2563c52d0188d873e6f8c78eee6bad0"
---

Custom CRM fields are fields that you can add to your CRM records to gather information specific to your business needs.

For information about working these fields in the UI, see [Creating Custom CRM Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827328.html).

The CRM custom field record is defined in the [setupCustom (customization)](https://webservices.netsuite.com/xsd/setup/v2025_2_0/customization.xsd) XSD.

## Supported Operations {#bridgehead_N3772504}

The following operations can be used with CRM custom field.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getCustomizationId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3493817.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3772708}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [CRM custom field](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/crmcustomfield.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Working with CRM Custom Fields Sublists {#bridgehead_N3772749}

The SOAP Schema Browser includes all sublists associated with the CRM custom fields record. See the following information for usage notes regarding specific CRM custom fields sublists. Usage notes are not provided for every sublist type.

## CrmCustomFieldFilter {#bridgehead_N3772761}

This list can only be populated when the type of custom field is set to List/Record.

### Related Topics

-   [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3768661.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
