---
id: "chapter_N2903520"
type: "chapter"
title: "Setting Up Your SuiteScript Environment"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > Setting Up Your SuiteScript Environment"
parent: "book_14946590423"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2903520.html"
anchors: ["subsect_14174037626", "procedure_N2903757"]
sha256: "36089c9375e063c7661744d38a5cd81b012e48110573972d26d4d9fbab824cde"
---

Before working with SuiteScript, you must configure both your NetSuite account and SuiteScript development environment. To do so, see the following topics.

-   [Enabling SuiteScript](#subsect_14174037626)
    
-   [Showing Record and Field IDs in Your Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0402065629.html)
    
-   [Setting Roles and Permissions for SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0403053450.html)
    
-   [Setting Up Your SuiteScript Development Environment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0402065535.html)
    

## Enabling SuiteScript {#subsect_14174037626}

Before you can use SuiteScript, a user with the Administrator role must enable the SuiteScript features that you plan to use.

#### To enable SuiteScript: {#procedure_N2903757}

1.  Go to _Setup > Company > Enable Features_.
    
2.  Click the **SuiteCloud** subtab.
    
3.  Under SuiteScript, check the **Client SuiteScript** or **Server SuiteScript** box (or both, depending on the scripts you want to run).
    
4.  Click **Save**.
    

Note:

If the Client SuiteScript feature is enabled, the **Custom Code** subtab becomes available on entry and transaction forms (see the following screenshot). On this subtab, you select the client script that you want to associate with the current form. For information about attaching client scripts to NetSuite forms, see [Associating Custom Code (Client SuiteScript) Files With Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2860797.html).

![The Custom Code tab on entry and transaciotn forms.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/customCodeTab.png)

After enabling SuiteScript, continue configuring your NetSuite account:

-   **Set up roles and permissions for SuiteScript** - Roles and permissions determine a user's level of access to specific areas in NetSuite. For information about SuiteScript permissions, see [Setting Roles and Permissions for SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0403053450.html).
    
-   **Set the preference to show internal IDs** - Internal record and field IDs are used as parameters in SuiteScript code. For information about the preference and how to view internal IDs, see [Showing Record and Field IDs in Your Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0402065629.html),
    
-   **Set up your development environment** - NetSuite provides a SuiteCloud plug-in or extension for specific IDEs. You can also use other development tools to create SuiteScript files. For more information, see [Setting Up Your SuiteScript Development Environment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0402065535.html)
    

After setting up your SuiteScript environment, see the tutorial in [SuiteScript 2.1 Hello World](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1503717063.html) for a sample SuiteScript implementation.

### Related Topics:

-   [SuiteScript Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163726005075.html)
-   [SuiteScript Governance and Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3350651.html)
-   [SuiteScript Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/part_N3360914.html)
-   [SuiteScript Debugger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3014215.html)
-   [SuiteCloud Processors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1498571420.html)
-   [SuiteScript Monitoring, Auditing, and Logging](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1494642209.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [SuiteScript IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1494647249.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
