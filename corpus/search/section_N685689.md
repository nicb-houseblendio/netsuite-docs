---
id: "section_N685689"
type: "section"
title: "Accessing a Saved Search"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Accessing a Saved Search"
parent: "chapter_N675442"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685689.html"
anchors: []
sha256: "f07772b511c19bc1d980a096cd7f3634eedc8a2010692b15c4c523c7505dc72b"
---

Note:

You can use SuiteAnalytics Workbook to query your NetSuite data with the analytics data source, which gives you advanced query options. For more on SuiteAnalytics Workbook and how to recreate your saved searches as workbooks, see the following topics:

-   [Getting Started with SuiteAnalytics Workbook](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158874665729.html)
    
-   [Analytics Data Source Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543418431.html)
    

To find a saved search:

-   Verify if the saved search has its own menu option at Reports > Saved Searches, and click on it, if available.
    
-   If you know part of the search title, use Global Search to find it. Enter **se:<search\_title\_text>** as keywords in the Search field in the upper right corner.
    
-   If you do not know the search title, you can display a list of all saved searches at:
    
    -   Transactions > Management > Saved Searches
        
    -   Lists > Search > Saved Searches
        
    -   Reports > Saved Searches > All Saved Searches
        
    
    You can click links to edit a saved search or view its results. If the list is lengthy, you can use available options to filter the list, review characteristics of searches, and find the search you need. See [Using the Saved Searches List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N687459.html).
    

You can run a saved search and view its results if:

-   The saved search is public, or
    
-   You have been defined as part of the saved search audience, either by name or based on your assigned role, department, subsidiary, or group.
    

Note:

When you run a saved search with the Advanced Employee Permissions feature enabled some fields are hidden depending on what your role has access to. Additionally, if you do not have access to a field used in a saved search criteria filter, the search results will not consider the criteria filter. Please contact your administrator to change what you are permitted to view. For more information about this feature, see [Advanced Employee Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1494536002.html).

You can edit a saved search if:

-   The saved search has been marked as Allow Audience to Edit,
    
-   You are the owner, or
    
-   You are an account administrator.
    

You also need general search permissions, and permissions for specific record types, to access saved searches. For information about general permissions required to access saved searches, see [Permissions for Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N664557.html).

Note:

Account administrators have greater access than other users to saved searches. For information, see [Administrator Access to Other Users' Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N687899.html).

After you have accessed a saved search page by clicking a menu link or **Edit** on a saved searches list page, you can:

-   Make changes to search definitions on any of the header check boxes or subtabs.
    
-   Click the **Preview** button to run the saved search and view its results.
    
-   Click the **New Template** button to create an advanced PDF/HTML template for printing the saved search results. For more information, see [Advanced Templates for Printing Saved Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4823423235.html)
    
-   Click the **Reset** button to clear any changes you have made.
    
-   Click the **New** button to open a page where you can create a new saved search for the same record type.
    
-   Click the **Change ID** button to open a page where you can enter a new script ID for the saved search.
    

If you are the saved search's owner, or the Allow Audience to Edit box has been checked, you can:

-   Click the **Save** button to resave the search with the same name.
    
-   Click the **Save & Run** button to resave the search with the same name and immediately run it to view results.
    
-   Click the **Save As** button to save the search with a different name.
    
-   Click the **Delete** button to remove the saved search from the system.
    
-   Additionally, if you have also the Publish Search permission, you can click the **Save & Email** button to resave the search with the same name and email the results to the recipients designated on the **Email, Recipients from Results** or **Email, Specific Recipients** subtabs.
    
    The results that are emailed to each recipient depend on the filters set up for the search, and the subtab on which the recipients are selected:
    
    -   If the recipients are selected on the Recipients from Results subtab, a single email with a summary of the results for each users' records is sent.
        
    -   If the recipients are selected on the Specific Recipients subtab, a single email with a summary of the results is sent to each recipient unless there is a **\-Mine-** filter set up on the Criteria subtab for any Entity fields. If this type of filter exists, each recipient is sent a summary of the results for their records only. In this scenario however, the results for all potential recipients are processed before the filter is considered, which can cause the data to exceed the size limit of 5MB or 10,000 rows. In such cases, the email that is sent might only contain some of the results and a truncation message, indicating that the results are incomplete.
        

If you are not the saved search's owner, and the Allow Audience to Edit box has not been checked, you can click the **Save As** button to save the search with a different name.

### Related Topics

-   [Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N675442.html)
-   [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html)
-   [Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680983.html)
-   [Audit Trail for Saved Searches, Reports and Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688127.html)
-   [Translations for Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688780.html)
-   [Displaying Saved Search Results on Your Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N689267.html)
-   [Persisting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1029112142.html)
-   [Saved Search Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
