---
id: "section_N2832010"
type: "section"
title: "Dynamic Defaults and Dynamic Hyperlinks"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Advanced Features for Custom Fields > Dynamic Defaults and Dynamic Hyperlinks"
parent: "section_4388569541"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832010.html"
anchors: []
sha256: "e2ff97b637d3412e7ee1b89908f7387e24b0062ffe0f0d3a435bbf2883549b21"
---

When working with free-form text, text area, rich text or hypertext fields, in the Default Value field on the Validation & Defaulting subtab, you can include NetSuite tags in the default definition. NetSuite tags are populated with field values when the page is loaded or saved.

Dynamic defaults can be used in the hyperlink fields to include information from the record or the current session in the URL for the website.

To include NetSuite tags in the default definition of a field, enclose each tag within curly braces, defining field tags in a dynamic default as **{tag}**, where **tag** is the ID of the field. Each field in NetSuite has a unique ID and therefore a unique tag definition.

Note:

Because field IDs are incorporated into tag definitions for fields, when creating custom fields, enter meaningful IDs for each custom field and use consistent naming conventions that meet your business needs. The default NetSuite IDs are meaningless, and in your dynamic defaults it'll be difficult to know exactly what the field references.

Dynamic defaults are evaluated, and each NetSuite tag is substituted on page load and page save. However, if you check the **Store Value** box, the tag substitution values are saved when the page is created as a true default. The default value is saved and doesn't dynamically change when page fields on the page change. This lets you create a dynamic default that retains its initial value. If you leave the default empty on the initial creation, it remains empty on the next edit. The default value doesn't effect previously saved records. The field must be edited manually or updated with custom code to change its initial value.

Important:

If you need to ensure that NetSuite tags defined in a dynamic default are substituted on each page load and save, clear the **Store Value** box.

See the following topics:

-   [NetSuite Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832058.html)
    
-   [Dynamic Hyperlinks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832147.html)
    
-   [Setting the Store Value Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1487762215.html)
    
-   [Setting the Formula Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1487762294.html)
    
-   [Predefined Formula Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_160492514847.html)
    

### Related Topics

-   [Advanced Features for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4388569541.html)
-   [Encrypted Custom Field Stored Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3908498467.html)
-   [Creating Custom Fields with Values Derived from Summary Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3746191995.html)
-   [Creating Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832369.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
