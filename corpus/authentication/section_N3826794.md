---
id: "section_N3826794"
type: "section"
title: "Complete the SAML Setup Page"
branch: "authentication"
category: "account-administration"
breadcrumb: "Account Administration > Authentication > SAML Single Sign-on > Complete the SAML Setup Page"
parent: "chapter_N3825119"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3826794.html"
anchors: ["kaltura_player_7", "bridgehead_N3826895", "subsect_1528125952", "subsect_1528125879", "bridgehead_N3826938"]
sha256: "9787fed6b70575b334b06b6026041fb71834de4c0bc93e1f1f4798edba034c64"
---

When the SAML Single Sign-on feature is enabled, the SAML Setup page is available at _Setup > Integration > SAML Single Sign-on_, to administrators and to users with the Set Up SAML Single Sign-on permission. (For details about SAML Single Sign-on permissions, see [Add SAML Single Sign-on Permissions to Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3827316.html).)

<a id="kaltura_player_7"></a>

Note:

As of May 2020, the default value for the location is set to the NetSuite system domain. You do not have to change the configuration if we move your account to a different data center location, or if you configure SAML SSO in multiple accounts in various data center locations.

For details about completing the SAML Setup page, see:

-   [Defining the NetSuite Configuration for SAML](#bridgehead_N3826895)
    
-   [Set Up Your Identity Provider (IdP) in NetSuite](#bridgehead_N3826938)
    

Note:

To enable SAML access to a website (as opposed to the NetSuite application), you need to complete the SAML subtab of the Web Site Setup page. See [SAML Single Sign-on Access to Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3940510119.html).

## Defining the NetSuite Configuration for SAML {#bridgehead_N3826895}

To support SAML single sign-on access to NetSuite, you must define the following on the SAML Setup page:

-   The [Logout Landing Page](#subsect_1528125952).
    
-   Optionally, the [Primary Authentication Method](#subsect_1528125879).
    

### Logout Landing Page {#subsect_1528125952}

**Logout Landing Page** - the URL for a page that users should be redirected to when they log out of NetSuite. An IdP Single Logout page can be specified for Single Logout to work.

Note:

This solution is not part of the SAML 2.0 standard. There is no guarantee that this will work.

### Primary Authentication Method {#subsect_1528125879}

The Primary Authentication Method is optional.

-   By default, the **Primary Authentication Method** box is not checked. If SAML users click a link to access NetSuite when no active NetSuite session exists, they are redirected to the NetSuite login page. This redirect might cause issues for users who do not know their NetSuite credentials.
    
-   If you check the **Primary Authentication Method** box, users can be redirected to the external IdP login page. This redirect is available if:
    
    -   the user has already been logged in, the redirect occurs based on previous experience with NetSuite.
        
    -   the access link includes the NetSuite account ID set as the **c** or **compid** URL parameter or as an account-specific domain, formatted like the following:
        
        https://system.netsuite.com/app/center/card.nl?c=<ACCOUNTID> or https://<accountID>.app.netsuite.com/app/center/card.nl
        
        Note:
        
        If the **Primary Authentication box** is checked, and a user clicks a link containing the **c** or **compid** URL parameter or the account-specific domain URL, the user is redirected to the external IdP login page. The originally requested URL will be passed as a RelayState parameter, in accordance with the SAML 2.0 specification. This means that the IdP can direct the user back to the correct NetSuite resource after authentication. If there is a live session for the IdP, the user will be directed back to the NetSuite resource without being asked for credentials.
        
    -   Users will be redirected to the IdP login page upon session timeouts.
        

## Set Up Your Identity Provider (IdP) in NetSuite {#bridgehead_N3826938}

SAML SSO access to NetSuite requires an IdP metadata XML file. The format of this file must be aligned with SAML v2.0 specifications.

On the SAML Setup page, the IdP metadata file can be specified by entering a URL or by uploading the metadata XML file. This is the information you gathered when you were setting up NetSuite with your IdP.

You must do one of the following:

-   Choose **Indicate IDP metadata URL** and enter the location URL of the metadata file.
    
-   Or, choose the **Upload IDP metadata File** option and browse to locate the file.
    

Note:

If you need to make changes to the IdP configuration, see [Update Identity Provider Information in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518814069.html).

### Related Topics

-   [SAML Single Sign-on](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3825119.html)
-   [Complete Preliminary Steps in NetSuite for SAML SSO](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3825373.html)
-   [Configure NetSuite with Your Identity Provider](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1520724227.html)
-   [Update Identity Provider Information in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518814069.html)
-   [IdP Metadata and SAML Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1520894757.html)
-   [Interactions with NetSuite Using SAML](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1520981877.html)
-   [SAML SSO in Multiple NetSuite Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4430963939.html)
-   [NetSuite SAML Certificate References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3715154860.html)
-   [Remove SAML Access to NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3827717.html)
-   [SAML SSO FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1541168340.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
