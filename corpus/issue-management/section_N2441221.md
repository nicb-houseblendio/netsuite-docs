---
id: "section_N2441221"
type: "section"
title: "Setting Issue Management Preferences"
branch: "issue-management"
category: "support-management"
breadcrumb: "Support Management > Issue Management > Setting Issue Management Preferences"
parent: "chapter_N2438260"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2441221.html"
anchors: ["procedure_N2441250"]
sha256: "aeb6261a1761b53a589092b5457e5697e9c707c4bf6d3c4635599b84e4527d0f"
---

You can set general preferences for the Issue Management feature on the Issue Preferences page. You can allow multiple versions and builds to be selected on issues. You can also set cases linked to an issue to automatically close when the issue is closed.

#### To set preferences for the Issue Management feature: {#procedure_N2441250}

1.  Go to _Issues > Setup > Preferences > Issue Preferences_.
    
2.  Check **Use Last Assignee** to automatically assign an issue to the last employee assigned the issue for the role type associated with the status.
    
    For example, an Engineer sets the status to Fixed, sending the issue to QA for completion. The QA Engineer finds that the issue still needs work and sets the status back to In Progress. When the status is set to In Progress, it's automatically assigned to the Engineer who was last assigned to the issue.
    
3.  Check **Use Multiple Versions and Builds** to add a **Versions** subtab to issue records. This lets you set an issue as broken in, targeted for, or fixed in more than one version and build.
    
    For example, a company that produces software finds that the same issue is present in both their Version 5 and Version 6 products.
    
4.  Check **Automatically Close Linked Cases** to set a case's status to **Closed** when all attached issues are set to a base status of **Closed**.
    
    Note:
    
    A case must be in a status that allows automatic closure to close with closed issues. To mark a case status as one that can automatically close, edit the case status. Go to _Setup > Support > Setup Tasks > Case Statuses > New_. Check **Auto Close With Issues**.
    
    You can have an email notification sent to customers when cases are closed automatically after their associated issues are closed. Go to _Setup > Support > Preferences > Support Preferences_. Under Notification, check **Notify Customer Upon Automatic Closure**.
    
5.  In the **Send Customer Notification When** field, select default criteria for when customers that have cases associated with an issue should be notified by email.
    
    For example, issue 503 is attached to a case submitted by customer Mary Smith. Selecting Status Changes sends email to the email address on the case record every time issue 503 changes status.
    
    Customers can change the notification criteria or choose not to be notified using preferences in the Customer Center.
    
6.  Check **Allow Customer Override** if you want customers to be able to change their issue notification email settings in the Customer Center.
    
7.  In the **Customer Template** field, select the template you want to use to notify customers of changes to an issue.
    
8.  In the **Employee Template** field, select the template you want to use to notify employees of changes to an issue.
    
    You can customize these templates at _Setup > Issues > Issue Preferences_. For more information, see [Customizing Issue Notification Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445049.html).
    
9.  Click **Save**.
    

### Related Topics

-   [Issue Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2439679.html)
-   [Issue Management Setup Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2439844.html)
-   [Getting Started With Issue Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2440450.html)
-   [Setting Issue Management Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2441221.html)
-   [Setting Up Issue Statuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2441539.html)
-   [Creating an Issue External Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442071.html)
-   [Setting Up Issue Severities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442248.html)
-   [Setting Up Issue Priorities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442386.html)
-   [Setting Up Issue Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442528.html)
-   [Setting Up Issue Sources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442704.html)
-   [Setting Up Issue Reproducibility](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442842.html)
-   [Setting Up Issue Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2442980.html)
-   [Working with Products and Modules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2443140.html)
-   [Creating Issue Role Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2443675.html)
-   [Managing Issue Status Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2444542.html)
-   [Creating Employee Groups for Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2444787.html)
-   [Logging Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445262.html)
-   [Linking Issues with Cases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445726.html)
-   [Working with Related Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3736605424.html)
-   [Issue Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2438260.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
