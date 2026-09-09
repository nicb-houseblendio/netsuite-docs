---
id: "section_N2445726"
type: "section"
title: "Linking Issues with Cases"
branch: "issue-management"
category: "support-management"
breadcrumb: "Support Management > Issue Management > Linking Issues with Cases"
parent: "chapter_N2438260"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445726.html"
anchors: ["procedure_N2445745"]
sha256: "fc7294cd48c6e6f7e2e64dabbc618cc5d9f907b89e763514902120aed6ab29ba"
---

You can create or attach issue records on existing case records to associate issue resolution with case resolution. When you link issues with case records, support reps working with cases can track related issue progress and keep customers updated.

#### To link issues with a case record: {#procedure_N2445745}

1.  Go to _Cases > Customer Service > Cases_.
    
2.  Click **Edit** next to the case you want to associate with an issue.
    
3.  Click the **Related Records** subtab.
    
4.  Choose one of the following to attach an issue:
    
    -   Select the issue number in the **Issue** field, and click **Attach**.
        
    -   Click **New Issue** to create an issue for this case in a new window. After you save the issue and return to the case record, click **Attach** to add the new issue record.
        
5.  Click **Save**.
    

You can have a case close automatically when all attached issues are set to a base status of **Closed**. Go to _Issues > Setup >Issue Preferences_. Check the **Automatically Close Linked Cases** box. The case also closes when all linked issues are removed.

Cases can only close automatically if their status allows auto-closing with resolved issues. To set a status to allow auto-closure, edit the case status at _Setup > Support > Setup Tasks > Case Statuses_. Check the Auto Close With Issues box.

For example, Wolfe Electronics has a case titled Can't Access Download. It's linked to issue 421, where several customers purchased a download but couldn't reach it in the Customer Center. The case has a status of Waiting For Customer Response while support team verifies it matches the problem documented in issue 421. The Waiting For Customer Response status is not set to auto-close with issues.

While the case remains in this status, issue 421 is resolved and closed. The customer then responds and confirms that their problem matches what's described in issue 421. The case status now changes to Pending Issue Resolution, which is set to auto-close with issues. Because the only linked issue (421) is already closed, the case status automatically changes to Closed - Issue Resolved.

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
-   [Customizing Issue Notification Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445049.html)
-   [Logging Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445262.html)
-   [Working with Related Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3736605424.html)
-   [Issue Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2438260.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
