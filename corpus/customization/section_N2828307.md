---
id: "section_N2828307"
type: "section"
title: "Creating Custom Transaction Line Fields"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Creating a Custom Field > Creating Custom Fields by Type > Creating Custom Transaction Line Fields"
parent: "section_161732113352"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828307.html"
anchors: ["procedure_N2828396", "bridgehead_4629019084"]
sha256: "0f9ced953de7743a666f76218c032fdfed889bf86d9976f677682e5a7477f564"
---

Custom transaction line fields let you add information specific to your business needs to the line items of your transaction records.

These records include:

-   expense items
    
-   purchase items
    
-   sale items
    
-   store items
    
-   revenue arrangements - available if Advanced Revenue Management is enabled
    
-   journal entries
    
-   expense reports
    
-   item receipts or fulfillments
    
-   opportunity items
    
-   time cards
    
-   inventory adjustment
    
-   inventory transfer
    
-   fulfillment requests
    
-   store pickup fulfillments
    
-   work orders
    
-   paycheck earnings
    
-   paycheck deductions
    
-   paycheck employee taxes
    
-   paycheck company taxes
    
-   paycheck company contributions
    

Note:

Additional options for custom transaction line fields include controls for displaying fields on printed forms (such as picking tickets or packing slips), grouping on invoices, storing with item groups, and applying to kit/assembly component lines. These options do not represent separate transaction types, but rather define display and storage behaviors for the custom field.

#### To create or modify custom transaction line fields: {#procedure_N2828396}

1.  Go to _Customization > Lists, Records, & Fields > Transaction Column Fields_.
    
2.  On the Custom Transaction Line Fields page, each custom field is listed, with columns providing detailed information about the field and which records the field has been applied to.
    
3.  Choose an option:
    
    -   To edit an existing custom Transaction Line field, click the field name in the Description column and then modify the field definition as needed.
        
    -   To add a new custom Transaction Line field, click **New**.
        
    
    For more information, see [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html).
    
4.  Fill in the required fields on the Transaction Line Field page, and then click **Save**.
    

You can use SuiteCloud Development Framework (SDF) to manage custom transaction line fields as part of file-based customization projects. For information about SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html). The Copy to Account feature lets you copy a custom transaction line field to another one of your accounts. Each custom transaction line field page has a clickable Copy to Account option in the upper right corner. For information about Copy to Account, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).

Here is an example of a custom transaction line field.

![Transaction Column Field page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CustTransColumnFieldSetup.png)

When the custom transaction line field is included in a form, it could look like the following example.

![Sample form with custom transaction line field highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CustTransColumnFieldDisplay.png)

If you set the Display Type to Hidden, the field is still included on all forms, but it won't be visible. Any changes you make to show or hide the field on forms won't affect the custom transaction line field.

## Check Box Type Limitation {#bridgehead_4629019084}

There's a limitation on custom transaction line fields when all of these conditions are met:

1.  Type = Check Box
    
2.  Store Value = checked
    
3.  Applies To = only Item Fulfillment is checked
    
4.  On the Validation & Defaulting subtab, Default Checked is checked
    
5.  Create a sales order and add at least one item
    
6.  Click Save & Fulfill
    

However, on the item fulfillment transaction, you'll notice the transaction line field isn't checked, even with the previous settings. This happens because NetSuite takes the custom field info from the sales order, and if the check box isn't applied, it defaults to the system value. To work around this, you can apply the field to sales orders and hide it on the sales order forms, if needed.

### Related Topics

-   [Custom Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827140.html)
-   [Creating Custom Fields by Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161732113352.html)
-   [Creating Custom CRM Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827328.html)
-   [Creating Custom Entity Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827562.html)
-   [Creating Custom Item Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827818.html)
-   [Creating Custom Transaction Body Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828059.html)
-   [Creating Custom Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828730.html)
-   [Creating Custom Item Number Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829121.html)
-   [Creating Other Record Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829304.html)
-   [Creating Other Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515582937.html)
-   [Apply to Kit or Assembly Components Setting for Custom Segments and Transaction Line Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161540199813.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
