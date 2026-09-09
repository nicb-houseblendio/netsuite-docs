---
id: "section_N3381364"
type: "section"
title: "Defining Bundle Terms of Service"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Bundle Builder Reference > Defining Bundle Terms of Service"
parent: "section_4422668647"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381364.html"
anchors: ["procedure_N3381387", "bridgehead_N3381533", "bridgehead_N3381576"]
sha256: "918ae54450e953628ee1cd320c04e737a542991c12e2dd67ea1b9bf56ff275f5"
---

You can associate terms of service with a bundle and require target account users to accept these terms before they install or update the bundle.

Note that terms of service defined for an individual bundle do not replace general SuiteBundler terms of service. Bundle-specific terms of service are in addition to general terms of service.

#### To define bundle-specific terms of service: {#procedure_N3381387}

1.  On the Bundle Properties page of the Bundle Builder, click the arrow next to Terms of Service and enter terms in the box provided.
    
    ![Bundle Properties page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/TOSBlankText.png)
    -   Formatting tools are available for terms of service text (when the **Enable Rich Text Editing** option is enabled at _Home > Set Preferences_).
        
    -   You can also edit lengthy text externally and paste it into the box.
        
2.  If you want to require users to agree terms of service before proceeding with installations and updates, check the **Requires Acceptance of Terms** box.
    
    When this box is checked, users must agree to terms of service during installation and update. Note that a standard NetSuite disclaimer is always included along with your text:
    
    ![Bundler Terms of Service NetSuite Disclaimer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleTOSAgree2.png)
    
    Important:
    
    If you do not check the **Requires Acceptance of Terms** box, users will not be required to accept terms and the link to these terms is not displayed.
    
3.  After installation, the terms of service defined for a bundle are available from a link on the Bundle Details page. For details, see [Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393542.html).
    

Note the following:

-   To stop requiring users to agree to terms of service, edit the bundle in the Bundle Builder and clear the **Requires Acceptance of Terms** box.
    
-   Managed bundles only require terms acceptance during initial installation. Users aren't required to agree to terms during managed bundle updates, as authors push these updates. If the terms of service have changed, this change could be communicated to customers through bundle email messages. Customers may respond, indicating whether they accept or reject the new terms of service. If a customer rejects the new terms of service, the author can exclude the customer from future bundle upgrades.
    
-   For pushed bundles, users are not required to agree to terms during installations or updates, as these are pushed by bundle authors with administrative access to target accounts.
    

## Verifying Acceptance of Bundle Terms of Service {#bridgehead_N3381533}

You can review the most recent date that each target account has accepted a bundle's terms of service on the Bundle Install Base page.

![Bundle Install Base page with Terms Accepted On field highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleTOSInstallBase.png)

Note:

The date value is hardcoded to Pacific Time Zone and does not reflect the time zone setting on _Home > Set Preferences_.

For details on accessing this page, see [Viewing Your Bundle Install Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392340.html).

## Revising Bundle Terms of Service {#bridgehead_N3381576}

You can revise a bundle's terms of service at any time, by editing the text in the Bundle Builder.

Check the **Requires Reacceptance** box to require users to accept updated terms during installation or update. If this box is not checked, the updated terms of service are written to the Bundle Details page, but they are not displayed during bundle installation or update.

![Bundle Properties page with reacceptance terms highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/BundleBuilderTOSReaccept.png)

The **Requires Reacceptance** box appears after **Requires Acceptance** has been checked at least one time. This box is cleared each time you return to the Bundle Builder to edit terms of service text. The most recent date when you previously required reacceptance of revised terms of service is displayed, if applicable.

Warning:

This feature is not intended to provide source control for changes to bundle terms of service, but only to maintain the most current terms of service text. Bundle authors are responsible for tracking changes to their bundle's terms of service.

### Related Topics

-   [Bundle Builder Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422668647.html)
-   [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html)
-   [Using Bundle Installation Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377481.html)
-   [Bundle Support during NetSuite Release Phasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382536.html)
-   [Documenting a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380831.html)
-   [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html)
-   [File and Folder Management in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381747.html)
-   [Bundling NetSuite Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382176.html)
-   [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html)
-   [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html)
-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Step 2 Bundle Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373339.html)
-   [Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393542.html)
-   [Bundle Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3393046.html)
-   [Editing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392791.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
