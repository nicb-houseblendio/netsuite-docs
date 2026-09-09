---
id: "section_N640579"
type: "section"
title: "Including Custom Fields in Global Search"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Global Search > Including Custom Fields in Global Search"
parent: "article_8124535945"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N640579.html"
anchors: []
sha256: "b5a17e33201cd7f9a1421db1c73338813b8ff3dcf490c07d671d5baaf38b2de2"
---

Global searches usually return only record name and ID fields, but some custom values can be included too.

Settings for custom records and custom fields are configured separately, so you can disable global search for a custom record but allow it for a custom field.

Custom field types that can be indexed for global search are:

-   CRM
    
-   Entity
    
-   Item
    
-   Transaction Body
    

To include a custom field type in global search, a user with permission to edit or create custom fields must check the **Available for Global Search** box on the custom field configuration record. By default, this box isn't checked for new custom fields.

Global search indexing is available for the following data types, when the **Store Value** box is checked:

-   Currency
    
-   Decimal Number
    
-   Email Address
    
-   Free-Form Text
    
-   Help
    
-   Hyperlink
    
-   Inline HTML
    
-   Integer Number
    
-   Percent
    
-   Phone Number
    
-   Text Area
    

If your search results include more than one record type, they show a Custom Fields column listing the custom field name and value for each match.

If your results include a single record type, they don't show the columns for custom fields by default. Therefore, you may not see matching custom field values on the results page.

For more information about custom fields, see [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html).

Warning:

You can't index a custom field for global search if None is selected for any Level for Search/Reporting option on the **Access** subtab of the custom field record.

### Related Topics

-   [Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_8124535945.html)
-   [Global Search Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161899349589.html)
-   [How to Use Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0713121656.html)
-   [Tips for Effective Global Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N637092.html)
-   [Global Search Prefixes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N639669.html)
-   [Inline Editing of Global Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N641270.html)
-   [User Preferences for Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N642323.html)
-   [Using Global Search to Find Help Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N639669.html#bridgehead_4615925459)
-   [Notes about Global Search Auto Suggest](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N642700.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
