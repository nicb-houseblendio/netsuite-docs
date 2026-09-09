---
id: "section_N688379"
type: "section"
title: "Audit Trail Search"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Audit Trail for Saved Searches, Reports and Schedules > Audit Trail Search"
parent: "section_N688127"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688379.html"
anchors: ["procedure_N688390"]
sha256: "c1cbd9d39a73075ecadc74ad8819dde44a08ec8de4ba32004484b45cf920100c"
---

Note:

By default, you are able to view audit trail records only for saved searches, reports, and report schedules that you own. To view audit trail records for saved searches, reports, and report schedules owned by other users, you need to have the Administrator role or the Unrestricted Analytics Audit Trail permission.

Analytics Audit Trail searches display audit trail data covering changes to all saved searches, custom reports, report schedules, and financial report layouts. For example, you can use this type of search to determine whether a saved search has been deleted.

#### To run an Analytics Audit Trail search: {#procedure_N688390}

1.  Go to _Reports > New Search_.
    
2.  Click **Analytics Audit Trail**.
    
3.  Use the **Record Type** list to specify the record types to be included in the search. You can specify any combination of the following record types:
    
    -   **Financial Layout** - Select this option to find the changes made to financial report layouts.
        
        Note:
        
        Formatting changes, such as font size or row color changes, are not logged in the audit trail.
        
    -   **Report** - Select this option to find the changes made to saved custom reports.
        
    -   **Report Schedule** - Select this option to find the changes made to report schedules.
        
    -   **Search** - Select this option to find the changes made to saved searches.
        
    
    If you are looking for specific changes, use the **Record Action** field.
    
    If you are looking for changes related to a specific search or report, you can specify its name in the **Record** field.
    
4.  To define your search further, you can also use the following fields:
    
    -   **Date** - If you are looking for changes during a specific time period, enter the time period.
        
    -   **From/To** - If you entered a time period to filter the search, enter the start and end dates for the period.
        
    -   **Component Name** - If you are looking for changes to a specific search or report component, enter the name of the component.
        
    -   **Component Type** - If you are looking for changes to search or report components of a specific type, enter this type.
        
    -   **Component Action** - If you are looking for a specific action that resulted in changes, enter this action.
        
    -   Use the **Old Value** and **New Value** fields to look for specific values before or after the change.
        
5.  When ready, click **Submit** to find the changes, or click **Create Saved Search** if you want to create a saved search based on your criteria.
    

### Related Topics

-   [Audit Trail for Saved Searches, Reports and Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688127.html)
-   [Audit Trail Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688186.html)
-   [Auditing Changes to Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688421.html)
-   [Auditing Saved Search Execution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688494.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
