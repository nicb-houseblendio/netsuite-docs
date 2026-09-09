---
id: "chapter_N3361671"
type: "chapter"
title: "Scheduled Script Best Practices"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Best Practices > Scheduled Script Best Practices"
parent: "part_N3360914"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361671.html"
anchors: []
sha256: "b12f1e586b534fe3582ad7811ac382f0ed08f6165b570a8d1e9a845739de9058"
---

The following are best practices for scheduled scripts. Also see [Scheduled Script Handling of Server Restarts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1490041886.html).

| General | 
-   **Scheduled** deployments and **Not Scheduled** deployments are executed from the same processor pool. Keep this in mind as you deploy multiple scheduled scripts because the amount of pending script instances is the ultimate bottleneck for scheduled script execution throughput.
-   Create **Not Scheduled** deployments based on the anticipated number of simultaneous calls to this script and approximate execution time of the script.
-   Although there is no restriction on the number of **Not Scheduled** scripts that can be placed into the processing pool, too many pending scripts may create a backlog and compromise system performance. Because only one script can be run in a processor at a time, you shouldn't overload the system.
-   If you want to deploy scheduled scripts that are **scheduled to run hourly on a 24 hour basis**, the following sample values should be set on the Script Deployment page:
    
    -   Deployed = checked
    -   Daily Event = \[radio button enabled\]
    -   Repeat every 1 day
    -   Start Date = \[today's date\]
    -   **Start Time = 12:00 am**
    -   Repeat = every hour
    -   End By = \[blank\]
    -   No End Date = checked
    -   Status = Scheduled
    -   Log Level = Error
    -   Execute as Role = Set to **Administrator**
    
    If the **Start Time** is set to any other time than 12:00 am (for example, set to 2:00 pm), the script will start at 2:00 pm, but then finish its hourly execution at 12:00 am. It won't resume until the next day at 2:00 pm.
-   When possible, schedule your deployments during the hours of 2 AM to 6 AM PST. Deployments scheduled for submission during the hours of 6 AM to 6 PM PST may not run as quickly due to high database activity.

 |
| --- | --- |
| Deployments that continue to use queues | 

-   If you don't have an account with SuiteCloud Plus, all **Scheduled** deployments and **Not Scheduled** deployments that continue to use queues are executed from the same queue. If you deploy multiple scheduled scripts that continue to use queues, your queue size is the ultimate bottleneck for scheduled script execution throughput. For additional information, see [Scheduled Script Deployments that Continue to Use Queues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1508968101.html).
-   Although there is no restriction on the number of **Not Scheduled** scripts that can be submitted to [SuiteCloud Processors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1498571420.html), too many waiting scripts may create a backlog and compromise system performance. Because only one script can be run at a time, you shouldn't overload the system.
-   Although there is no restriction on the number of **Not Scheduled** scripts that can be placed into the processing pool, too many pending scripts may create a backlog and compromise system performance. Because only one script can be run in a processor at a time, you shouldn't overload the system.

 |
| Scheduled script vs Map/Reduce script | 

-   In general, you should use a map/reduce script rather than a scheduled script for any scenario where you want to process multiple records, and where your logic can be separated into relatively lightweight segments. However, a map/reduce script isn't as well suited to situations where you want to enact a long, complex function for each part of your data set.
-   Map/reduce scripts can be run manually or on a schedule, the same as scheduled scripts. However, map/reduce scripts offer several advantages over scheduled scripts. One advantage is that, if a map/reduce job violates certain aspects of NetSuite governance, the map/reduce framework automatically causes the job to yield and its work to be rescheduled, without disruption to the script. However, be aware that some aspects of map/reduce governance can't be handled through automatic yielding.
-   SuiteScript 2.x scheduled scripts don't support recovery points or yielding, so use map/reduce scripts for large data processing. If you need to process a large amount of data or a large number of records, use a map/reduce script instead. The map/reduce script type has built in yielding and can be submitted for processing in the same ways as scheduled scripts.

For information about map/reduce scripts, see [SuiteScript 2.1 Map/Reduce Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799161.html). |

### Related Support Articles

-   [SuiteApp Architectural Fundamentals and Examples (SAFE Guide)](https://suiteanswers.custhelp.com/ci/okcsFattach/getFile/1011960/SuiteAppArchitecturalFundamentalsandExamples.pdf)

### Related Topics

-   [SuiteScript Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/part_N3360914.html)
-   [General Development Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361037.html)
-   [Client Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361924.html)
-   [Map/Reduce Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0801064715.html)
-   [Suitelets and UI Object Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361294.html)
-   [User Event Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361453.html)
-   [Optimizing SuiteScript Performance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460387617.html)
-   [SuiteScript Security Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_159804448843.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
