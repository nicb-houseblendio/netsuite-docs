---
id: "chapter_N2997500"
type: "chapter"
title: "Executing Scripts Using a Specific Role"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Monitoring, Auditing, and Logging > Setting Runtime Options > Executing Scripts Using a Specific Role"
parent: "chapter_N2996991"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2997500.html"
anchors: []
sha256: "3fca370075d57d4e9f11c1a88eaf4bcc73eb5733da295e727421887ebda95423"
---

The **Execute as Role** field sets which role's permissions uses at runtime. It lists all standard and custom roles, plus Current User, which runs the script with the logged-in user's permissions. For example, if you choose Sales Person, the script always runs with that role's permissions-even if an Administrator triggers it. If no existing role fits, create a custom one with the needed permissions and choose it instead.

![The Script Deployment page setting Execute As Role field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/executeAsRole.png)

Important:

Keep these behaviors in mind:

-   When one script triggers another, the triggered script runs with the first script's role-not the role set on its own deployment.
    
-   When you're testing, set the deployment status to **Testing** so the script runs only for you and the selected role; other users won't trigger it.
    

For more details on roles in script deployments, see the following topics:

-   [Script Types That Support Execute as Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1212112429.html)
    
-   [Setting Your Script to Run With Administrative Privileges](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2997678.html)
    

For an overview of roles and permissions in SuiteScript, see [Setting Roles and Permissions for SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0403053450.html). For limits that are specific to client scripts, see [Client Script Role Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1512507167.html).

### Related Topics:

-   [Setting Runtime Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2996991.html)
-   [Setting Roles and Permissions for SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0403053450.html)
-   [Client Script Role Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1512507167.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
