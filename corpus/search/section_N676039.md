---
id: "section_N676039"
type: "section"
title: "Defining a Saved Search"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Defining a Saved Search"
parent: "chapter_N675442"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html"
anchors: ["procedure_N676115", "procedure_N676064"]
sha256: "854e047748efc43cc4559be45f0e18d90b42dc075217d59bfa8cfe9c77b16a6f"
---

Note:

You can use SuiteAnalytics Workbook to query your NetSuite data with the analytics data source, which gives you advanced query options. For more on SuiteAnalytics Workbook and how to recreate your saved searches as workbooks, see the following topics:

-   [Getting Started with SuiteAnalytics Workbook](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158874665729.html)
    
-   [Analytics Data Source Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543418431.html)
    

To create a saved search, go to a saved search definition page for your chosen record type. You can access a saved search definition page in any of the following ways:

-   Go to _Reports > Saved Searches > All Saved Searches > New_ and select the record type for the saved search.
    
-   On a simple or advanced search definition page, click **Create Saved Search**.
    
-   On a search results page, click **Save This Search**.
    
-   For an existing saved search, go to Reports > Saved Searches > All Saved Searches, and click Edit next to the saved search you want to redefine. The maximum number of saved searches available in the NetSuite navigation menu is 100.
    

#### To define a saved search: {#procedure_N676115}

1.  On a saved search definition page, enter a title for the saved search.
    
    Make the title short and meaningful, as it may appear in menu links, as a dashboard portlet header, or as a custom KPI name.
    
2.  If you're editing an existing saved search, you can use the **Owner** dropdown menu to change who owns it. By default, the creator is the owner.
    
    -   The **Owner** dropdown menu is available to administrators and, if the search is public or has an audience defined, to the owner.
        
    
    Warning:
    
    If you change the owner of a scheduled saved search to another user who has never previously scheduled a saved search, the search email is no longer sent at the scheduled time. To reinstate the scheduled email for this search, the new owner must log in with the appropriate role and resave the search.
    
3.  If you want the search to be available to all users, check the **Public** box. If not, you can define a more limited audience on the **Audience** subtab.
    
    -   The **Public** box and the **Audience** subtab are available only to administrators and to other users with at least Create level of the Publish Search permission, a Lists type permission.
        
    -   Making a saved search public lets all users run and view it, but only administrators and the search owner can edit it. To let audience members edit, check the **Allow Audience to Edit** box on the **Audience** subtab.
        
    -   To save or delete a public saved search, you need to have the Publish Search permission. This applies also to saved searches you own. For more information, see [Editing or Deleting a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679137.html).
        
    -   Customers, vendors, and most partners can't access saved searches, even public ones. If they do get access, they can run it only if they have permission to that record type, and they can see only their own records.
        
        Important:
        
        If your saved search has sensitive data, don't make it public. Use the fields on the **Audience** subtab to limit the audience.
        
4.  Check any of the following boxes, if you want search results to be available as views for list pages of the searched record type.
    
    -   **Available as List View**
        
    -   **Available as Dashboard View**
        
    -   **Available as Sublist View**
        
    
    To limit these views to certain users, leave these boxes blank and check the corresponding boxes on the **Roles** subtab. For more information, see [Using a Saved Search as a View](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679407.html).
    
5.  If you want to be able to link to search results from the Reminders portlet, check the **Available for Reminders** box. For more information, see [Creating Custom Reminders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N585781.html).
    
6.  If you want this search to be available in menus, check the **Show in Menu** box.
    
7.  On the **Criteria** subtab, define criteria to filter saved search records. These criteria can include dynamically calculated field values, including join fields; formulas containing SQL functions, as well as AND/OR expressions. For information, see:
    
    -   [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html)
        
    -   [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html)
        
    -   [Search Formula Examples and Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N662868.html)
        
    -   [Using Expressions in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N647582.html)
        
    -   [Related Records Fields Available for Advanced Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N651952.html)
        
    
    Note:
    
    To use a saved search as a custom KPI that displays results for multiple date ranges, don't define a date field as a filter on the **Criteria** subtab. For additional requirements for this type of custom KPI, see [Notes on Using Saved Searches as Custom KPIs](#procedure_N676064).
    
