---
id: "section_N2827562"
type: "section"
title: "Creating Custom Entity Fields"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Creating a Custom Field > Creating Custom Fields by Type > Creating Custom Entity Fields"
parent: "section_161732113352"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827562.html"
anchors: ["procedure_N2827651"]
sha256: "dfd3fa5be11ec7b395d6aeac52a690eaf7ff0c81a9d98daca3d4b35e4fc265a4"
---

Custom entity fields let you add information specific to your business needs to your entity records. You can add entity custom fields to existing and custom subtabs on entry forms used to enter entity records in your NetSuite account.

These records include the following relationship and employee records:

-   customer records
    
-   project records
    
-   vendor records
    
-   other name records
    
-   contact records
    
-   partner records
    
-   entity group records
    
-   employee records
    
-   website registration
    
-   generic resource
    

#### To create or modify custom entity fields: {#procedure_N2827651}

1.  Go to _Customization > Lists, Records, & Fields > Entity Fields_.
    
2.  On the Custom Entity Fields page, each custom field is listed, with columns providing detailed information about the field and which records the field has been applied to.
    
3.  Choose an option:
    
    -   To edit an existing custom entity field, click the field name in the Description column and then modify the field definition as needed.
        
    -   To add a new custom entity field, click **New**.
        
    
    For more information, see [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html).
    
4.  Fill in the required fields on the Custom Entity Field page and then click **Save**.
    

Note:

You can also index custom entity fields for global search. To include a custom field in global searches, check the Global Search box on its record. You can't index a custom field for global search if None is selected for any **Level for Search/Reporting** option on the Access subtab of the custom field record. For more information, see [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html) and [Including Custom Fields in Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N640579.html).

You can use SuiteCloud Development Framework (SDF) to manage custom entity fields as part of file-based customization projects. For information about SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html). You can use the Copy to Account feature to copy an individual custom entity field to another of your accounts. Each custom entity field page has a clickable Copy to Account option in the upper right corner. For information about Copy to Account, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).

Here is an example of a custom entity field.

![Custom Entity Field page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CustEntityFieldSetup.png)

When the custom Entity field is included on a form, it could look like the following example.

![Sample form with custom Entity field highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CustEntityFieldDisplay.png)

### Related Topics

-   [Custom Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827140.html)
-   [Creating Custom CRM Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827328.html)
-   [Creating Custom Item Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827818.html)
-   [Creating Custom Transaction Body Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828059.html)
-   [Creating Custom Transaction Line Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828307.html)
-   [Creating Custom Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828730.html)
-   [Creating Custom Item Number Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829121.html)
-   [Creating Other Record Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829304.html)
-   [Creating Other Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515582937.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
