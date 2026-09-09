---
id: "section_N2852278"
type: "section"
title: "Creating a Custom List"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Custom Lists > Creating a Custom List"
parent: "section_N2852109"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852278.html"
anchors: ["procedure_N2852295"]
sha256: "e81a056cd12c683d524f19a6fb48e5dbf9689ced5199093513b0f547517f8bca"
---

A custom list is a list of values that you can use in custom fields on your forms and records. Custom lists enable you to set up predefined choices for your employees and customers to select when entering transactions and records. You can create an unlimited number of custom lists and an unlimited number of values for each list.

You can use CSV import to import large custom lists. For information, see [Custom List Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363830.html).

Important:

Custom lists can be used to set up options for matrix items. For details, see [Setting up an Item Matrix](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2228669.html).

#### To create a custom list: {#procedure_N2852295}

1.  Go to _Customization > Lists, Records, & Fields > Lists > New_. The Custom List page appears.
    
2.  In the **Name** field, enter a name for the list.
    
3.  In the ID field, enter a unique alphanumeric ID for the custom list. For information about best practices and naming conventions, see [Conventions for Naming Custom Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162428958352.html). For information about changing an existing ID, see [Changing the ID of a Custom Object](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162428789058.html).
    
4.  Select the owner of the custom list (default is you).
    
    Only the owner and users with edit or full permission levels can modify the custom list.
    
5.  Enter a description for the custom list.
    
6.  By default, values are listed in the order in which they're entered. To list values in alphabetical order, click the **alphabetical order** radio button.
    
7.  If the list is for matrix items, check the **Matrix Option List** box.
    
    If you check the box, an **Abbreviation** column is added to the **Values** list.
    
    Note:
    
    The Accounting Matrix Items feature must be enabled to use the matrix lists option. If it **isn't** enabled, the **Matrix Option List** box **isn't** displayed.
    
8.  In the **Value** field, enter a value for the list.
    
9.  Click **Add**.
    
10.  Add values to the list as needed.
     
11.  Click **Save**.
     

The custom list can now be used in your custom fields. For details, see [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html) and [Adding Translations for Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852517.html).

You can use SuiteCloud Development Framework (SDF) to manage custom lists as part of file-based customization projects. For information about SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html). You can use the Copy to Account feature to copy an individual custom list to another of your accounts. Each custom list page has a clickable Copy to Account option in the upper right corner. For information about Copy to Account, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).

Important:

Custom lists are intended for use with small, fixed, related sets of data. Custom lists should include no more than 1000 values.

### Related Topics

-   [Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852109.html)
-   [Adding Translations for Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852517.html)
-   [Managing Large Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4823380225.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
