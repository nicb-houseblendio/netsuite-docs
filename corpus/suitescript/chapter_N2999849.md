---
id: "chapter_N2999849"
type: "chapter"
title: "Script Parameter Preferences"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > Creating Script Parameters (Custom Fields) > Script Parameter Preferences"
parent: "part_1542289448"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999849.html"
anchors: []
sha256: "b701c89702b2223d62e766669b7d88cb7576fc48ad34e40b071de98e8987069a"
---

When you use script parameters, you can specify a preference type. Available preference types are Company and User or you can choose not to set a preference.

-   **Company:** For Company preference, the parameter's value comes from the value set in _Setup > Company > General Preferences_ on the Custom Preferences subtab. For an example, see [Setting Script Parameter Preferences Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3000000.html).
    
-   **User:** For User Preference, the parameter's value comes from the value set in _Home > Set Preference_ on the Custom Preferences subtab. This lets end users override the company default script behavior and set their own default value. End users can change script parameter values without modifying the script or its deployments.
    

![The Script record page Parameters tab with the Company preference selected.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/checkboxCompanyPref2.png)

If you don't set a preference, the script parameter is considered a "deployment" script parameter by default. In this case, you define the value of the script parameter on the Parameters subtab of the Script Deployment record.

![The Script Deployment page with the Parameters tab fields highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/scriptParametersNoPreference.png)

Note that users who install a bundled script that uses preferences can override the default behavior of the script and customize the script to their specific business needs. Setting preferences eliminates having to manipulate the script code or the script deployment. For more information, see [SuiteBundler Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3363483.html) and [Script Parameter Preference Updates in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3000106.html).

### Related Topics

-   [Creating Script Parameters Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999300.html)
-   [Setting Script Parameter Preferences Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3000000.html)
-   [Script Parameter Preference Updates in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3000106.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
