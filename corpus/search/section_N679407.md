---
id: "section_N679407"
type: "section"
title: "Using a Saved Search as a View"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Defining a Saved Search > Using a Saved Search as a View"
parent: "section_N676039"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679407.html"
anchors: ["bridgehead_N679501"]
sha256: "f0184010a078fc91039b313159dab6cc7567afc81f438d03468301d624336381"
---

You can make a saved search available as a view for its audience, set it as the default view for that record type's lists, or both. The audience is set in the **Public** box and the **Audience** subtab.

A list view is a definition of the records and fields to be displayed on a list page for a record type. A sublist view is a definition of the records and fields to be displayed on a subtab list for a record type. A dashboard view is a definition of the records and fields to be displayed in the List portlet for a record type. These view definitions are based on saved searches, so you can reuse your search settings for all of them.

![Available as List View box](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/savedview1.png)

Important:

If the **Use Expressions** option is enabled for a search, inline editing is disabled in list, dashboard, and sublist views based on the search. If you want inline editing to be available for a view, ensure that the **Use Expressions** box on the **Criteria** subtab is not checked for the search that filters view results. See [Using Expressions in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N647582.html).

## Making a Saved Search Available for Views {#bridgehead_N679501}

Each saved search page has a set of **Available as View** check boxes in the header. Check one or more of these boxes to let the audience apply it to list views, sublist views, and dashboard list portlets of the selected record type.

-   If the **Available as List View** box is checked, users can select the saved search's title in the **View** dropdown list at the bottom of list pages of the selected record type, to display records and fields according to saved search definitions.
    
-   If the **Available as Sublist View** box is checked, users can select the saved search's title in the **View** dropdown list at the bottom of lists of the selected record type on subtabs.
    
-   If the **Available as Dashboard View** box is checked, users can select the saved search's title in the **View** dropdown list at the bottom of dashboard list portlets of the selected record type.
    

If a list, sublist, or dashboard List portlet doesn't have a **View** dropdown list, no saved searches are available for that record type. Don't use record type names in search titles.

In addition to the **View** dropdown list, users can click **Customize View** to create their own custom search to use as a custom view. See [Working with List Views, Sublist Views, and Dashboard Views](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495842.html).

Note:

Account administrators can prohibit users with a specific role from using saved searches as views, even if the **Available** boxes have been checked, by restricting that role to use of one list view, sublist view, or dashboard view only. This setting is on the **Searches** subtab of the Role record. See [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html).

### Related Topics

-   [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html)
-   [Selecting Available Filters for Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678025.html)
-   [Defining Audiences for Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678294.html)
-   [Highlighting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678573.html)
-   [Marking a Search Inactive](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4098463669.html)
-   [Editing or Deleting a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679137.html)
-   [Defining a Saved Search as Preferred Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679861.html)
-   [Defining a Saved Search as a Preferred Search Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680007.html)
-   [Using a Saved Search as a Reminder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680807.html)
-   [Using Saved Searches for Customer Center Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3842991795.html)
-   [Change of Sign for Expense Account Amounts in Transaction Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3891485192.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
