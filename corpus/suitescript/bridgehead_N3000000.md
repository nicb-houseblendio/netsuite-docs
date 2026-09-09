---
id: "bridgehead_N3000000"
type: "bridgehead"
title: "Setting Script Parameter Preferences Example"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > Creating Script Parameters (Custom Fields) > Script Parameter Preferences > Setting Script Parameter Preferences Example"
parent: "chapter_N2999849"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3000000.html"
anchors: []
sha256: "8e392065e8f0968580eca2fd078aa68aa6f2dbaa83a96c8082e496e184393a19"
---

In this example, the Suitelet script includes a parameter called **Check Box Required** (with the internal ID _custscript\_checkboxtest2_ ), which is set to the Company preference.

![The Script record page Parameters tab with the Preference parameter highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/definingParameters.png)

By going to _Setup > Company > General Preferences_ on the Custom Preferences subtab, administrators can set the default value of this parameter for the entire company. In this example, the value of the **Check Box Required** script parameter is set to T (True, or box checked).

![The Custom Preferences tab with Check Box Required checked.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/checkboxSetCompany.png)

When the Suitelet that contains this box is deployed, **Check Box Required** is checked.

![A Simple Form page with the Check Box Required field highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/checkboxAdded.png)

If the **Check Box Required** parameter had been set to F (False, or box not checked), the box would have been cleared on the form when the Suitelet was deployed.

Note:

To create a script parameter, see [Creating Script Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999459.html). For information about accessing script parameter values, see [Referencing Script Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999784.html).

### Related Topics

-   [Creating Script Parameters Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999300.html)
-   [Script Parameter Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999849.html)
-   [Script Parameter Preference Updates in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3000106.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
