---
id: "section_N2431043"
type: "section"
title: "Customizing Support Notification Email"
branch: "setting-up-case-management"
category: "support-management"
breadcrumb: "Support Management > Setting Up Case Management > Customizing Support Notification Email"
parent: "chapter_N2421072"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2431043.html"
anchors: []
sha256: "86fc69108b88b89400d04670806e0c27ea05c23c51baa809e132078785c9254a"
---

When you create or update case records, you can set up automatic email notifications that are sent to customers and support reps. Standard templates are used by default for these notifications, but you can edit them by going to _Setup > Company > Email > System Email Templates_. You can also create custom templates for each type of notification in the following scenarios:

-   to customers when a new case is created
    
-   to customers when their case has been updated or replied to
    
-   to customers when their case has been closed because all related issues are closed
    
-   to support reps when they have been assigned to a case
    
-   to support reps when a case assigned to them has been updated
    
-   to employees when a case has been escalated to them
    

For example, Wolfe Electronics support manager changes the font and text size of the standard notification sent to customers when a new case is created, adds the company logo, and updates the wording.

Important:

Assignment notifications aren't sent when the logged in user is the new assignee, and update notifications aren't sent when the logged in user is the assignee. You can work around this limitation by creating a SuiteScript that sends a notification to the logged in user after the case is submitted.

There are three steps to set up custom notifications:

1.  Create your template.
    
2.  Upload your template.
    
3.  Select the custom template at _Setup > Support > Preferences > Support Preferences_.
    

If you use NetSuite OneWorld, set up notifications for each subsidiary.

For more information, see [Setting Subsidiary-Level Support Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2433676.html).

Note:

Automatic email notifications don't affect the initial response time. For more information, see [Performance Metrics for Support Cases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1483445494.html).

### Related Topics

-   [Creating an Email Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162316437163.html)
-   [Uploading Your Email Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162316440035.html)
-   [Creating Case Profiles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3914420072.html)
-   [Assignment Rules & Territories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2426488.html)
-   [Setting Case Escalation Rules and Assignments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2427176.html)
-   [Using Email Case Capture](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2427546.html)
-   [Online Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2428291.html)
-   [Help Desk](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2430719.html)
-   [Customizing Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2430856.html)
-   [Setting Up Customer Support in NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2433348.html)
-   [Setting Up Case Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2421072.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
