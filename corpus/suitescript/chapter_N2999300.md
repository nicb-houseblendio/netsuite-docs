---
id: "chapter_N2999300"
type: "chapter"
title: "Creating Script Parameters Overview"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > Creating Script Parameters (Custom Fields) > Creating Script Parameters Overview"
parent: "part_1542289448"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999300.html"
anchors: []
sha256: "9181bfc50d8e8f4761667e58d47d27909eca699395f0095c41750dab3412a1f4"
---

In the context of SuiteScript, script parameters are similar to custom fields; they are not considered to be parameters that are passed between JavaScript functions. Script parameters share characteristics with custom fields created through point-and-click customization. Script parameters are configurable by administrators and the users of your Suite App, and are accessible programmatically through SuiteScript. Script parameters are defined on the Parameters subtab of the Script record page.

Warning:

Do not include confidential information in script parameters. Information saved in script parameters can be indexed by search engines and therefore be viewable by the public. This means, for example, that the information could be found in Google searches.

You should create script parameters in the following situations:

-   You want part of your script to be configurable, either through script deployment or by the users of your SuiteApp. You do not need to create script parameters if your script is not designed to be configurable.
    
-   You need to parameterize a script that was deployed multiple times. This approach makes it more convenient to customize the behavior of the script for each deployment.
    
-   You want to configure a scheduled script. You're able to do this by specifying configuration parameters as arguments to [task.create(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4392320106.html).
    

The advantages of using script parameters include:

-   With deployment-specific parameters, you can configure script behavior without writing code. These parameters are useful when administrators deploy scripts that were installed as part of a bundle. The parameters let administrators to control or modify the script without knowing anything about the code. Deployment-specific parameters are similar to property or configuration files that some applications use to modify behavior at runtime.
    
-   Script parameters let you to modify script behavior for troubleshooting without changing code, which is often expensive and not feasible (for example, if the original script author is unavailable).
    
-   Script parameters provide flexibility to handle various inputs based on context. For example, consider a situation in which one script is deployed to 50 different records, but requires slightly different behavior for each record. You could hard-code and deploy 50 different scripts, but they may be difficult to maintain because the code isn't configurable, code might be duplicated unnecessarily, and changes in business requirements likely require code changes.
    

For more information, see the following help topics:

-   [Creating Script Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999459.html)
    
-   [Referencing Script Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999784.html)
    
-   [Script Parameter Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999849.html)
    
-   [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html)
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
