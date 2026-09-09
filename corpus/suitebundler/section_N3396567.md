---
id: "section_N3396567"
type: "section"
title: "Starting the Bundle Installation Process"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Installation and Update > Installing a Bundle > Starting the Bundle Installation Process"
parent: "section_N3395142"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3396567.html"
anchors: []
sha256: "6f074240e8a375f5cf0833bb2d44da227b769724212411114ddb4529515c5e1c"
---

After you've started installing a bundle by clicking **Install Bundle** on the Preview Bundle Install page, the Installed Bundles page appears.

-   If the installation isn't finished, the **Status** column shows the percentage of progress.
    
-   If the installation is done, the **Status** column shows a green check.
    

The time required to install the bundle depends on the size of the bundle. You can continue work in NetSuite during the time that the bundle installs.

Warning:

Enabling the **Include Data** option for a bundled custom record object with an extremely large number of custom records may result in bundle installation failure due to network connection problems. To ensure installation success, do not enable the **Include Data** option for the custom record object. Then run a bundle installation script that executes after installation to import custom record object data into the target account through CSV import. For information, see [SuiteScript 2.1 Bundle Installation Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460460309.html) and [task.CsvImportTask](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345798668.html).

You can go back to the Installed Bundles page and check the status of the bundle installation later, at _Customization > SuiteBundler > Search & Install Bundles_. See [Reviewing the Installed Bundles List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3397033.html).

### Related Topics

-   [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html)
-   [Choosing a Bundle to Install](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395426.html)
-   [Reviewing the Preview Bundle Install Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3396121.html)
-   [Bundle Installation Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3396757.html)
-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [Resolving Conflicting Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394371.html)
-   [Bundle Searches Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3394713.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
