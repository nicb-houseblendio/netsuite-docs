---
id: "section_N688186"
type: "section"
title: "Audit Trail Subtab"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Audit Trail for Saved Searches, Reports and Schedules > Audit Trail Subtab"
parent: "section_N688127"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688186.html"
anchors: ["bridgehead_N688263", "bridgehead_N688275", "bridgehead_N688346"]
sha256: "f9e59839b5eb324ad6c14d782af69313a7d30ad38dafaf0ffd9ec12b013cf776"
---

Note:

By default, you are able to view audit trail records only for saved searches, reports, and report schedules that you own. To view audit trail records for saved searches, reports, and report schedules owned by other users, you need to have the Administrator role or the Unrestricted Analytics Audit Trail permission.

The Audit Trail Subtab lists all audited changes and actions for the respective Saved Search, Saved Report, or Report Schedule.

![Audit trail subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/audittrail1.png)

The default columns displayed are as follows:

-   Date: the date and time the change was made.
    
-   Set By: the user who made the change.
    
-   Component Action: the action taken (update, delete, or create).
    
-   Component Type: the type of page component that was edited.
    
-   Component Name: the name of the edited page component.
    

## Customizing the default Audit Trail View {#bridgehead_N688263}

Click Customize View to customize the default view for your specific needs. Additional columns available include; New value, Old Value, Record Type, Record Title, Record Owner and Record Action.

## Understanding Audit Trail Data {#bridgehead_N688275}

The Audit Trail offers a rich selection of data that can be used to gather a detailed understanding about the changes made. In the example below two changes were made to a saved search.

1.  The Public box was unmarked. This change registered 2 changes in the Audit Trail.
    
    -   The Search Options component type was updated from value=T to value=F.
        
    -   The component type Audience was updated from value=T to value=F.
        
    
    In effect the value for the Audience Search Option was changed from true to false.
    
2.  The Public box was marked again. This change also registered 2 changes in the Audit Trail - the reverse of the previous changes.
    

![Public box checked.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/public1.png)

## Tips {#bridgehead_N688346}

-   A single user action can create a series of cascading events in the audit trail. When reading audit trail data it is useful to group actions by date and time. Actions with the same time are most probably a single action.
    
-   Customize the audit view to increase your understanding of what events took place.
    
-   Focus on the key data that you need. Are you searching for the new and old values, or are you more concerned with who made the change?
    

### Related Topics

-   [Audit Trail for Saved Searches, Reports and Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688127.html)
-   [Audit Trail Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688379.html)
-   [Auditing Changes to Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688421.html)
-   [Auditing Saved Search Execution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N688494.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
