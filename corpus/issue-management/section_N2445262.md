---
id: "section_N2445262"
type: "section"
title: "Logging Issues"
branch: "issue-management"
category: "support-management"
breadcrumb: "Support Management > Issue Management > Logging Issues"
parent: "chapter_N2438260"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445262.html"
anchors: ["procedure_N2445314", "procedure_1549885388", "procedure_N2445538", "procedure_N2445634"]
sha256: "2391031d8ed24b12411482c8fd2370487fb934b247fe3866cc2acf74013cfef3"
---

Tip:

You can get writing help for text fields Abstract, New Details, External Abstract, and External Details from our generative AI service, NetSuite Text Enhance. Click the Enhance Text button to use the available options. For more information about using this capability, see [Text Enhance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2171112518.html).

You can log issues at _Issues > Issues > Issues > New_. After you create an issue record, you can attach the issue to case records.

#### To create an issue record: {#procedure_N2445314}

1.  Go to _Issues > Issues > Issues > New_.
    
2.  Under Primary Information:
    
    1.  In the **Issue Type** field, select the type of problem or request that needs resolution.
        
    2.  In the **Product Team** field, select the group that handles issues of this type.
        
    3.  In the **Assigned To** field, select the person or group who needs to perform the next step in resolving this issue.
        
        If your issue role type is set to restrict assignees, you can only assign issues to others with the same issue role type as yours. To assign an issue to another role, you must leave this field blank. Then, you must change the status to one that's linked to another issue role type. Administrators can change this setting at Setup > Issues > Issues Roles.
        
    4.  In the **Issue Status** field, select the status of this issue. The status indicates what needs to be done next to resolve this issue.
        
    5.  In the **Severity** field, choose the severity level that describes how much this issue is affecting product use.
        
    6.  In the **Priority** field, select an issue priority from 1 to 5.
        
        1 is the highest priority and 5 is the lowest.
        
    7.  Check the **Showstopper** box if this issue is preventing the next product version.
        
    8.  In the **Abstract** field, enter a brief description of the issue.
        
        This abstract shows both internally and in the NetSuite Support Center unless you enter an external abstract on the **External** subtab.
        
    9.  If this issue is related to another existing issue, click the **Related Records** subtab, and note the related issues. For more information, see [Working with Related Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3736605424.html).
        
3.  Under Problem Information:
    
    1.  In the **Item** field, select the item this issue is about.
        
    2.  In the **Product** field, select the name of the product this issue is about.
        
        To create product records, go to _Issues > Setup > Products > New_.
        
    3.  In the **Module** field, select the module type for the product. Modules are created and added on each product record.
        
    4.  In the **Source** field, select how you were made aware of this issue.
        
    5.  In the **Reproduced** field, select whether this issue has been reproduced and where.
        
    6.  In the **Tags** field, select keywords associated with this issue.
        
        Selecting tags makes it easier for others to find this issue when searching.
        
    7.  In the **Broken In Version** and **Build** field, select the product version and build experiencing the issue.
        
4.  Click the **Details** subtab.
    
5.  In the **New Details** field, enter a detailed description of the issue, where the problem is occurring, and steps to reproduce the issue.
    
6.  Click **Save**, or click the **Communication** subtab to email other employees or set up a notification email.
    

#### To close an issue: {#procedure_1549885388}

1.  Go to _Issues > Issues_.
    
2.  **Edit** the required issue.
    
3.  In the **Issue Status** field, select the reason for closing the issue.
    
4.  Click **Save**.
    

#### To email an issue: {#procedure_N2445538}

1.  On the issue record, click the **Communication** subtab.
    
2.  Check the **I Own This Issue** box to be assigned this issue when it's sent back to the status for your issue role.
    
    For example, an engineer enters a fix for an issue and then sets the status to **Fixed**. Then, the engineer assigns the issue to the QA issue queue. When a QA engineer tests the issue, they still experience the issue. The QA engineer then sets the status back to **In Progress**. Because this status is associated with the Development role type, the issue is automatically assigned back to the same engineer.
    
    There can only be one owner per issue for each issue role type.
    
    This preference isn't available unless the **Use Last Assignee** box is checked at _Issues > Setup > Issue Preferences_.
    
3.  In the **Email Me When** field, select when you want to be emailed a current copy of this issue.
    
4.  Check the **Email Assignee** box to send a copy of this issue to the person selected in the Assigned To field.
    
5.  In the **Copy Employees** field, you can select employees to send copies of this issue.
    
6.  In the **Email Functional Teams** field, select the employee groups you want to copy on this issue.
    
    Emailing a group sends an email to the address saved on the group record, not to each member individually.
    
7.  Click **Save**.
    

#### To enter an external abstract and details: {#procedure_N2445634}

1.  On the issue record, click the **External** subtab.
    
    Information you add here is shown to customers when they view issues in the Customer Center.
    
2.  In the **External Abstract** field, enter an abstract for this issue to show customers.
    
3.  In the **External Details** field, enter details about the issue to show customers.
    
4.  Click **Save**.
    

You can now attach this issue to cases on the **Issues** subtab of the case record.

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
-   [Linking Issues with Cases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445726.html)
-   [Working with Related Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3736605424.html)
-   [Issue Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2438260.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
