---
id: "bridgehead_N3827426"
type: "bridgehead"
title: "SAML SSO Permission Limitations"
branch: "authentication"
category: "account-administration"
breadcrumb: "Account Administration > Authentication > SAML Single Sign-on > Complete Preliminary Steps in NetSuite for SAML SSO > Add SAML Single Sign-on Permissions to Roles > SAML SSO Permission Limitations"
parent: "section_N3827316"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3827426.html"
anchors: []
sha256: "7770943176aad11d92dab4b0066bf30d0fac0061e43c25a57aaacea7854d8899"
---

SAML Single Sign-on roles and permissions have various limitations that are intended to prevent problems.

No one can log in as an administrator using SAML single sign-on. This limitation makes sure a user with the Administrator role can always log in and fix any issues with the third-party IdP setup or SAML access.

Administrators cannot add SAML Single Sign-on permission to a role that has SuiteAnalytics Connect permission; SAML access is not supported for SuiteAnalytics Connect.

Some limitations make sure the administrator is fully responsible for deciding who can access their NetSuite account with SAML Single Sign-on. The administrator is choosing to trust the third-party IdP to authenticate and let people into their NetSuite account. That's why these limitations exist:

-   If someone logs in to NetSuite with a role that doesn't have SAML Single Sign-on permission, they can't access any roles that do have it. This stops users from switching between SAML and non-SAML roles with different privileges.
    
-   As of 2018.1, it is up to an administrator to decide whether users should be locked in a single account. See [Account Attribute](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1518813066.html#subsect_1518211003) for more information. (In previous releases, a user who accessed NetSuite through SAML Single Sign-on could not access any roles that belonged to a different NetSuite account. SAML Single Sign-on access was provided to only a single account.)
    

Some limitations are intended to ensure there are no conflicts resulting from having two different trust authorities (the third-party IdP and NetSuite) authenticating a single user. After SAML is enabled for certain roles in an account, NetSuite trusts the third-party identity provider. This is the reason behind the following limitations:

-   A user who has accessed NetSuite through SAML Single Sign-on cannot access any roles that do not have SAML Single Sign-on permission. This prevents users from switching from a SAML role to a non-SAML role with greater privileges.
    
-   Only one type of inbound single sign-on permission can be assigned to a specific role. If a role has SAML Single Sign-on permission, it cannot have OpenID Connect (OIDC) Single Sign-on permission.
    

### Related Topics

-   [SAML Single Sign-on](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3825119.html)
-   [Configure NetSuite with Your Identity Provider](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1520724227.html)
-   [Complete the SAML Setup Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3826794.html)
-   [Update Identity Provider Information in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518814069.html)
-   [IdP Metadata and SAML Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1520894757.html)
-   [Interactions with NetSuite Using SAML](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1520981877.html)
-   [SAML SSO in Multiple NetSuite Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4430963939.html)
-   [NetSuite SAML Certificate References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3715154860.html)
-   [Remove SAML Access to NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3827717.html)
-   [SAML SSO FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1541168340.html)
-   [Add SAML Single Sign-on Permissions to Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3827316.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
