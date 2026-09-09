---
id: "bridgehead_N495470"
type: "bridgehead"
title: "Additional Notes about Inline Editing"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Lists > Using Inline Editing > Additional Notes about Inline Editing"
parent: "section_N495192"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N495470.html"
anchors: ["bridgehead_N495546", "bridgehead_N495583", "bridgehead_N495616", "bridgehead_N495645", "bridgehead_43103529320"]
sha256: "d75ac2512d236ffa173f1eb948bf7b7f084e1c401bc7f40c4d8a8f08680cc28f"
---

See the following additional notes about using inline editing:

-   [Edit and Customize List Views](#bridgehead_N495546)
    
-   [Limitations for Inline Editing on Referenced Fields](#bridgehead_N495583)
    
-   [Additional Setup Option for Custom Search Portlets](#bridgehead_N495616)
    
-   [Allow Editing Option for Custom Records Is Unrelated](#bridgehead_N495645)
    
-   [Inline Editor Sublist Tooltip](#bridgehead_43103529320)
    

## Edit and Customize List Views {#bridgehead_N495546}

You can customize the list view to display certain fields from a record type on the list page. For more information, see [Customizing List Views](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N496170.html). Note that if the Use Expressions option is enabled for a search, inline editing is disabled in list, dashboard, and sublist views based on the search. If you want inline editing to be available for a view, ensure that the Use Expressions box on the Criteria subtab isn't checked for the search that filters view results. See [Using Expressions in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N647582.html).

## Limitations for Inline Editing on Referenced Fields {#bridgehead_N495583}

If a field on a record is referred to by a formula custom field, you can't edit the referenced field with inline editing. For more information about sourcing, see [Creating Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832369.html).

## Additional Setup Option for Custom Search Portlets {#bridgehead_N495616}

When the Inline Editing feature is enabled, editing is available by default for all search results in dashboard portlets. However, each Custom Search portlet has an Allow Edit setup option that you can use to enable or disable the Edit feature for specific portlets. See [Displaying Saved Search Results in Dashboard Portlets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N690632.html).

## Allow Editing Option for Custom Records Is Unrelated {#bridgehead_N495645}

Each custom record type created in NetSuite has an Allow Editing option that is different from the general editing that is available when the Inline Editing feature is enabled. When enabled, the custom record type option permits records of this type to be edited directly when they display in a sublist on a parent record. Enabling this option doesn't control whether records of this type can be edited inline in their own list pages and views. This option isn't related to the Inline Editing feature or to the Edit buttons that display on list pages when the feature is enabled.

## Inline Editor Sublist Tooltip {#bridgehead_43103529320}

When you're editing a sublist inline and you hover over a cell, the tooltip appears and shows the column name. If a sublist has many lines, you can view the column name when scrolling down the sublist.

You can enable or disable the tooltip by checking or clearing the **Sublist Column Name Tooltip** box which is located on the Appearance subtab at _Home > Set Preferences_.

![Inline Editor Sublist tooltip](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/WorkingWithRecords_SublistTooltip.png)

### Related Topics

-   [Using Inline Editing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495192.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
