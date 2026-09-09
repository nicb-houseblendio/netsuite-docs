---
id: "section_N2422557"
type: "section"
title: "Creating Case Statuses"
branch: "setting-up-case-management"
category: "support-management"
breadcrumb: "Support Management > Setting Up Case Management > Setting Up Support Checklist > Creating Case Statuses"
parent: "section_N2421296"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2422557.html"
anchors: ["procedure_N2422608"]
sha256: "34792002c7802cd2abaefa6f19ad6d4eb1ae1feb913538cea955fd7ab4e2e0d0"
---

You can create custom statuses for your customer support cases. Statuses show how close a case is to being closed or how it was closed.

The Case Status field appears on case records. If you use online case forms, you can choose to show or hide this field on the form.

For example, Wolfe Electronics wants to keep cases open until customers confirm that their issue is completely resolved. They change the In Progress status to Awaiting Customer Reply for cases that need more information, and then create new statuses: Repairs Needed, Awaiting Confirmation, and Confirmed.

NetSuite provides the following default case statuses that can be edited:

-   Not Started
    
-   In Progress
    
-   Escalated
    
-   Re-Opened
    
-   Closed
    

#### To create a case status: {#procedure_N2422608}

1.  Go to _Setup > Support > Case Statuses > New_.
    
2.  In the **Case Status** field, enter a name for the new status.
    
    This name appears in the **Status** field on case records.
    
3.  In the **Insert Before** field, select where you want this status listed in the **Status** field on case records.
    
    For example, you may want to arrange statuses by how cases are resolved or alphabetically.
    
4.  In the **Stage** field, choose if this status describes cases that are Open, Escalated, or Closed.
    
    Statuses must be associated with a stage.
    
    For example, you can create an Awaiting Customer Response status for the Open State. This would mean that support has asked the customer for more information to resolve the case.
    
5.  Check the **On Hold** box if you don't want time counted against cases with this status.
    
    For example, if you're waiting for a reply from a customer or a solution from another department, use an on hold status to pause the case's time log. This lets you track your support team's efficiency more accurately.
    
6.  Check the **Show Awaiting Support Reply** box if you want this case status to show in searches and case tracking reports.
    
7.  If you use the **Issue Management** feature, check the **Auto Close With Issues** box. This option automatically closes a case of this status when all attached issues are closed.
    
    You must also have the **Automatically Close Linked Cases** box checked at _Setup > Issues > Issue Preferences_.
    
8.  In the **Description** field, enter a brief definition of cases that should be assigned this status.
    
9.  Click **Save**.
    

### Related Topics

-   [Creating Case Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2422185.html)
-   [Creating Case Origins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2422364.html)
-   [Creating Case Priorities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2422747.html)
-   [Creating Case Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2422868.html)
-   [Offering Support for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2423026.html)
-   [Setting Up Support Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2423204.html)
-   [Setting Customer Service Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2423389.html)
-   [Marking Employees as Support Reps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2426343.html)
-   [Setting Up Support Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2421296.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
