---
id: "bridgehead_N3000106"
type: "bridgehead"
title: "Script Parameter Preference Updates in Bundles"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > Creating Script Parameters (Custom Fields) > Script Parameter Preferences > Script Parameter Preference Updates in Bundles"
parent: "chapter_N2999849"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3000106.html"
anchors: []
sha256: "8c6943274077abafa1c013fb069fdf7b91dfe341e407229c0c73b8c271eed95c"
---

Script parameters that have a user or company preference set are not updated in target accounts when the bundle is updated. Script parameters without a preference are part of the script deployment and are updated in target accounts based on the bundle object preference:

-   With Update Deployments, script deployment parameters in target accounts are updated to match the source account.
    
-   With Do Not Update Deployments, script deployment parameters in target accounts remain unchanged.
    

Set the preference to Company or User if target account users need to change parameter values. Users can change parameter values as needed, and these changes won't be overwritten on bundle update even if the related bundle object preference is set to Update Deployments.

To prevent changes, set the bundle object preference to Do Not Update Deployments for parameters without a preference.

For more information, see [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html).

### Related Topics

-   [Creating Script Parameters Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999300.html)
-   [Script Parameter Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999849.html)
-   [Setting Script Parameter Preferences Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3000000.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
