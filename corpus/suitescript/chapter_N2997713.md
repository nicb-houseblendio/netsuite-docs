---
id: "chapter_N2997713"
type: "chapter"
title: "Setting Available Without Login"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Monitoring, Auditing, and Logging > Setting Runtime Options > Setting Available Without Login"
parent: "chapter_N2996991"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2997713.html"
anchors: []
sha256: "8c0bfe18ff8d24f2b6c899518369df09883ddbc7d6559e58035acaa41d49e38a"
---

You can allow Suitelet scripts to be executed without a login. Select the Available Without Login box on the Script Deployment page give users access to the Suitelet even if they're not logged in.

Warning:

Suitelets configured as available without login should not be used in integration use cases, including SDN partner SuiteApps. Suitelets configured as available without login are a violation of Built for NetSuite (BFN) standards.

To ensure that users without an active NetSuite session can access the Suitelet, **Online Form User** must be selected in the External Roles field. All other roles that require access to the script should also be selected in the Internal Roles and External Roles fields. Values from the Departments, Groups, Employees, and Partners fields must be cleared.

Note:

The Available Without Login box is available on the Script Deployment page for Suitelets only. When working with Client Scripts and externally available Suitelets, the Website feature must be enabled.

To be able to select the **Online Form User** role in the External Roles field, the Online Forms feature must be enabled. To enable the feature, go to Setup > Company > Enable Features. Click the CRM subtab, and check the **Online Forms** box in the Marketing section. If the role is still not available after enabling the feature, you may need to log out and log back in to see the updated roles list.

![The Script Deployment page setting Available Without Login.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/availableWithoutLoginSuitelet2.png)

The following are some uses cases when you might want to make a Suitelet externally available (however, when considering these use cases, keep in mind that using Suitelets externally without login is forbidden in BFN):

-   Hosting one-off online forms (for example, capturing partner conference registrations).
    
-   Inbound partner communication (such as, listening for payment notification responses from PayPal or Google checkout, or for generating an unsubscribe request from email campaigns page, which requires access to account information but should not require a login or hosted website).
    
-   For Facebook, Google, and Yahoo mashups in which the Suitelet lives in those websites but needs to communicate to NetSuite using POST requests.
    

Important:

Note that the data contained within the Suitelet will be less secure when it is allowed to be accessed (using Suitelet execution) without login.

For information about errors when using the Available Without Login URL, see [Errors Related to the Available Without Login URL](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1524084097.html).

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
