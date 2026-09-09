---
id: "section_N3352137"
type: "section"
title: "Governance on Script Logging"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Governance and Limits > Governance on Script Logging"
parent: "chapter_N3350651"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352137.html"
anchors: ["subsect_156355789462", "subsect_156355399752"]
sha256: "2cce2696d9e001efb8dcf17320920547fe00e354f187f2c53155ebb088e51d03"
---

NetSuite governs the amount of script execution logging that can be done. The governance model is:

-   A company can make up to 100,000 N/log calls across all scripts within a 60-minute period.
    
-   System error logs are purged after 60 days. User-generated logs are purged after 30 days.
    

Use the [N/log Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4574548135.html) methods to log script execution details.

Script owners are notified if a script is logging excessively and NetSuite automatically adjusts the log level.This keeps the script running and prevents it from logging too much. For example, say one company has 10 scripts running during a 60-minute period. If one script makes 70,000 [log.debug(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4430385329.html) calls within each 20-minute period, NetSuite will automatically raise the script's log level.

You can see the new log level in the Log Level field on the script's deployment page:

![Script Deployment page with Log Level of Audit highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/logLevelChange.png)

For example, if the offending script's log level was originally set to Debug, NetSuite will increase the level to Audit. This means that the `log.debug` line of code will continue to execute, however, nothing will be logged, because the log level for the script has been raised to Audit and the line of code is using the Debug level. For more information about log levels, see the help topic [Using Log Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4574548135.html#bridgehead_4546180151). For more information about viewing script execution logs, see the help topic [Script Execution Logs](#subsect_156355789462).

For more information, see [N/log Module Guidelines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4574548135.html#bridgehead_4430315777).

## Script Execution Logs {#subsect_156355789462}

All script execution logs in NetSuite are stored for up to 30 days. You can view script execution logs using the Execution Log subtab, using a Server Script Log search, or using the Script Execution log page. Details are shown in the following table:

| Access to Script Execution Logs | Details |
| --- | --- |
| Execution Log subtab on script and script deployment records | The capacity for script execution logs on the Execution Log subtab is shared by customers on the same NetSuite database. To prevent excessive logging, there's a 5 million log limit per database instance. If this limit is reached, all logs for all customers on that database are purged. If you need to view all logs up to 30 days on the Execution Log subtab, consider creating a custom solution using custom records to store log information from logs. For more information, see the help topic [Using the Script Execution Log Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4375896105.html). |
| Server Script Log search | The capacity for script execution logs returned by the Server Script Log search is shared by all customers on the same NetSuite database. To prevent excessive logging, script execution logs are governed by a total storage limit of 5 million log limit per database instance for this search. On each NetSuite server, if this limit is reached, logs across all customers on that server are purged. If you need to search all logs up to 30 days, consider creating a custom solution using custom records to store log information from logs. If a Server Script Log search is not returning logs less than 30 days old, go to _Customization > Scripting > Script Execution Logs_ and use the filters at the top of the Script Execution Log page to search for logs. You can also check script deployments that have large amounts of logging and consider lowering the Log Level to Error or Emergency or limiting the number of log lines in your script. |
| Script Execution log page | The execution logs shown on the Script Execution log page are stored for 30 days regardless of volume. For more information about the Script Execution log, see the help topic [Viewing a List of Script Execution Logs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4375937190.html). |

## Script Owner Notifications {#subsect_156355399752}

If NetSuite detects that a script is logging excessively, the owner of the script is notified that the script is logging excessively and could possibly exceed the 100,000 logging threshold (for a 60-minute time period).

NetSuite sends email notifications and adds a log entry to the script's Execution Log indicating that a script's log level has been increased. For more information about script execution log levels, see the help topic [Setting Script Execution Log Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2997347.html).

### Related Topics

-   [SuiteScript Governance and Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3350651.html)
-   [SuiteScript 2.1 API Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157072844224.html)
-   [Script Type Usage Unit Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3351480.html)
-   [Monitoring Script Usage](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352047.html)
-   [Search Result Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352288.html)
-   [Script Execution Time Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161591009480.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
