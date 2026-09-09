---
id: "section_N3377764"
type: "section"
title: "Protecting Your Bundled Server SuiteScripts"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Bundle Builder Reference > Protecting Your Bundled Server SuiteScripts"
parent: "section_4422668647"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html"
anchors: ["procedure_N3377830"]
sha256: "d58b2f9574ba315352771f63716b9c06f242e4d3cd00082e97b410ef5ae04ee4"
---

You can include server SuiteScripts in bundles and hide their contents from users.

To hide a server-side script in a bundle, you must upload your SuiteScript .js file to the File Cabinet and then edit the file record. On the file record, enable the **Hide in SuiteBundle** preference before you create the bundle that includes the server SuiteScript.

Note:

Script files that need to be accessed on the client-side cannot have the Hide in SuiteBundle preference enabled. This includes both client scripts and script files that are referenced inside of client scripts.

![File page highlighting Hide in SuiteBundle box.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/HideInSuiteBundle.png)

Important:

Setting the Hide In SuiteBundle preference for a script is the only way to prevent target account users from seeing its code. Locking a bundled file, as described in [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html), only prevents users from editing the script, not from viewing it or downloading it. For a comparison of setting the Hide in SuiteBundle preference and locking a bundled file, see [Locked vs. Hidden Bundle Scripts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380255.html).

#### To prevent bundle installers from seeing server SuiteScript contents: {#procedure_N3377830}

1.  Upload your SuiteScript .js file to the File Cabinet.
    
    For information, see [Uploading Files to Your Account with SuiteCloud Extension for Visual Studio Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161643514921.html) and [Uploading Scripts to the File Cabinet Without SuiteCloud IDEs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0402065535.html#subsect_0403050043).
    
2.  Before you create your bundle, go to _Documents > Files > File Cabinet_.
    
3.  Click the link for the File Cabinet folder where your script is located.
    
    Scripts are usually in the SuiteScripts folder, but may be in another folder.
    
4.  Click **Edit** next to the script you want to protect.
    
5.  Check the **Hide In SuiteBundle** box.
    
6.  Click **Save**.
    

Warning:

You should not check the **Hide In SuiteBundle** box for a script to be included in a bundle developed in sandbox. Checking this box for a script in the source sandbox account for the bundle can eventually lead to the script being hidden in that account. After the bundle is installed in production and the sandbox account is later refreshed, the production account setting for this option is copied to the sandbox account. This copy causes the **Hide in SuiteBundle** box to be checked and disabled in the source sandbox account, preventing bundle developers from accessing the script.

### Related Topics

-   [Bundle Builder Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422668647.html)
-   [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html)
-   [Using Bundle Installation Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377481.html)
-   [Bundle Support during NetSuite Release Phasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382536.html)
-   [Documenting a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380831.html)
-   [Locked vs. Hidden Bundle Scripts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380255.html)
-   [Defining Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381364.html)
-   [File and Folder Management in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381747.html)
-   [Bundling NetSuite Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382176.html)
-   [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html)
-   [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Uploading Files to the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N542268.html)
-   [SuiteApps and Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3405306.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
