---
id: "section_N2829121"
type: "section"
title: "Creating Custom Item Number Fields"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Creating a Custom Field > Creating Custom Fields by Type > Creating Custom Item Number Fields"
parent: "section_161732113352"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829121.html"
anchors: ["procedure_0809091320"]
sha256: "859bb0cce3854bd66b0f658f84b3469634f2f5559e37a8a5b56d39ae1b140459"
---

Custom item number fields let you track item-specific information or workflows that are unique to your business on inventory records. For instance, you can track the status and results of quality control procedures specific to each serialized item or track recall information on lot records.

These records include:

-   serial numbered items - see [Serial Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230290.html)
    
-   lot numbered items - see [Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235684.html)
    
-   gift certificate items - see [Gift Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2244991.html)
    

Note:

To use custom item number fields, make sure at least one of the features in the preceding list is enabled.

#### To create a custom item number field {#procedure_0809091320}

1.  Go to _Customization > Lists, Records, & Fields > Item Number Fields_.
    
2.  The Custom Item Number Field page lists each custom field, showing details about the field and which records use it. Choose an option:
    
    -   To edit a custom item number field, click the field name in the Description column and then modify the field definition as needed.
        
    -   To add a new custom item number field, click **New**.
        
        For more information, see [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html).
        
3.  Fill in the required fields on the Item Number Field page, and then click **Save**.
    

When you create a lot numbered or serialized inventory item or edit an existing record, you can add the custom field to the item if it's not already applied to all items. On the item record, click the **Custom** subtab. In the **Inventory Number Options** field, press Ctrl and select all the item number fields you want to add to the item. Then click **Save**.

You can use SuiteCloud Development Framework (SDF) to manage custom item number fields as part of file-based customization projects. For information about SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html). The Copy to Account feature lets you copy a custom item number field to another one of your accounts. Each custom item number field page has a clickable Copy to Account option in the upper right corner. For information about Copy to Account, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).

Here is an example of a custom item number field.

![Item Number Field page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CustItemNumberFieldSetup.png)

When the custom item number field is included on a form, it could look like the following example.

![Sample form with custom item number field highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CustItemNumberFieldDisplay.png)

The custom item number field is found in the serial number record or lot number record of the inventory detail subrecord. To view the custom field, create a new transaction that uses the field. Enter an item and then click Inventory Detail. Select and open the details of a serial or lot number. The custom item number field appears on the Serial Number Record page, as shown in the preceding screenshot.

For more information, see [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html).

### Related Topics

-   [Custom Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827140.html)
-   [Creating Custom Fields by Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161732113352.html)
-   [Creating Custom CRM Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827328.html)
-   [Creating Custom Entity Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827562.html)
-   [Creating Custom Item Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827818.html)
-   [Creating Custom Transaction Body Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828059.html)
-   [Creating Custom Transaction Line Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828307.html)
-   [Creating Custom Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828730.html)
-   [Creating Other Record Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829304.html)
-   [Creating Other Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515582937.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
