---
id: "section_N2828730"
type: "section"
title: "Creating Custom Transaction Item Options"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Creating a Custom Field > Creating Custom Fields by Type > Creating Custom Transaction Item Options"
parent: "section_161732113352"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828730.html"
anchors: ["procedure_N2828793", "bridgehead_N2828869", "procedure_N2828881"]
sha256: "a4235a4a03815cb8654cd35a85d1a570213f9226768f7a2427ff75b719fb7c9c"
---

Transaction item options let you add information, specific to your business needs, to line items on transaction records.

Item options can be used to track item characteristics. For instance, you can use item options to record different colors of an item.

You can create item options for:

-   purchase items
    
-   sales items
    
-   opportunities
    
-   web store items
    
-   transfer orders
    
-   kits and assemblies
    

Note:

Be aware that too many characters in item option fields can cause performance issues. It's best to limit custom item option fields to 50, with a total character count of 4000 or fewer. Note that the total character count includes both field names and values.

#### To create or modify custom transaction item option fields: {#procedure_N2828793}

1.  Go to _Customization > Lists, Records, & Fields > Transaction Item Option_.
    
2.  On the Custom Transaction Item Option Fields page, each custom field is listed, with columns providing detailed information about the field and which records the field has been applied to.
    
3.  Choose an option:
    
    -   To edit an existing custom **Transaction Item Option** field, click the field name in the description column and then modify the field definition as needed.
        
    -   To add a new custom **Transaction Item Option** field, click **New**.
        
    
    For more information, see [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html).
    
4.  Fill in the required fields on the Item Option page and then click **Save**.
    

Note:

You can define a formula for an item option's default value (by checking the Formula box on the [Setting Validation and Defaulting Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830711.html)), but it can't reference non-item option fields. You may be able to save an item option successfully with a reference to a non-item option field. However, users will encounter errors when they try to save a line item with the item option selected.

## Offer your customers free promotional gift wrapping {#bridgehead_N2828869}

After you've enabled the Item Options feature, you can offer your customers complementary gift wrapping on select items as a promotion. With item options, create a Gift Wrapping check box on items so customers can indicate if they would like gift wrapping.

#### To create an item option for gift wrapping: {#procedure_N2828881}

1.  Go to _Customization > Lists, Records, & Fields > Transaction Item Options > New_ > New.
    
2.  In the **Label** field, enter the name of your option, **Gift Wrapping**.
    
3.  To create a check box field, in the **Type** field, select **Check Box**.
    
4.  On the **Applies To** subtab, check the **Sale** and **Web Store** boxes for the option to appear on sales transactions and in your website.
    
5.  In the **Items** field, select the individual items you want to offer gift wrapping for.
    
    You can select multiple items by holding down the Ctrl key as you select the items with the mouse.
    
6.  On the **Display** subtab, in the **Label for Input** field, enter the name for the option as it should appear to customers on your website.
    
7.  Click **Save**.
    

Now, you can offer customers complementary gift wrapping for items. The choice your customers make appears in the **Options** column of each sales transaction.

Here's an example of a custom transaction item option field.

![Custom Transacton Item Option page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CustTransItemFieldSetup.png)

When the custom transaction item option field is included on a form, it could look like the following example.

![Sample form with custom transacton item option field highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CustTransItemFieldDisplay.png)

### Related Topics

-   [Custom Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827140.html)
-   [Creating Custom Fields by Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161732113352.html)
-   [Creating Custom CRM Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827328.html)
-   [Creating Custom Entity Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827562.html)
-   [Creating Custom Item Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827818.html)
-   [Creating Custom Transaction Body Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828059.html)
-   [Creating Custom Transaction Line Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828307.html)
-   [Creating Custom Item Number Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829121.html)
-   [Creating Other Record Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829304.html)
-   [Creating Other Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515582937.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
