---
id: "section_N3645529"
type: "section"
title: "Project (Job)"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Entities > Project (Job)"
parent: "chapter_N3639664"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3645529.html"
anchors: ["bridgehead_N3645563", "bridgehead_N3645835", "bridgehead_3795870828"]
sha256: "519d045d331e6b243935ebe1ec7e40af023fb47403f537dabb48673d36ba34ee"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Job](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_83090456314.html).

You use the project record to manage company initiatives.

The project record is defined in the [listRel (relationships)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/relationships.xsd) XSD, where it is called _Job_.

To use the project record, you must have the Projects feature enabled at _Setup > Company > Enable Features_, on the Company subtab. If you plan to do advanced project tracking, you must also enable Project Management. If you do not see the Project Management box, your company must first purchase the Project Management add-on from NetSuite.

To access the project record in the UI, choose _Lists > Relationships > Projects_ (or Jobs). For help working with projects manually, see [Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3714107248.html).

For more on using SOAP web services to interact with projects, see the following:

-   [Adding a Project with a Status Example One](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3795306517.html)
    
-   [Adding Resources Example Two](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3795308162.html)
    

Important:

Starting with the 2008.2 version of NetSuite, the Job record was renamed to Project, but if you have existing code that references the Job record, this code will not break. The name change applies to external UI labels only. You should continue to reference the Job complex type in your code.

## Supported Operations {#bridgehead_N3645563}

The following operations can be used with the project record:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [searchMoreWithId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3523074.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3645835}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [project](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/job.html) reference page. For information about using this tool, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_3795870828}

When using SOAP web services, the behavior of the Resources sublist differs slightly from the behavior in the UI. Specifically, in the UI, each line must have a unique value in the Name field. Further, in the UI, you can select more than one role for each resource.

With SOAP web services, if you want to add a resource that has three different roles, you set up your code as if you are adding three sublist records for that resource - one for each role. The jobResource values are not required to be unique. To see an example, refer to [Adding Resources Example Two](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3795308162.html). Note that after you complete the add operation, the Resources sublist in the UI looks the same as it would if you had manually added one line for the resource, with multiple roles specified on that line, as shown in the illustration above.

### Related Topics

-   [Creating a Project Resource Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188929.html)
-   [Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3639664.html)
-   [Entity Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3650214.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
