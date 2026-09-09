---
id: "section_N2832369"
type: "section"
title: "Creating Formula Fields"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Advanced Features for Custom Fields > Creating Formula Fields"
parent: "section_4388569541"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832369.html"
anchors: []
sha256: "51112e456f8a38c35aff16847bee88a7c5b552d93531ef7a3d0a91e5e5e385b6"
---

In addition to defining a custom field that's populated with dynamic data as described in [Dynamic Defaults and Dynamic Hyperlinks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832010.html), you can define fields to be dynamically **calculated** based on the values returned in the dynamic fields.

To define formula fields, click the Validation & Defaulting subtab of the custom field. Check the Formula box. In the Formula field, use [NetSuite Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832058.html) to define the dynamically defaulted fields to be used in the calculation and use [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html) to define the formula.

![Validation & Defaulting subtab with Formula box checked.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/formula.png)

To dynamically recalculate a formula, clear the Store Value box, and if needed, use the NULLIF function in your formula to prevent division by zero.

Important:

The **Formula** box must be checked for the field to be processed as a formula. Also, as with any defaulted field, the **Store Value** box must be cleared to dynamically recalculate the value each time the field is viewed. Additionally, when a record is loaded, custom formula fields are calculated. However, if you change fields used in the formula definition while the record is loaded, the formula field won't recalculate until you reload the record.

Note:

If the formula field doesn't have the **Store Value** box checked, the field isn't available in search results, including lists based on saved searches.

If you have a use case for running a saved search on a formula field where the value isn't stored, there's an alternative solution available. For more information, see Running a Saved Search on a Formula Field Where the Value is Not Stored (SuiteAnswers ID: 1017388).

For more information about storing values, see [Setting the Store Value Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1487762215.html).

You might get these inline errors during validation:

-   ERROR: Field Not Found - returned when either a custom field or search formula isn't recognized.
    
    If you get a Field Not Found error, ensure that the user or role has the necessary access level in the **Default Level for Search/Reporting** list and permissions table. You can find these settings on the Access subtab of the custom field record.
    
-   ERROR: Invalid Formula - returned when there's a syntax or data type error in the custom formula field.
    

When custom formula fields appear in search results, they show the dynamically calculated value at the time of the search. You can also define search criteria as formula fields without using a custom formula field. For more information, see [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html).

Warning:

If a field on a record is referred to by a formula custom field, you can't edit the referenced field with inline editing.

Note:

Knowledge of SQL will help you to fully leverage the flexibility and power of SQL functions to define complex formulas, but the Formula popup window can help you to correctly define formula expressions. The popup includes a Function list that lets you select SQL functions to be included in expressions, and Filter or Field lists that let you to select field names and have their IDs included in expressions. For more details, refer to [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html). Also, you can refer to the SuiteScript Reference Guide for tables of NetSuite field IDs.

For additional information, see the following topics:

-   [Referencing Related Records in Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832533.html)
    
-   [Creating a Formula Field Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832724.html)
    
-   [Creating a Formula Field to Display Transaction Line Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832808.html)
    
-   [Using a Field Formula to Remove Extra Spaces After Date/Time Field Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4322174650.html)
    

### Related Topics

-   [Advanced Features for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4388569541.html)
-   [Referencing Related Records in Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832533.html)
-   [Creating a Formula Field Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832724.html)
-   [Creating a Formula Field to Display Transaction Line Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832808.html)
-   [Using a Field Formula to Remove Extra Spaces After Date/Time Field Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4322174650.html)
-   [Formulas with Various Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163612417610.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
