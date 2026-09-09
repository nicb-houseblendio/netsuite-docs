---
id: "chapter_N3825119"
type: "chapter"
title: "SAML Single Sign-on"
branch: "authentication"
category: "account-administration"
breadcrumb: "Account Administration > Authentication > SAML Single Sign-on"
parent: "book_4299752196"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3825119.html"
anchors: ["subsect_1519940921"]
sha256: "42a9bf22eb1f8b9698985c0ad2ca3b24a3ef6616b1ed857608706add93005775"
---

SAML (Security Assertion Markup Language) is an XML-based standard that lets different apps, called service providers (SPs), share user data. An identity provider (IdP) creates security assertions that SPs use. A single IdP can handle user authentication for numerous SPs. An SP and an IdP can set up a circle of trust by sharing metadata in the SAML XML format, so the SP accepts users authenticated by the IdP.

The NetSuite SAML Single Sign-on feature is based on the SAML v2.0 specifications. For information about these specifications, click [here](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=security#samlv20). Any SAML 2.0-compliant application can serve as the IdP for SAML access to NetSuite.

This feature lets users who are already logged in to an external app go to NetSuite without needing to log in again. When someone uses SAML SSO to access NetSuite, they're taken straight to their Home page. Admins can use role-based permissions to control who gets SAML SSO access in NetSuite.

Note:

SAML SSO access to NetSuite UI honors any IP address rules for your company, or IP address restrictions for your employees, that you may have created in your NetSuite account. IP address rules or restrictions do not apply for SAML access to web stores or websites.

Note:

To use the SAML Single Sign-on feature, you need Full level for the SAML Single Sign-on permission. For more information, see [NetSuite Permissions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N325094.html).

## Task List for SAML SSO Set Up {#subsect_1519940921}

Setting up SAML SSO requires some back-and-forth between NetSuite and the IdP of your choice.

1.  In the NetSuite application, perform preliminary setup: enable the feature, create roles and assign SSO permissions, and assign users to the roles.
    
2.  Using the IdP of your choice: create your NetSuite service provider (SP) configuration. The procedure varies depending on the IdP you choose to use.
    
    Note:
    
    Some IDPs already have NetSuite listed among their out-of-the-box service providers, others require that you configure the set up of NetSuite as new SAML service provider yourself.
    
3.  In the NetSuite application, complete the SAML Setup page: create the configuration in your account for your IdP.
    

See the following sections for detailed information about each step:

-   [Complete Preliminary Steps in NetSuite for SAML SSO](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3825373.html)
    
-   [Configure NetSuite with Your Identity Provider](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1520724227.html)
    
-   [Complete the SAML Setup Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3826794.html)
    

If you are interested in setting up SAML SSO access to your web store, familiarize yourself with the SAML SSO documentation in this section. Then, see [SAML Single Sign-on Access to Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3940510119.html) for more information.

### Related Topics

-   [Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_4299752196.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
