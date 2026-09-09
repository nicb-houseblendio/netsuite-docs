---
id: "chapter_N2998873"
type: "chapter"
title: "Setting Script Deployment Status"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Monitoring, Auditing, and Logging > Setting Runtime Options > Setting Script Deployment Status"
parent: "chapter_N2996991"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2998873.html"
anchors: ["bridgehead_N2998933", "bridgehead_N2998993"]
sha256: "d6042506bc277c62b82185ca194609d4e61a621f103fc079c5e003091454a930"
---

A script's deployment status can be set to Testing or Released. When the status is set to Testing, the script will execute for the script owner and specified audience. When the status is set to Released, the script will execute in the accounts of all specified audience members

To set the deployment status, select either Testing or Release from the Status field on the Script Deployment page:

![Script Deployment page setting Status to Testing.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/ScriptDeploymentStatus.png)

Note:

The Testing and Released statuses do not apply to scheduled scripts. To learn about scheduled script deployment statuses, see [Scheduled Script Submission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4658507760.html).

## Status Set to Testing {#bridgehead_N2998933}

When a script's deployment status is set to Testing, only the script owner can execute the script. The script owner can test the script functionality in a different role using the Audience subtab, but the script will not be available for other users until the status is set to Released. For information, see [Using the Audience Subtab to Test Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999041.html#bridgehead_N2999160).

Note that when using the SuiteScript Debugger to test scripts, the script's deployment status must be set to Testing. You cannot debug a Deployed script if the status has been set to Released. (See [Debugging Deployed SuiteScript 1.0 and SuiteScript 2.0 Server Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160418170126.html) and [Debugging Deployed SuiteScript 2.1 Server Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157625777670.html) for more information about using the SuiteScript Debugger to test existing scripts.)

If you are working with Suitelet Script Deployment records, see [Errors Related to the Available Without Login URL](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1524084097.html),to learn how Testing status affects internally and externally available Suitelets.

Note:

A bundle installation script can't execute in target accounts if its deployment status is set to Testing.

## Status Set to Released {#bridgehead_N2998993}

When a script's deployment status is set to Release, the script executes in the accounts of all specified audience members. (See [Defining Script Audience](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999041.html) for information about defining script audiences.) When the deployment status is set to Released, the script is considered to be 'production ready.'

Note that if you do not specify any values on the Audience subtab, the script will execute only for the script owner, even if the script deployment status is set to Released.

Note:

Bundle installation scripts and scheduled scripts do not have an audience. If the deployment status is set to Released for a bundle installation script, the script will execute automatically in target accounts when the associated bundle is installed or updated.

If you are working with Suitelet Script Deployment records, see [Errors Related to the Available Without Login URL](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1524084097.html), to learn how Released status affects internally and externally available Suitelets.

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
