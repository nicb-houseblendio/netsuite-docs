---
id: "section_N3377481"
type: "section"
title: "Using Bundle Installation Scripts"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Bundle Builder Reference > Using Bundle Installation Scripts"
parent: "section_4422668647"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377481.html"
anchors: []
sha256: "5722c53af60b670054c83e3cf9db9e860be92e28bdbcf0050885561f8367903e"
---

Bundles can include a server SuiteScript that runs automatically during installation, update, or uninstall. Bundle installation scripts can include triggers for before/after install, update, or uninstall. This trigger code can ensure that bundles are implemented and removed correctly and efficiently, and can prevent bundle installation, update, or uninstall if proper setup has not occurred. Note that this type of script can be run in any target account where the associated bundle is installed, even if scripting features are not enabled in that account.

To associate a bundle installation script with your bundle, you need to create the script .js file, upload the script file to the NetSuite File Cabinet, create a script record, and define one or more deployments for the script.

After a bundle installation script has been created and at least one deployment has been defined for it, you can associate the script with a bundle by selecting from the Installation Script list on the [Step 1 Bundle Basics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3372533.html) page. A single bundle installation script can be associated with multiple bundles. When you associate a script with a bundle, you select a specific script deployment.

Detailed documentation about bundle installation scripts is available in the SuiteScript section of the Help Center:

-   For step-by-step instructions for developing bundle installation scripts and associating them with bundles, see the SuiteScript help topic [Setting Up a Bundle Installation Script](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158134526570.html).
    
-   For more details about bundle installation scripts, see the SuiteScript help topic [SuiteScript 2.1 Bundle Installation Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460460309.html).
    
-   To review a sample script, see [Bundle Installation Script Sample](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460460309.html#bridgehead_4468410297).
    

Note:

On the [Step 3 Select Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373513.html) page of the Bundle Builder, you do not have to explicitly add the bundle installation script. This script record and the related .js file are included automatically in the bundle, as are any other .js files that are listed as library script files on the script record.

### Related Topics

-   [Bundle Builder Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422668647.html)
-   [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html)
-   [Bundle Support during NetSuite Release Phasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382536.html)
-   [Documenting a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380831.html)
-   [Defining Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381364.html)
-   [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html)
-   [File and Folder Management in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381747.html)
-   [Bundling NetSuite Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382176.html)
-   [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html)
-   [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [SuiteScript 1.0 Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7151939532.html)
-   [SuiteScript 1.0 Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7151939532.html)
-   [Setting Up a Bundle Installation Script](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158134526570.html)
-   [SuiteScript 1.0 Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7151939532.html)
-   [SuiteApps and Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3405306.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
