---
id: "section_N3380255"
type: "section"
title: "Locked vs. Hidden Bundle Scripts Overview"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Bundle Builder Reference > Protecting Your Bundled Server SuiteScripts > Locked vs. Hidden Bundle Scripts Overview"
parent: "section_N3377764"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380255.html"
anchors: []
sha256: "7de43c44a0237d5dafcf9d5e16ff102438e219128c587b2c2c8b60ee25de14e4"
---

You can do the following to limit user access to objects installed by bundles in target accounts:

-   In the Bundle Builder, you can lock objects so that users in target accounts cannot edit them. However, users can still view locked objects, including scripts. See [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html).
    
-   In the Bundle Builder, you can enable the Hide Components option so that by default, objects installed by the bundle are not displayed on list pages in target accounts. See [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html). This setting is a default, however, that can be overridden by any target account administrator. When an administrator disables the Hide Components option, users can see all bundled objects in list pages.
    
-   In the File Cabinet, you can enable the Hide in SuiteBundle option for a server SuiteScript included in a bundle. See [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html). Enabling this option is the only way to ensure that target account users cannot view the code in a script and cannot be set for scripts that will be accessed on the client side.
    

You can use any or all of these options. To understand the combined effects of locking and setting the Hide in SuiteBundle option for a script, see the following table.

| Locked? | Hide in SuiteBundle option enabled? | Effect in Target Accounts |
| --- | --- | --- |
| No | No | User can view and edit both the script and its NetSuite file record, and can download the script file. |
| No | Yes | User cannot view, edit, or download the script file, but can view and edit the file record. |
| Yes | No | User can view both the script and the file record, and download the script file, but cannot edit the script or file record. |
| Yes | Yes | User cannot view, edit, or download the script file, and cannot view or edit the file record. This preference will cause a validation error on client scripts or on scripts that are referenced from client scripts. |

### Related Topics

-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html)
-   [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html)
-   [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
