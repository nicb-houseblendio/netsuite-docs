---
id: "section_N3733259"
type: "section"
title: "Support Case"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Support > Support Case"
parent: "chapter_N3732579"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3733259.html"
anchors: ["bridgehead_N3733300", "bridgehead_N3733574", "bridgehead_N3733611", "bridgehead_N3733619", "bridgehead_N3734621", "bridgehead_N3734633"]
sha256: "5ac531f4bb825d1912fdad171e4fc3d299b8d2bdf78d0a03fb472af3bebdc8c4"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Support Case](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_91142453659.html).

Support Cases are support issues logged for a specific company.

The SupportCase record is defined in the [listSupport (support)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/support.xsd) XSD.

For details about using case records in the user interface, see [Setting Up Case Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2421072.html).

## Supported Operations {#bridgehead_N3733300}

The following operations can be used with the support case record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

Note:

The getDeleted operation is NOT supported for Cases.

## Field Definitions {#bridgehead_N3733574}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [support case](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/supportcase.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3733611}

## Case Status and Priority Internal IDs {#bridgehead_N3733619}

The following table lists the internal IDs for all standard Case Status and Priority values that can be used to populate the status and priority fields.

The status and priority values can be deleted or recreated so that the following internal ID values may differ for your organization. If the Show Internal IDs preference is enabled, you can confirm the internal ID values in the associated list. See [Setting the Show Internal IDs Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3420345.html).

| Case Statuses |  | Case Priorities |
| --- | --- | --- |
| ID | Status |  | ID | Priority |
| --- | --- | --- | --- | --- |
| 1 | Not Started |  | 1 | High |
| 2 | In Progress |  | 2 | Medium |
| 3 | Escalated |  | 3 | Low |
| 4 | Re-Opened |  | \- | \- |
| 5 | Closed |  | \- | \- |

## Working with Support Case Sublists {#bridgehead_N3734621}

The SOAP Schema Browser includes all sublists associated with the support case record. See the following information for usage notes regarding specific support case sublists. Usage notes are not provided for every sublist type.

## EmailEmployeesList {#bridgehead_N3734633}

Use this list to provide a list of employees that should be copied when the record is updated. Values submitted in this list are not saved in the NetSuite database.

### Related Topics

-   [Support](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3732579.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
