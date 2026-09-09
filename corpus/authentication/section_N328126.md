---
id: "section_N328126"
type: "section"
title: "Designate Two-Factor Authentication Roles"
branch: "authentication"
category: "account-administration"
breadcrumb: "Account Administration > Authentication > Two-Factor Authentication (2FA) > Designate Two-Factor Authentication Roles"
parent: "chapter_N327688"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N328126.html"
anchors: ["procedure_N328145"]
sha256: "aef90fd6927ea4f23cc1556cbb195ed56f817c7dd5bd8e9df068bc50e44db7a9"
---

An administrator or a user with the Two-Factor Authentication base permission can use the Two-Factor Authentication Roles page to indicate 2FA-required roles. Each 2FA role can be configured to specify how often users with that role are presented with the 2FA challenge. The Duration of Trusted Device column includes values for hours (4, 6, 8, 12) and days (1-30). The default value is Per session. The value works in conjunction with the devices users indicate as trusted devices. See [Users and Trusted Devices for Two-Factor Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4702272427.html) for more information.

Important:

The 2FA-required designation can be applied to most roles, including Employee Center, Partner Center, and Vendor Center roles, but not to Customer Center roles.

2FA is required for the Administrator role and other roles with highly privileged permissions. These roles are indicated in the **Mandatory 2FA** columns on the Two-Factor Authentication Roles page. For more information, see [Permissions Requiring Two-Factor Authentication (2FA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515446005.html).

#### To designate two-factor authentication roles: {#procedure_N328145}

1.  Go to _Setup > Users/Roles > Two-Factor Authentication Roles_.
    
2.  Select **2FA authentication required** from the list in the **Two-Factor Authentication Required** column for any role that you want to be 2FA required.
    
    ![Duration of Trusted Device dropdown list on the Two-Factor Authentication Roles page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/Authentication/2FA_2019_2_Mandatory2FAColumn_2FARolesPage.png)
3.  In the **Duration of Trusted Device** column, accept the default (Per session) or select the length of time before a device a user has marked as trusted will be subject to a two-factor authentication request.
    
4.  Click **Submit**.
    

Note:

The Two-Factor Authentication feature isn't compatible with web services or SuiteAnalytics Connect. To use web services or SuiteAnalytics Connect, you must be logged in with a role that doesn't require 2FA. If you want to use RESTlets or web services with a highly privileged role, use Token-based Authentication or OAuth 2.0. See [Token-based Authentication (TBA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4247329078.html) or [OAuth 2.0](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157769826287.html) for more information. OAuth 2.0 can't be used with SOAP web services.

If you need more information about setting up access or roles in NetSuite, see [NetSuite Roles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285436.html) and [NetSuite Access Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285060.html).

### Related Topics

-   [Two-Factor Authentication (2FA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N327688.html)
-   [Managing Two-Factor Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N327761.html)
-   [Users and Trusted Devices for Two-Factor Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4702272427.html)
-   [2FA in the NetSuite Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4410552915.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
