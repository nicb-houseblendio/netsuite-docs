---
id: "section_N2444542"
type: "section"
title: "Managing Issue Status Transitions"
branch: "issue-management"
category: "support-management"
breadcrumb: "Support Management > Issue Management > Managing Issue Status Transitions"
parent: "chapter_N2438260"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2444542.html"
anchors: ["procedure_N2444666"]
sha256: "e295a939d3efd144fab4942f5c83ccf6de00dcf5e3776e85f2be145fb1edf3c5"
---

On the Manage Status Transitions page, you can set the workflow of issue statuses. For example, you can decide that when an issue is created, its status can only be either Submitted, In Progress, or On Hold. Or, you can decide that an issue in Released status can't be changed to any other status.

You can set up a status workflow for each issue role and issue type combination. For example, if you use four issue roles and two issue types, you can create up to eight unique status workflows.

Select the issue role and issue type before checking the boxes for which settings can be made on issue records.

Warning:

If you've already submitted issues using the current status transition table, only make changes that ensure open issues can continue the resolution process. For example, if an issue is assigned to a QA Engineer in Fixed status, make sure that user role can either change the status to Closed, or reassign the issue.

The following should be completed before managing status transitions:

1.  To set up issue types, see [Setting Up Issue Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442528.html).
    
2.  To set up issue roles, see [Creating Issue Role Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2443675.html).
    
3.  To set up issue statuses, see [Setting Up Issue Statuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2441539.html).
    

Note:

Administrator issue role types can use any status transition, so they don't show up in the Issue Role field on this page.

#### To manage issue status transitions: {#procedure_N2444666}

1.  Go to _Setup > Issues > Manage Status Transitions_.
    
2.  In the **Issue Role** field at the bottom of the page, select the role type you want to manage statuses for.
    
3.  In the **Issue Type** field, select the type of issue you want to set transitions for when employees use the role type you selected.
    
4.  Click the **Mark All** button to check all boxes.
    
5.  In the -Start- row, clear the boxes for each status you don't want available when an issue is first created.
    
    For example, you may want to clear any boxes in the status columns with a base status of **Closed**.
    
6.  For each status in the **From** column, clear the boxes for any statuses that shouldn't be available for the next stage in issue resolution.
    
    Each status row on the left side of the table represents the status an issue will be changing from. The status columns represent the possible statuses that an issue of that status can change to.
    
7.  Click **Submit**.
    

You can return to this page anytime to edit your settings for each issue role and issue type.

### Related Topics

-   [Issue Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2439679.html)
-   [Issue Management Setup Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2439844.html)
-   [Getting Started With Issue Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2440450.html)
-   [Setting Issue Management Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2441221.html)
-   [Creating an Issue External Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442071.html)
-   [Setting Up Issue Severities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442248.html)
-   [Setting Up Issue Priorities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442386.html)
-   [Setting Up Issue Sources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442704.html)
-   [Setting Up Issue Reproducibility](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442842.html)
-   [Setting Up Issue Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442980.html)
-   [Working with Products and Modules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2443140.html)
-   [Managing Issue Status Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2444542.html)
-   [Creating Employee Groups for Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2444787.html)
-   [Customizing Issue Notification Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445049.html)
-   [Logging Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445262.html)
-   [Linking Issues with Cases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445726.html)
-   [Working with Related Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3736605424.html)
-   [Issue Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2438260.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
