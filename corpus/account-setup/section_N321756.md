---
id: "section_N321756"
type: "section"
title: "NetSuite Users Overview"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Users & Roles > NetSuite Users Overview"
parent: "chapter_N284861"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N321756.html"
anchors: ["procedure_N321781", "bridgehead_N321823", "bridgehead_3705030364"]
sha256: "91db5e5696adb982d37e3e98e9d62065afa0096f461862cfdf17dc2712fe0e1b"
---

To set up users with access to your NetSuite account, you must have the Administrator role to set up records for them, either employee, vendor, partner, or customer records, depending on the type of users. To add a user, you need to set up a record for that user and on that record, explicitly indicate that access to NetSuite should be provided

On each record, you need to provide an email address, which serves as the user ID. Each record has an Access subtab, where you can enable the Give Access option and assign roles. For users to have access to NetSuite, they must also have a password. Users with the Administrator role can send an access notification email that includes a link that lets users create their own passwords.

**For links to instructions for adding NetSuite users, see the topics in [Manage Different Types of Users](#bridgehead_3705030364).**

If you assign an additional role to a user who is currently logged in to NetSuite, that user will need to log out and log back in to NetSuite to see the newly assigned role. The same is true if you add permissions to an existing role when a user is currently logged in to NetSuite. The user needs to log out and log back in to exercise the new permissions.

Note:

When the Advanced Employee Permissions feature is enabled, the Employee System Access permission must be assigned to a role to give access and assign roles to employees. For more information, see [Employee Access Tab Permission Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1541786744.html).

To review users' roles, go to _Setup > Users/Roles > Manage Users_. The Manage Users page lists all users by name, with their email addresses and roles.

#### The Manage Users Page {#procedure_N321781}

1.  Click a user name to open his or her record. You can then click the **Edit** button in the record to make changes.
    
2.  Click an email address to send mail to the user.
    

For more information, see [Viewing Your NetSuite Users List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N324056.html).

## The Login Audit Trail {#bridgehead_N321823}

The Login Audit Trail is a specialized search that returns a list of account login and logout activity, that can be filtered by date, user, role, or IP address. This search helps keep track of account users, when they have logged in or logged out, and from where. Search results indicate whether each login or logout attempt was successful. This search is available at _Setup > Users/Roles > View Login Audit Trail_.

Note:

In some cases, users' login to NetSuite is ended when they have not explicitly logged out of NetSuite. For example, this situation occurs when a user's NetSuite session times out. If the logout is not explicit, the system does not create a logout entry in the Login Audit Trail.

For more information, see [Login Audit Trail Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N324233.html).

## Manage Different Types of Users {#bridgehead_3705030364}

See the following topics for information about setting up and maintaining access for different types of NetSuite users.

-   [Employee Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N322041.html)
    
-   [Vendor Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N322273.html)
    
-   [Partner Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N322424.html)
    
-   [Customer Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N322570.html)
    

Note:

Only active users with access count against the Full User Count purchased for your account. Inactive users that have access do not count. For details about making users inactive, see [Employee Termination](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3753809772.html).

### Related Topics

-   [NetSuite Users & Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N284861.html)
-   [NetSuite Access Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285060.html)
-   [Standard Roles Permissions Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html)
-   [Roles and Permission Considerations for APIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0320025211.html)
-   [Permissions Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326485.html)
-   [Feature Permissions Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1491844394.html)
-   [NetSuite Roles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285436.html)
-   [NetSuite Permissions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N325094.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
