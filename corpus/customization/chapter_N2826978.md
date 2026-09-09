---
id: "chapter_N2826978"
type: "chapter"
title: "Custom Fields"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields"
parent: "book_N2823893"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2826978.html"
anchors: ["kaltura_player_265"]
sha256: "111bc2e752cc31528ff6159cdcd4b1ec18e4b28c6625a2029e1a3c8ecca91e18"
---

Custom fields let you add information specific to your business needs to records and transactions. You can create custom fields for records or transactions. Record custom fields can be added to existing and custom subtabs on the entry forms you use to enter records in your NetSuite account. Transaction custom fields can be added to the top (body) or the line items (columns) of transactions. Custom fields are based on standard fields and field types. For more information about custom field types, see the following:

-   [Field Type Descriptions for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2842731.html)
    
-   [Custom Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827140.html)
    
-   [Available Standard Fields and Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2843906.html)
    

Important:

SuiteScript doesn't support direct access to the NetSuite UI through the Document Object Model (DOM). You should access the NetSuite UI only by using SuiteScript APIs. For information about using SuiteScript APIs to customize the UI, see [SuiteScript 2.1 Custom Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1518456405.html).

The following table lists required steps you must follow to create a custom field:

| Required Steps | Related Help Topics |
| --- | --- |
| Set the basic properties for the field | [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html) |
| Assign the field to forms, as needed | [Assigning Custom Fields to Specific Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830027.html) |
| Set the display properties for the field | [Setting Display Options for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830238.html) |
| Set up validation and defaulting, and create dynamic defaults and hyperlinks if needed | 
-   [Setting Validation and Defaulting Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830711.html)
-   [Dynamic Defaults and Dynamic Hyperlinks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832010.html)

 |
| Set any sourcing criteria needed for the field | [Setting Sourcing Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2839623.html) |
| Set any access restrictions to the field based on department, role, or subsidiary | 

-   [Restricting Access to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2841053.html)
-   [Restricting Access to Employee Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1514478336.html)

 |
| Set any filtering criteria needed for the field | [Setting Filtering Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2840153.html) |

Here are some optional tasks you can do when creating a custom field:

| Optional Tasks | Related Help Topics |
| --- | --- |
| Filter dropdown list field options | [Dependent Dropdown Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2840468.html) |
| Make a field read-only | [Creating Read-Only Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2842596.html) |
| Add field-level help for a custom field | [Adding Field-Level Help for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_164519258566.html) |
| Translate the field label and help text | [Adding Translations for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4308565496.html) |
| Add a custom transaction field to a custom transaction form | [Adding Custom Fields to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828541.html) |
| Add a formula to a field | [Creating Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832369.html) |
| Create a custom list | [Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852109.html) |
| Change a custom field's type | [Converting the Field Type of a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_160640754252.html) |
| Track changes to a custom field | [Tracking Changes to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_54095541974.html) |
| Inactivate a custom field | [Inactivating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4352401817.html) |
| Create custom fields from summary search results | [Creating Custom Fields with Values Derived from Summary Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3746191995.html) |
| Maintain saved searches with edited custom fields | [Maintaining Saved Searches that Include Edited Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1122060904.html) |

For step-by-step instructions about creating and editing custom fields, see the following:

-   [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html)
    
-   [Inactivating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4352401817.html)
    
-   [Editing a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314473404.html)
    
-   [Advanced Features for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4388569541.html)
    
-   [Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852109.html)
    

Warning:

Be aware of what happens when you delete a custom field. When you delete a field, instances of the field are removed from forms and lists, and all related data is deleted. Reports and searches with the deleted field may remove the field or error out, depending on how the field is used. If you inactivate the field, the data remains in NetSuite. Changing the field's data type or permissions can cause errors in reports and searches that use it. For information about deleting a custom field, see [Buttons and Menus in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180852421.html).

Custom fields work with SuiteCloud Development Framework (SDF). SDF is a development framework for creating SuiteApps or customizing NetSuite accounts using a local integrated development environment (IDE). SuiteCloud projects are file-based and use XML definitions of custom NetSuite objects. For more information, see [SDF Custom Object and File Development in SuiteCloud Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4715411907.html).

Watch this video for an overview of custom field setup options.

<a id="kaltura_player_265"></a>

To view a list of custom fields training videos, see [Custom Fields Videos](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0510123425.html).

### Related Topics

-   [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N2823893.html)
-   [Customization Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2824008.html)
-   [Customization Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163039950342.html)
-   [Customizing Field Level Help for Standard Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1530729846.html)
-   [Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2852749.html)
-   [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html)
-   [Advanced Templates Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SBADVTemplates.html)
-   [Basic Printing Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453552264.html)
-   [Custom Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2875173.html)
-   [Custom Transactions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4172599049.html)
-   [Custom Segments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4313464438.html)
-   [Custom Centers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2890160.html)
-   [Deploying Upgraded Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2894013.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
