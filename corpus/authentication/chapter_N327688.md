---
id: "chapter_N327688"
type: "chapter"
title: "Two-Factor Authentication (2FA)"
branch: "authentication"
category: "account-administration"
breadcrumb: "Account Administration > Authentication > Two-Factor Authentication (2FA)"
parent: "book_4299752196"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N327688.html"
anchors: ["subsect_1531243338", "subsect_1531243566"]
sha256: "593aa42bea0e795fa42511ba3b120a3fac0c5594d5455962f22c81b7af13fd25"
---

Two-factor authentication (2FA) enforces a second level of security for logging in to the NetSuite user interface. Using 2FA can protect your company from unauthorized access to data.

Two-factor authentication requires that users log in to the NetSuite UI with:

-   NetSuite user credentials-their email address and password.
    
-   A verification code. Each verification code is a unique series of numbers valid for a limited time, and only for a single login. Users choose an authenticator app for receiving verification codes during 2FA setup. When users finish their 2FA setup, they receive a list of one-time use backup codes.
    
-   An authenticator app that complies with OATH TOTP. The app generates a time-based verification code for each login. Authenticator apps are supported in all NetSuite accounts. See [Supported Authenticator Apps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1490363269.html).
    

See the following sections for more information:

-   [What Administrators Need to Know About 2FA](#subsect_1531243338)
    
-   [Benefits of 2FA in Your NetSuite Account](#subsect_1531243566)
    

To read 2FA help topics available to users, see [Logging In Using Two-Factor Authentication (2FA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1493300400.html).

## What Administrators Need to Know About 2FA {#subsect_1531243338}

-   Certain roles with highly privileged permissions require using 2FA in NetSuite. See [Permissions Requiring Two-Factor Authentication (2FA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515446005.html).
    
-   New users are prompted to set up security questions when they first log in to NetSuite. However, users logging in with a 2FA role aren't prompted to answer security questions. The level of security provided by 2FA is greater than that provided by security questions. Users logging in with 2FA roles are only asked to answer their security questions if they forget their passwords. See [Setting Up Security Questions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1548704486.html) for more information.
    
-   2FA isn't compatible with web services or SuiteAnalytics Connect. If you want to use RESTlets or web services with a 2FA-required role, use OAuth 2.0 or Token-based Authentication. See [OAuth 2.0](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157769826287.html) and [Token-based Authentication (TBA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4247329078.html) for more information.
    
    Note:
    
    OAuth 2.0 is only available for use with RESTlets and REST web services. It can't be used with SOAP web services.
    
-   If a role is designated as a SAML Single Sign-on (SSO) role, the SAML authentication requirement takes precedence, and the 2FA requirement is ignored.
    

## Benefits of 2FA in Your NetSuite Account {#subsect_1531243566}

The benefits of 2FA include:

-   No special licensing is required. (No cost.)
    
-   No special tokens are required. (No cost.)
    
-   Access is supported for the NetSuite UI and NetSuite Mobile applications.
    
-   Little maintenance is required of administrators. After being assigned to a 2FA required role, users configure their own 2FA settings and manage their own devices in NetSuite.
    
-   Self-service user setup: pages in the NetSuite UI guide users through setting up 2FA, and provide users with backup codes.
    
-   2FA works with all non-customer center roles, including contacts.
    
-   The user's 2FA setup is shared across all NetSuite accounts and for all companies to which they have access.
    

### Related Topics

-   [Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_4299752196.html)
-   [Managing Two-Factor Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N327761.html)
-   [Designate Two-Factor Authentication Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N328126.html)
-   [Users and Trusted Devices for Two-Factor Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4702272427.html)
-   [2FA in the NetSuite Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4410552915.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
