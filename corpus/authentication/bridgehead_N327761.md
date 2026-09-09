---
id: "bridgehead_N327761"
type: "bridgehead"
title: "Managing Two-Factor Authentication"
branch: "authentication"
category: "account-administration"
breadcrumb: "Account Administration > Authentication > Two-Factor Authentication (2FA) > Managing Two-Factor Authentication"
parent: "chapter_N327688"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N327761.html"
anchors: ["subsect_1536340317"]
sha256: "1af554e2cb5c4b5f57d19b4d3ae0ab30317e8c3cf5844ac044bdcadbbbf9e7f3"
---

You don't have to enable, or purchase a feature to use 2FA in a NetSuite account. Setup required of administrators is minimal. You can begin using 2FA in your NetSuite account at any time. Administrators, or other users with the **Two-Factor Authentication base** permission, can designate roles as 2FA required. Users who are assigned to 2FA-required roles must set up their authenticator applications in NetSuite.

Important:

2FA is required for the Administrator role and other roles with highly privileged permissions. These roles are indicated in Mandatory 2FA column on the Two-Factor Authentication Roles page. For a list of roles that are considered highly privileged, see [Permissions Requiring Two-Factor Authentication (2FA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515446005.html).

![Two-Factor Authentication Roles page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/Authentication/2FA_2019_2_Mandatory2FAColumn_2FARolesPage_30days.png)

## Required 2FA Tasks {#subsect_1536340317}

See the following required tasks for managing 2FA in a NetSuite account. These tasks can be completed by administrators and users that have the Two-Factor Authentication base permission.

-   For roles that you want to restrict as 2FA roles, designate the role as 2FA authentication required. See [Designate Two-Factor Authentication Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N328126.html).
    
-   When using 2FA, the users:
    
    -   Are sent a verification code by email during the initial login attempt to a 2FA role.
        
    -   Must set up their 2FA preferences. Authenticator apps for generating 2FA verification codes are supported in all NetSuite accounts. See the following topics written for users: [Set up Your Preferences for Two-Factor Authentication (2FA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1531519158.html).
        
        To generate verification codes using an authenticator app, users must install an authenticator application.
        

Each time a users log in to NetSuite, they must enter an email address and password. If the role is a 2FA required role, the user must also enter a verification code. Each verification code is a unique series of numbers valid for a limited time, and only for a single login. During 2FA setup, users are also supplied with backup codes that can also be used for 2FA access.

For help written for users, see [Logging In Using Two-Factor Authentication (2FA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1493300400.html).

### Related Topics

-   [Two-Factor Authentication (2FA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N327688.html)
-   [Designate Two-Factor Authentication Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N328126.html)
-   [Users and Trusted Devices for Two-Factor Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4702272427.html)
-   [2FA in the NetSuite Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4410552915.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
