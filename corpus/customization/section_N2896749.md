---
id: "section_N2896749"
type: "section"
title: "Avoid Editing Custom Forms in Tandem"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Deploying Upgraded Forms > Deploying Upgraded Custom Forms > Avoid Editing Custom Forms in Tandem"
parent: "section_N2896089"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896749.html"
anchors: []
sha256: "5d2580cfb1899567e5eda46ced8d9513cc3d1447fd0e7041ab55053621da39e5"
---

You should not simultaneously edit the forms that are currently in use (in your production account) and their corresponding forms accessed through the Upgrade Checklist. For example, you should not edit the layout of **Custom Form A** that is currently used in production, during the time that you also edit the 'preview version' of **Custom Form A** accessible through the Upgrade Checklist. Editing both versions will cause the undeployed preview version to get out of synch with the version in production.

Instead, you should select one version of the form to modify: either the version currently in production, or the (upgraded) undeployed preview version accessed through the Upgrade Checklist.

If you choose to edit the production version, then when you preview the form through the Upgrade Checklist, the preview will show the [Form Layout Enhancements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N472127.html) - as they apply to **ALL** the modifications you have made to the form. Note that if you continue to modify the production version after you have previewed it, the two versions of the form will be out of sync.

If you choose to make all form layout edits to the upgraded/undeployed 'preview' version, you will know that when you are ready to deploy the form, none of the modifications you have made will be lost. This cannot be said of the modifications made to the 'production' version currently in use.

### Related Topics

-   [Deploying Upgraded Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896089.html)
-   [Previewing Undeployed Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896302.html)
-   [Editing the Layout of Custom Forms Prior to Deployment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896507.html)
-   [Testing Undeployed Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896824.html)
-   [Deploying Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2897031.html)
-   [Deploying Skipped Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2897360.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
