---
id: "section_N2903330"
type: "section"
title: "Using SuiteScript with NetSuite Records"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Overview > Using SuiteScript with NetSuite Records"
parent: "article_163726005075"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2903330.html"
anchors: []
sha256: "53127156dd99615d089b9acead17c3c1302a5472e6c0e0c21552d2ea7186fb75"
---

NetSuite records have four main parts: body fields, buttons and actions, subtabs, and sublists. The following figure shows a standard sales order record with each of the basic components indicated.

![Basic components of a record with the body fields, buttons and actions, subtabs, and sublists called out.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptOverview/RecordComponents.png)

The basic components of the record are:

1.  Record object
    
2.  Body fields
    
3.  Buttons and actions
    
4.  Subtabs
    
5.  Sublists
    

You can use SuiteScript to create each basic component and to get and set values on the components. The following table describes the basic components.

| Record Component | Corresponding SuiteScript 2.x Module |
| --- | --- |
| Record object | [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html) - interact with the entire record object. |
| Body fields | [N/currentRecord Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4625600928.html) - interact with the body fields on the main area of the record or on a subtab. |
| Buttons and actions | You can't use SuiteScript on built-in buttons, but you can create a custom button using these two modules: [N/ui/serverWidget Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4321345532.html) - add a new button object to a page. [N/action Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1510761537.html) - perform business logic to update the state of records in view mode. |
| Subtabs | [N/ui/serverWidget Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4321345532.html) - programmatically add fields to a NetSuite tab or add custom subtabs. |
| Sublists | [N/ui/serverWidget Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4321345532.html) - interact with 'line item' sublist fields. |

For more information about NetSuite records, see [Working with Records, Transactions, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N488023.html). For more information about using SuiteScript to interact with NetSuite records, see [SuiteScript Records Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_1494659042.html).

### Related Topics

-   [SuiteScript 1.0 to SuiteScript 2.1 API Map](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4752722762.html)
-   [SuiteScript 2.1 API Introduction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4387172221.html)
-   [SuiteScript Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163726005075.html)
-   [What You Can Do with the SuiteScript API](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2902985.html)
-   [SuiteScript Script Type and Execution Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158379074356.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
