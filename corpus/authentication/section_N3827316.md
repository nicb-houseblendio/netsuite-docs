---
id: "section_N3827316"
type: "section"
title: "Add SAML Single Sign-on Permissions to Roles"
branch: "authentication"
category: "account-administration"
breadcrumb: "Account Administration > Authentication > SAML Single Sign-on > Complete Preliminary Steps in NetSuite for SAML SSO > Add SAML Single Sign-on Permissions to Roles"
parent: "section_N3825373"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3827316.html"
anchors: []
sha256: "f6e24d552daa6aa85b9ba94aa7418eb8b3f0110b6096db965495bb651a129b0a"
---

You can customize a standard NetSuite role for use with SAML Single Sign-on (SSO) permissions. You can also add SAML SSO permissions to existing roles assigned to users that require this type of access.

Note:

If a role is already designated as two-factor authentication (2FA) required, and you add the SAML SSO permission to the role, the 2FA requirement will be ignored. The SAML SSO permission takes precedence.

To complete the following procedure, you must be logged in to NetSuite with an Administrator role. If you need more detailed information about creating roles in NetSuite, see [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html).

#### To customize roles and add SAML permissions:

1.  Go to _Setup > Users/Roles > User Management > Manage Roles_.
    
2.  Choose a role and click **Customize**.
    
3.  Create a unique and identifiable name for the role. For example, you could replace the word Customize in the role name with the word SAML.
    
4.  Click the **Permissions** subtab.
    
5.  On the **Setup** subtab, select the appropriate SAML permission from the list, and click **Add**. There are two SAML permissions. Add one or both permissions to the role as appropriate. See [SAML SSO Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1518196382.html).
    
6.  Click **Save**.
    

For more information about SAML permissions, see the following:

-   [SAML SSO Access for Center Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3827410.html)
    
-   [SAML SSO Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1518196382.html)
    
-   [SAML SSO Permission Limitations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3827426.html)
    

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

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
