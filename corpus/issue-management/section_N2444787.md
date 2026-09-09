---
id: "section_N2444787"
type: "section"
title: "Creating Employee Groups for Issues"
branch: "issue-management"
category: "support-management"
breadcrumb: "Support Management > Issue Management > Creating Employee Groups for Issues"
parent: "chapter_N2438260"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2444787.html"
anchors: ["procedure_N2444846"]
sha256: "09acfdef548026560e517cbe9ce08affe1b54157278c1adb1ebc4774931f6e92"
---

You can create three types of employee groups for working with issues:

-   **Product Team groups** - Can be selected in the Product Team field on issues. Product teams decide who's responsible for resolving an issue. Members of this team receive an email notification when an issue is first entered, so everyone knows about the problem.
    
-   **Functional Team groups** - Can be emailed copies of the issue from the Communication subtab on issue records. You may want to check this box for all product team groups, then create additional function team groups for other teams you want to email.
    
-   **Issue Role/Issue Queue groups** - Roles that correspond to the role of this group's members can assign this group to issues.
    

One group can be a product team, a functional team, and have an issue role if needed.

#### To create an employee group for issues: {#procedure_N2444846}

1.  Go to _Lists > Relationships > Groups > New_.
    
2.  On the Create Group page, select **Static**.
    
3.  Select **Employee** as the type of members you would like to include in the group.
    
4.  Click **Continue**.
    
5.  In the **Name** field, enter a name for this group.
    
6.  Select the owner of this group. You are selected by default.
    
    Only the group owner can add or remove members or delete the group.
    
7.  In the **Email** field, enter an email alias for this group.
    
    Note:
    
    The group email address is used for non-issue notifications. For example, when composing an email you can use this address to cc the group. Issue notifications, however, are sent directly to each member's individual email address.
    
8.  Check the **Product Team** box if this group handles issues for a particular product.
    
    You can select product team groups on issue records and associate them with issue tags. If you select a tag associated with a product team on an issue record, the related product team will be selected automatically.
    
9.  Check the **Functional Team** box to let this group be emailed from the **Communication** subtab on issue records. Email is sent from the address in the Email field on this group's record.
    
    If this group is a product team or issue queue, this option sends them a copy of the issue record by email, when needed.
    
10.  In the **Issue Role** field, select an issue role type to make this group an issue queue. Assigning an issue role lets the group be assigned to issues using the defaults and status transitions for that role type.
     
     Employees with the **Restrict Assignees** issue role type can assign issues to issue queues when assigning issues outside of their role type.
     
     For example, a support person with restricted assignees can assign a new customer-reported issue to a QA Investigation issue queue/group. A member of the QA Investigation group can then assign it to the appropriate person for further investigation.
     
11.  On the **Members** subtab, do the following to add members to this group:
     
     -   To add individual members, enter part of a member's name in the **Name** column, and press Tab. Select a member, and click Add. Repeat these steps for each member.
         
     -   Click **Add Multiple**, and hold CTRL to select more than one member from the list.
         
     -   Click **Add With Search** to enter search criteria for the members you want to add.
         
     
     You can use more than one of these methods to add members to the same group. For example, select a few members individually, and then add all members that meet certain search criteria.
     
12.  Click **Save**.
     

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
-   [Customizing Issue Notification Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445049.html)
-   [Logging Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445262.html)
-   [Linking Issues with Cases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2445726.html)
-   [Working with Related Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3736605424.html)
-   [Issue Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2438260.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
