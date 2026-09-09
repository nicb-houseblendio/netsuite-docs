---
id: "section_N3405828"
type: "section"
title: "Two Sandbox Bundle Deployment Model"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApps and Sandbox Accounts > Two Sandbox Bundle Deployment Model"
parent: "chapter_N3405306"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3405828.html"
anchors: []
sha256: "d32396d923c70a4e8f48bf692332be427c8ce6781ddbeb56767675459600162b"
---

If your company has two sandbox accounts, you can dedicate separate sandboxes for development and testing. With this model, you create a bundle in a development (DEV) sandbox, install the bundle in another sandbox for testing (QA), and then deploy the tested bundle from the DEV sandbox into your production account.

Because this model provides a dedicated sandbox account for testing, it ensures that development and testing activities do not interfere with each other. Administrators can continue work on future versions of the bundle or other customizations in the DEV sandbox account at the same time that the bundle is tested in the QA sandbox account.

Important:

If you use a two sandbox model, be sure to deploy from the development sandbox account into production and never from the QA sandbox account. If you deploy from the QA account, the development sandbox account will lose the bundle definition after being refreshed from production.

![Two sandbox install to QA/testing environment and production deployment model.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/TwoSandboxDeploy1.png)

### Related Topics

-   [SuiteApps and Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3405306.html)
-   [Single Sandbox Bundle Deployment Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3405732.html)
-   [Sandbox Refresh Impact on Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3405932.html)
-   [Selective Update of Sandbox Bundle Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770233024.html)
-   [Dissolving Bundles Created in Sandbox](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770244609.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
