---
id: "section_N2828059"
type: "section"
title: "Creating Custom Transaction Body Fields"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Creating a Custom Field > Creating Custom Fields by Type > Creating Custom Transaction Body Fields"
parent: "section_161732113352"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828059.html"
anchors: ["procedure_N2828141"]
sha256: "446b1ca04001deb6830bb127d5841fa96396d54523698351d3f40e44921b6c61"
---

Custom transaction body fields let you add information specific to your business needs to the body of transaction records.

These records include:

-   purchase transactions
    
-   sales transactions
    
-   revenue arrangements
    
-   opportunities
    
-   journal entries
    
-   expense reports
    
-   transfer orders
    
-   item receipts
    
-   item fulfillments
    
-   fulfillment requests
    
-   store pickup fulfillments
    
-   inventory adjustments
    
-   work orders / assembly builds
    
-   customer payments
    
-   vendor payments
    
-   vendor prepayments
    
-   deposits
    
-   deposit applications
    
-   pay checks
    
-   other transaction types
    

You can also display custom transaction body fields on your web store transaction's checkout page. If you do this, the fields are automatically added to the body of sales transaction records.

#### To create or modify custom transaction body fields: {#procedure_N2828141}

1.  Go to _Customization > Lists, Records, & Fields > Transaction Body Fields_.
    
2.  The Custom Transaction Body Fields page lists each custom field, with details about the field and the records that use it.
    
3.  Choose an option:
    
    -   To edit an existing custom transaction body field, click the field name in the Description column and then modify the definition as needed.
        
    -   To add a new custom transaction body field, click **New**.
        
    
    For more information, see [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html).
    
4.  Fill in the required fields on the Transaction Body Field page, and then click **Save**.
    

Note:

You can also index custom transaction body fields for global search. Check the Global Search box on the record to include it in global searches. You can't index a custom field for global search if None is selected for any **Level for Search/Reporting** option on the Access subtab of the custom field record. For more information, see [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html) and [Including Custom Fields in Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N640579.html).

You can use SuiteCloud Development Framework (SDF) to manage custom transaction body fields as part of file-based customization projects. For information about SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html). The Copy to Account feature lets you copy a custom transaction body field to another one of your accounts. Each custom transaction body field page has a clickable Copy to Account option in the upper right corner. For information about Copy to Account, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).

The following screenshot shows the Custom Transaction Body Field page configured for a custom **Entered By:** field.

![Transaction Body Field page configured for a custom Entered By: field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CustTransBodyFieldSetup.png)

After it has been created, the custom transaction body field can be applied to a transaction form. The following screenshot shows the **Entered By:** field included on a Purchase Order form.

![Sample Purchase Order with custom Transaction Body field highlighted on the Custom subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CustTransBodyFieldDisplay.png)

If you set the Display Type to Hidden, the field is still included on all forms, but it won't be visible. The system ignores any changes you make to show or hide the field on all forms that apply to the custom transaction body field.

If the Log System Notes on Update Only preference is off, and you have the View access level to a custom transaction body field, its default value will show up in system notes fields when you create a transaction search. For more information, see [Searching System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N673560.html).

### Related Topics

-   [Custom Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827140.html)
-   [Creating Custom Fields by Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161732113352.html)
-   [Creating Custom CRM Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827328.html)
-   [Creating Custom Entity Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827562.html)
-   [Creating Custom Item Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827818.html)
-   [Creating Custom Transaction Line Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828307.html)
-   [Creating Custom Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828730.html)
-   [Creating Custom Item Number Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829121.html)
-   [Creating Other Record Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829304.html)
-   [Creating Other Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515582937.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
