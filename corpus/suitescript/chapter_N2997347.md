---
id: "chapter_N2997347"
type: "chapter"
title: "Setting Script Execution Log Levels"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Monitoring, Auditing, and Logging > Setting Runtime Options > Setting Script Execution Log Levels"
parent: "chapter_N2996991"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2997347.html"
anchors: []
sha256: "2e0021489b46499ee7d463cb909cd4bcb3060ed0f8fc567c1f76870e7f2e2af2"
---

In the Log Level field on the Script Deployment page, specify which log entries you want to appear on the Execution Log subtab:

![The Script Deployment page setting the Log Level to Debug.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/logLevels.png)

The Log Level field is essentially used as a basic filtering mechanism. Each log entry written with [N/log Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4574548135.html) methods specifies a log level based on the specific method used: [log.audit(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4430384449.html), [log.debug(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4430385329.html), [log.emergency(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4430385611.html), [log.error(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4430385812.html).

Select one of the following log levels from the Log Level field:

-   **Debug**: For scripts in testing mode. Selecting this level will show all log messages (debug, audit, error, and emergency).
    
-   **Audit**: For scripts going into production. Selecting this level will show the events that have occurred during the processing of the script (for example, 'A request was made to an external site.').
    
-   **Error**: For scripts going into production. Selecting this level will show only unexpected script errors.
    
-   **Emergency**: For scripts going into production. Selecting this level will show only the most critical errors in the script log.
    

Important:

NetSuite governs the amount of logging that can be done by a company in any 60 minute time period. For complete details, see [Governance on Script Logging](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352137.html).

Note:

The log level you specify on the Script Deployment page is independent of any error handling within your script.

See [Using the Script Execution Log Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4375896105.html) for details on how to further customize your view of all log entries.

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
