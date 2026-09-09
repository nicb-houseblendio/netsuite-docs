---
id: "section_N2495065"
type: "section"
title: "Debug a SuiteScript 1.0 SSP Application"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > SuiteScript 1.0 SSP Applications > Debug a SuiteScript 1.0 SSP Application"
parent: "section_1529595280"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495065.html"
anchors: []
sha256: "8f801a5786e9317b93ca3671eae8287fd209d8018eb4922bbac77acc7bfd83aa"
---

Creating an SSP Application record lets you write debugging details to the script execution log when SSP application scripts run. You'll see these details on the Execution Log subtab of the SSP Application record.

Note:

For more information about SuiteScript 1.0, see [SuiteScript 1.0 Guide.](https://system.netsuite.com/app/help/helpcenter.nl?fid=SuiteScript10.pdf)

Use the SuiteScript API `nlapiLogExecution(type, title, details)` to debug SSP applications written in SuiteScript 1.0. This API requires the following parameters:

-   _type_ {string} \[required\] - One of the following log types:
    
    -   DEBUG (the default when Status is set to Testing)
        
    -   AUDIT
        
    -   ERROR
        
    -   EMERGENCY
        
-   _title_ {string} \[required\] - A title used to organize log entries (max 99 characters). The _title_ argument is required, so you can't set it to _null_ or an empty string.
    
-   _details_ {string} \[optional\] - The log entry details (max 3999 characters)
    

For more details about this API, see the SuiteScript Help.

Note:

Currently, you can't use the SuiteScript Debugger for SSP application scripts.

### Related Topics

-   [Enable Required Features for SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2492346.html)
-   [Create a SuiteScript 1.0 SSP Application Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2493657.html)
-   [Set Execute as Role Permissions for .ss and .ssp Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4589350481.html)
-   [Link a Website or Domain to an SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495714.html)
-   [Remove Touch Points](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3753064405.html)
-   [Change SSP Application Precedence](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496052.html)
-   [Sample SSP Application Code (SuiteScript 1.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538995.html)
-   [SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529595280.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