8.  On the **Results** subtab, define the display options for saved search results.
    
    -   In the subtab header you can set up the following options:
        
        -   **Sort By** - sets the sort order of results records or rows.
            
            Note:
            
            A saved search must include at least one sort order. If you don't specify a column in the **Sort By** field, the first column specified on the Columns subtab is used for sorting. For saved searches with large data sets, set **Sort By** to the same columns that you added on the **Results** subtab.
            
        -   **Output Type** - sets the overall format for the results page. The available options are **Normal**, **Report**, **Grid**, and **Graph**.
            
        -   **Show Totals** - displays a total line on the results page.
            
        -   **Run Unrestricted** - makes search results available to users who would normally be restricted from seeing the underlying records.
            
            Note:
            
            Users without the correct permissions will still be unable to view the search results. For more information, see [Permissions and Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3781107123.html).
            
            Important:
            
            The **Run Unrestricted** option isn't applied to time and expense searches by users that have roles with the **Restrict Time and Expenses** option enabled. Employees using a role with the Restrict Time and Expenses option enabled can't enter expense reports or time transactions on behalf of other employees and their reports and searches don't show any time or expense transactions entered by other employees. The Restrict Time and Expenses option for a role overrides the Run Unrestricted option for a search.
            
        -   **Disallow Drill Down** - prevents users of unrestricted search results from drilling down to more detailed data.
            
        -   **Max Results** - limits the number of records displayed in results.
            
        -   **My Preferred Search Results** - applies search settings to quick search results pages. For more information, see [Defining a Saved Search as Preferred Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679861.html).
            
    -   On the **Columns** sublist you can set up the following options:
        
        -   Order of the columns.
            
        -   Fields or formula calculations to be displayed as columns on the search results page, including:
            
            -   Custom labels for one or more fields.
                
            -   Summary types to group one or more fields' values (including group, sum, count, min, max, and average).
                
            -   Functions to be applied to one or more fields' values.
                
    -   On the **Drill Down Fields** sublist you can set up the following options:
        
        Note:
        
        This sublist is available only if you have the Presentation Categories permission, a Lists type permission. You don't have to be an administrator.
        
        -   Fields, including join fields, to be displayed when a viewer of search results drills down on a record.
            
        -   The order in which drill down fields are displayed.
            
        -   Custom labels for displayed drill down fields
            
    
    For more information, see [Search Results Display Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648053.html).
    
9.  On the **Highlighting** subtab, you can set up visuals to draw attention to selected individual or aggregated results. Highlighting options include images, colored text, background colors, and bold text. For information, see:
    
    -   [Highlighting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678573.html)
        
    -   [Adding a Legend to Highlighted Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678573.html#bridgehead_160987057592)
        
10.  On the **Available Filters** subtab, define fields or formulas to show as filters on the results pages. For information, see [Selecting Available Filters for Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678025.html).
     
     Note:
     
     To use a saved search as a custom KPI that displays results for multiple date ranges, define a date field as an available filter. You don't need to check the **Show in Filter Region** box. For additional requirements for this type of custom KPI, see [Notes on Using Saved Searches as Custom KPIs](#procedure_N676064).
     
11.  On the **Audience** subtab, define the users who can run the saved search and view its results, and whether they can edit its definitions. For information, see [Defining Audiences for Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678294.html).
     
     Note:
     
     The **Audience** subtab is available only if you have at least the Create level of the Publish Search permission.
     
12.  On the **Roles** subtab, define the users who will see search results as their view of the selected record type, in lists, sublists, dashboard list portlets, forms, and quick search results. For information, see [Using a Saved Search as a View](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679407.html) and [Defining a Saved Search as a Preferred Search Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680007.html).
     
     Note:
     
     The **Roles** subtab is available only if you have at least the Create level of the Publish Search permission.
     
13.  On the **Email** subtab, you can send search results email, as alerts triggered by record changes, according to a schedule, or both.
     
     -   Check the **Send Alerts When Records are Created/Updated** box to send email alert messages when saved search results are added or updated, and then define recipients for alerts. For information, see [Enabling Saved Search Email Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681962.html).
         
     -   You can make alerts available to users other than defined recipients by checking the **Public and Allow Users to Subscribe** boxes. Then users can go to _Home > Set Preferences_ and elect to receive alerts. For information, see [Setting User Preferences to Receive Saved Search Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N682720.html).
         
     -   Check the **Send Emails According to Schedule** box to set up the search to be run on a certain date or interval, with results emailed to yourself, other users, or both. For information, see [Enabling Saved Search Scheduled Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N681274.html). Scheduling is a good option for saved searches that take a long time to run.
         
     
     For more information, see [Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680983.html).
     
     Note:
     
     The **Email** subtab is available only if you have at least the Create level of the Publish Search permission.
     
14.  After you've finished setting up your search, you can:
     
     -   Click **Preview** to see search results without saving the search definitions.
         
     -   Click **Save** to save your search and let you and other audience members run it.
         
         -   Click **Save & Run** to save the search and see the results.
             
         -   Click **Save & Email** to save the search and email results to your chosen recipients. You set this up in the **Email** subtab, on the **Specific Recipients** sublist.
             
             Note:
             
             This option is available only if you have the Publish Search permission assigned to your role.
             

For information about viewing saved search results, see [Displaying Saved Search Results on Your Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N689267.html).

## Notes on Using Saved Searches as Custom KPIs {#procedure_N676064}

For a saved search to be used as a custom KPI with results for multiple date ranges in the KPI portlet, scorecard, a trend graph, or meter, your search must:

-   Not include any date fields defined as filters on the **Criteria** subtab.
    
-   Have only field with a summary type (such as group, sum, or count) defined on the **Results** subtab.
    
-   Have a date field defined as an available filter on the **Available Filters** subtab.
    
    For more information, see [Custom KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609047.html).
    

### Related Topics

-   [Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N675442.html)
-   [Saved Search Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680983.html)
-   [Accessing a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685689.html)
-   [Audit Trail for Saved Searches, Reports and Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688127.html)
-   [Translations for Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688780.html)
-   [Displaying Saved Search Results on Your Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N689267.html)
-   [Persisting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1029112142.html)
-   [Saved Search Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
