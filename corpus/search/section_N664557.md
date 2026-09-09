---
id: "section_N664557"
type: "section"
title: "Permissions for Searches"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Search Overview > Permissions for Searches"
parent: "chapter_N635877"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N664557.html"
anchors: []
sha256: "0025c1fc165191ad57292a7e37dec8457c6a78389a3fb0935a2394f9984dee97"
---

Note:

You can use SuiteAnalytics Workbook to query your NetSuite data with the analytics data source, which gives you advanced query options. For more information about SuiteAnalytics Workbook and how to turn your saved searches to workbooks, see the following topics:

-   [Getting Started with SuiteAnalytics Workbook](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158874665729.html)
    
-   [Analytics Data Source Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543418431.html)
    

Your NetSuite account administrator assigns roles to users. For each role, they set up permissions for viewing, editing, and searching specific record types.

You have one or more roles you can use to log in to NetSuite. The permissions and search access for your role decide which searches you can run. For saved searches, your role's permissions also decide the record types you can use for saved searches.

NetSuite has four types of permissions: Lists, Reports, Setup, and Transactions. Five Lists type permissions control what you can do with searches and saved searches, like running, exporting, emailing, and sharing them:

-   **Perform Search** - This permission has two levels, View and Full. With View, you can run searches and saved searches for the record types you have access to. With Full, you can also create and save searches.
    
-   **Publish Search** - This permission has four levels, View, Create, Edit, and Full. With Create level or higher, you can share saved searches, set up alert emails, and schedule emails of saved search results. The Audience, Roles, Email, and Execution Log subtabs are available on the saved search definition page.
    
-   **Persist Search** - This permission has one level only, Create. With it, you have a Persist (CSV) link for saved searches listed at _Reports > Saved Searches > All Saved Searches_. This permission lets you extend the timeout for saved searches to up to 3 hours and save results as a CSV file.
    
-   **Export Lists** - This permission has one level only, Create. With it, you get Export and Email buttons on your search and saved search results pages, so you can export and email searches and saved searches for the record types you can access. You need to have at least the View level for the Perform Search permission to activate this permission.
    
-   **Tableau® Workbooks Export** - This permission has one level only, Create. With it, you get the Export to Tableau Workbook button on search and saved search results pages, so you can export search results as analysis-ready Tableau® workbooks for the record types you can access. You need to have the Export Lists permission and at least the View level of the Perform Search permission to activate this permission.
    

The Create HTML Formulas in Search permission is a Setup permission that lets users use HTML code in saved searches with the Formula(HTML) fields. You need to enable the **HTML Formulas in Search** feature first to set up this permission. For more information, see [Evaluating Code in Saved Searches Using Formula(HTML) Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0403035152.html).

Additionally:

-   The following Transactions permission controls whether you can save a transaction search:
    
    **Find Transaction** - This permission has four levels, View, Create, Edit, and Full. With Create level or higher, you get the Create Saved Search button for transaction searches. With View, you can run transaction searches but not save them.
    
-   The following employee permissions control whether you can create a search or use global search:
    
    -   Perform Search
        
    -   Employee Record
        
-   The following address permission determines your ability to search all addresses:
    
    **Address List in Search** - Without this, you can only see your own address records
    

If you don't see the Email and Export buttons on your search and saved search results page, you may need a higher level of the Perform Search permission. This also applies if you have trouble running, exporting, or emailing searches, or creating, running, exporting, emailing, or viewing the log for saved searches. Contact your administrator to see if your assigned role, permissions, and search access require changes. For information about role permissions, see [NetSuite Permissions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N325094.html).

There's another level of access for saved searches created by other users. You can access a saved search created by another user if the search is public, or if you're listed as an audience member by name, role, department, subsidiary, or group.

Important:

When you create or customize roles that need to search for employees, ensure that they have the Perform Search, Employees, and Employee Search permissions.

Note:

Custom fields have additional field-level security for searches. You can set Search/Reporting access level on the custom field record. Access can be defined generally, or by role, department, or (in NetSuite OneWorld) subsidiary. The access levels are Edit (view and change the field), Run (view the field only), and None (no access). For more information, see [Restricting Access to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2841053.html).

### Related Topics

-   [Search Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N635877.html)
-   [Searchable Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N644265.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
