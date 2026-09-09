---
id: "section_N3652149"
type: "section"
title: "Project Task"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Activities > Project Task"
parent: "chapter_N3650400"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3652149.html"
anchors: []
sha256: "fc23036e769244a1717be7f86b53a633d88b908d85ff7c4a4e45366b511632d3"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Project Task](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_68093010260.html).

The project task record can be used to keep track of specific activities and milestones associated with a project.

This record is defined in the [actSched (scheduling)](https://webservices.netsuite.com/xsd/activities/v2025_2_0/scheduling.xsd) XSD, where it is called _ProjectTask_.

The project task record is available when the Project Management feature is enabled at _Setup > Company > Enable Features_, on the Company subtab. When the feature is enabled, you can access the project task record in the UI by navigating to an existing project and clicking the New Project Task or New Milestone button. For details on working with this record in the UI, see [Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html).

Project task records cannot be created as standalone records. Rather, you create a project task for a specific project record, and the task remains attached to that record. For information about working with the project record in SOAP web services, see [Project (Job)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3645529.html).

For more on using SOAP web services to interact with the project task record, see the following:

-   [Project Tasks Versus Milestone Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3793231818.html)
    
-   [Project Task Supported Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3793222925.html)
    
-   [Project Task Field Definitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3793221576.html)
    
-   [Project Task Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3793220177.html)
    
-   [Adding a Project Task Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3790879161.html)
    
-   [Adding a Milestone Task Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3790879372.html)
    

### Related Topics

-   [Using Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html)
-   [Creating a Project Task Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1194983.html)
-   [Assigning Resources to Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1200642.html)
-   [Enabling Project Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4740572949.html)
-   [Activities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3650400.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
