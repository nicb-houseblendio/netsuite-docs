---
id: "section_N2876492"
type: "section"
title: "Creating Custom Record Types"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Creating Custom Record Types"
parent: "chapter_N2875173"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2876492.html"
anchors: []
sha256: "bbdfbe6ec59dfaf8f8532be3f00eb961e32cc52d1707723ff75c6f6b06a7ec83"
---

Use custom record types to store business information that isn't represented by a standard NetSuite record type. Custom record types are useful when users need to create, search, report on, or manage business-specific records independently from standard NetSuite records.

For example, organizations commonly use custom record types to track assets, certifications, maintenance records, or other business-specific information.

To create a custom record type, perform the following steps:

1.  [Creating a New Custom Record Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501860307.html).
    
2.  [Entering Name and Display Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501860247.html).
    
3.  [Specifying Permission and UI Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501860092.html).
    
4.  [Configuring File and Child Record Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501859968.html).
    
5.  [Defining Search and Edit Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501859705.html).
    
6.  To create a custom record type, click **Save**.
    

Note:

To enable QuickViews for your custom record, use form customization for the custom record. For more information, see [Configuring QuickViews for Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_95152126340.html).

The following subtabs are available to help you further define your custom records before saving:

-   **Subtabs** - Create and arrange subtabs on your custom record type. For more information, see [Adding Subtabs to a Custom Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2877748.html).
    
    Note:
    
    To save time, create and arrange subtabs for your custom records before defining your custom fields.
    
-   **Sublists** - Add search results as sublists on your custom record type.
    
    For more information, see [Applying Custom Sublists to Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4453542165.html).
    
-   **Icon** - Select the PNG sprite you want to use to represent this record type in the New Bar, Create New menu, Recent Records menu, Recent Records portlet, and QuickViews. You can choose from built-in icons or create your own custom icon.
    
    For more information, see [Choosing an Icon for a Custom Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2881257.html).
    
-   **Numbering** - Specify the numbering format for the custom record types. For more information, see [Numbering Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2878042.html).
    
-   **Permissions** - Select the roles you want to access custom record entry forms, choose a default form, and restrict the forms available here. For information, see [Setting Permissions for a Custom Record Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2879388.html) and [Applying Role-Based Restrictions to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880594.html).
    

Important:

For these permissions to apply, you must select **Use Permission List** from the **Access Type** list.

-   **Links** - Create links that take you to the list of record entries for this custom record type and select where to place the links. For more information, see [Creating Links to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880942.html).
    
-   **Managers** - Define specific employees as managers of the current record type, which enables the employee to modify the custom record type. When defined as a manager, employees are automatically granted custom record view permission. The custom record view permission permits managers to see the list of custom record types but **not** drill down on them.
    

Note:

If an employee has a role that includes the Custom Record Type permission, they have edit access to **all** custom record types. The Managers subtab enables you to grant permission for an employee to the current record type only.

-   **Translation** - (when Multi-Language feature is enabled) Define translations for the custom record type name to be used when users change the language preference. For more information, see [Adding Translations for Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2882154.html).
    

After you save a custom record type, the following subtabs become available. You can continue customizing by adding fields, creating custom forms, configuring online forms, and defining parent-child relationships, depending on your business requirements.

-   **Fields** - Create and arrange the fields for your custom record type. For more information, see [Adding Fields to Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2878340.html).
    
-   **Forms** - Customize and select a preferred entry form for your custom record type. For more information, see [Adding Custom Forms for a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2878636.html).
    
-   **Online Forms** - Create and manage online forms for your custom record types. For more information, see [Adding Custom Online Forms for a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2879167.html).
    
-   **Child Records** - If this record type is a parent record, its child records are listed here.
    
-   **Parent Records** - If this record type is a child record, its parent records are listed here.
    
    For information about parent and child records, see [Parent-Child Record Relationships](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2885788.html), [Creating a Parent-Child Relationship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158229389859.html), and [Using Child Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2886136.html).
    

After saving a custom record type, administrators can use Advanced Record Customization (ARC) to review and manage supported record type configurations and overrides in a centralized location. For more information, see [Advanced Record Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2144345458.html).

You can use SuiteCloud Development Framework (SDF) to manage custom record types as part of file-based customization projects. For information about SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html). You can use the Copy to Account feature to copy an individual custom record type to another of your accounts. Each custom record type page has a clickable Copy to Account option in the upper right corner. For information about Copy to Account, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).

### Related Topics

-   [Custom Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2875173.html)
-   [Parent-Child Record Relationships](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2885788.html)
-   [Sourcing with Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2886428.html)
-   [Updating Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501860753.html)
-   [Using Custom Record Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2888872.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
