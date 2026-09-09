---
id: "section_N2830027"
type: "section"
title: "Assigning Custom Fields to Specific Record Types"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Creating a Custom Field > Assigning Custom Fields to Specific Record Types"
parent: "section_N2829580"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830027.html"
anchors: ["procedure_N2830046"]
sha256: "1f8bd8504eb81e94995b9fe04c1bb8869a60936004291d1b6f3d42af8c665e44"
---

You can assign custom fields to display on specific record types. When you assign the field to a record type, it's automatically available as a possible field when creating a custom form for that record type. The field will also be available on all standard forms.

For custom entity fields, you must select the record types where the field is available. If you select a record type, the field automatically displays on all forms of that record type, including any custom forms. You can then edit custom forms to not show the new custom field.

Conversely, all custom transaction fields are automatically available in form customization, regardless of what you select on the **Applies To** subtab. For example, if you apply a custom transaction field to sales transaction forms, the field is also available when you customize purchase transaction forms.

For more information about available custom field types, see [Field Type Descriptions for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2842731.html).

#### To apply a custom field to a record type: {#procedure_N2830046}

1.  On the custom field setup page, click the **Applies To** subtab.
    
    ![Custom field Applies To subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CustomFieldAppliesToSubtab.jpg)
2.  Check the boxes to select the records you want the field to display on.
    
    Note the following:
    
    -   When a new transaction is created from a transaction that has a custom field value, the field value is copied to the new transaction.
        
    -   You can add record custom fields to existing and custom subtabs on the entry forms you use to enter records in your NetSuite account.
        
    -   You can add transaction custom fields to the top (body) or the line items (columns) of transactions. When adding a custom field to the body of a transaction, you apply the field to the type of transaction.
        
    -   When adding a custom field to the line items of a transaction, you apply the field to the type of line item.
        
    -   To apply a custom item field to a portion of the item, check the Select Individual Items box. Then in the Items field, hold down the Ctrl key and click each item that should have the custom field.
        
    -   To specify that the settings for a custom item field or custom transaction item option field also apply to its child items, check the Include Child Items box. Any child item fields added later will inherit the parent settings.
        
    -   When you have the Advanced Employee Permissions feature enabled and you select **Employee** from the **Applies To** subtab, an **Employee Access** subtab appears. From this subtab you can select the custom advanced employee permission you want to associate the custom field with. For more information, see [Advanced Employee Permissions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1513370474.html).
        
    -   You can set up the kit or assembly transaction line custom field to copy values from sales order items to fulfillment items. For more information, see [Apply to Kit or Assembly Components Setting for Custom Segments and Transaction Line Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161540199813.html).
        
    -   For custom item fields, there's a **Subtype** field with options to select **Both**, **Purchase**, or **Sale**. This selection applies the custom field to items available only for purchase, only for sale, or for both purchase and sale. Item subtypes apply only to non-inventory, service, and other charge item records
        
    -   For custom transaction body fields, if the Log System Notes on Update Only preference is off, and you have the View access level to a field, the default value of your custom transaction body field will show up in system notes fields when you create a transaction search. For more information, see [Searching System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N673560.html).
        
    
    You can't clear the **Applies To** box if the custom field is used for criteria in duplicate detection. If you try to do so, you'll receive an error message. For more information about duplicate detection, see [Setting Up Duplicate Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N258211.html).
    
3.  After you've defined a custom field to display on specific record types, you should define the display properties for that field. See [Setting Display Options for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830238.html).
    

Warning:

If you assign a custom field to a record type that's a child of another record, that custom field may not always show on the parent record forms. A child record may not be available on a form for a parent record that was created through transformation from another record type. For example, if you define a custom record as a child record of sales order, the custom child record isn't available on forms for sales orders transformed from quotes.

### Related Topics

-   [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html)
-   [Creating Custom Fields by Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161732113352.html)
-   [Assigning Custom Fields to Specific Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830027.html)
-   [Behavior of View from Order Only Settings on Transaction Line and Transaction Body Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0528113109.html)
-   [Setting Display Options for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830238.html)
-   [Setting Validation and Defaulting Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830711.html)
-   [Setting Sourcing Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2839623.html)
-   [Sourcing and Filtering Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2839994.html)
-   [Setting Filtering Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2840153.html)
-   [Dependent Dropdown Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2840468.html)
-   [Restricting Access to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2841053.html)
-   [Restricting Access to Employee Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1514478336.html)
-   [Creating Read-Only Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2842596.html)
-   [Adding Translations for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4308565496.html)
-   [Adding Custom Fields to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828541.html)
-   [Tracking Changes to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_54095541974.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
