---
id: "section_N3351480"
type: "section"
title: "Script Type Usage Unit Limits"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Governance and Limits > Script Type Usage Unit Limits"
parent: "chapter_N3350651"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3351480.html"
anchors: []
sha256: "cc78c303a1c7a3ab864bd038434a50d941dd3d5dbf034548b6c10635306da7e9"
---

The following table lists the maximum allowable usage units for each SuiteScript (1.0 and 2.1) script type. You can use the [Script.getRemainingUsage()](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296661153.html) method to see how many usage units you have remaining for a particular script.

| Script Type | Total usage units Allowed per Script | Notes |
| --- | --- | --- |
| Bundle Installation Scripts (SuiteScript 1.0) [SuiteScript 2.1 Bundle Installation Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460460309.html) | 10,000 | The limit is 10,000 usage units per execution. |
| Client Scripts (SuiteScript 1.0) [SuiteScript 2.1 Client Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387798404.html) | 1,000 | Client scripts are metered on a per-script basis. If an account has one form-level client script attached to a form and one record-level client script deployed to a record (which may be associated with a form), each client script can total 1,000 usage units. Usage units are not shared by all the client scripts associated with a form or record. For information about record- and form-level client scripts, see [Record-Level and Form-Level Script Deployments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4576055055.html). |
| [SuiteScript 2.1 Custom Tool Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1185045525.html) | 1,000 | The limit is 1,000 usage units per execution of the tool. |
| [SuiteScript 2.1 Event Subscriber Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_8125656702.html) | 1,000 | The limit is 1,000 usage units per execution of the script. |
| [SuiteScript 2.1 Map/Reduce Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799161.html) | \- | Map/reduce scripts are not available in SuiteScript 1.0. There are no limits imposed on the full duration of a map/reduce script deployment instance. Instead, isolated components of the deployment, such as the usage units used by a single method invocation, are regulated. For more information, see [Map/Reduce Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4480364878.html). |
| Mass Update Scripts (SuiteScript 1.0) [SuiteScript 2.1 Mass Update Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460452911.html) | 1,000 | The limit is 1,000 usage units per record or execution of the script. |
| Portlet Scripts (SuiteScript 1.0) [SuiteScript 2.1 Portlet Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799288.html) | 1,000 | \- |
| RESTlets (SuiteScript 1.0) [SuiteScript 2.1 RESTlet Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799403.html) | 5,000 | The SuiteScript governance model for RESTlets tracks usage units on the API level and the script level. For more information, see the help topic [RESTlet Governance and Security](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4640094112.html) |
| Scheduled Scripts (SuiteScript 1.0) [SuiteScript 2.1 Scheduled Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799491.html) | 10,000 | Within one scheduled script, all actions combined cannot exceed 10,000 usage units. For example, a scheduled script that includes two calls to [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html) and one call to [email.send(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4358681681.html) consumes from 24 to 40 usage units (depending on the record type for [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html)) out of a possible 10,000 usage units available. If you have a scheduled script with potentially long execution times, you should consider using a map/reduce script instead. SuiteScript 2.1 does not have a method to allow you to set recovery points or provide a yield to avoid exceeding the allowed governance for a scheduled script. A map/reduce script has built-in yielding and can be submitted for processing in the same ways as a scheduled script. |
| [SuiteScript 2.1 SDF Installation Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1544719586.html) | 10,000 | The limit is 10,000 usage units per execution. |
| Suitelets (SuiteScript 1.0) [SuiteScript 2.1 Suitelet Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799600.html) | 1,000 | Within one Suitelet, all actions combined cannot exceed 1,000 usage units. For example, a Suitelet that calls [record.create(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258059.html) and [http.get(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4426024767.html) consumes from 12 to 20 usage units (depending on the record type for [record.create(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258059.html)) out of a possible 1,000 usage units available. Regardless of the 1,000 unit limit for Suitelets, you should create your Suitelets to be responsive to users, otherwise user experience may be impacted. |
| User Event Scripts (SuiteScript 1.0) [SuiteScript 2.1 User Event Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799721.html) | 1,000 | Regardless of the 1,000 usage unit limit for user event scripts, you should create your scripts so that they are responsive to users, otherwise user experience may be impacted. |
| Workflow Action Scripts (SuiteScript 1.0) [SuiteScript 2.1 Workflow Action Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460429314.html) (also referred to as [Custom Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2752089.html) in SuiteFlow) | 1,000 | Within one workflow state, all actions combined cannot exceed 1,000 usage units. For example, if you have developed a custom action (using a workflow action script) that consumes 990 usage units, be aware of the unit consumption of the other actions within that state. |
| [Core Plug-ins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_4616046155.html) | Varies based on the plug-in | The default limit for core plug-ins that do not have more restrictive limits defined is 10,000. See the help topic for each core plug-in for any specific usage unit limits. |
| [Custom Plug-ins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_4060648050.html) | 10,000 | The limit is 10,000 usage units per plug-in. |
| SSP Application Scripts | 1,000 | For more information, see [SSP Application Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538501.html). |

Note:

There is also a limit of 1,000 usage units when using the [SuiteScript Debugger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3014215.html). For more information, see [Script Debugger Metering and Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3018263.html).

### Related Topics

-   [SuiteScript Governance and Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3350651.html)
-   [SuiteScript 2.1 API Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157072844224.html)
-   [Monitoring Script Usage](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352047.html)
-   [Governance on Script Logging](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352137.html)
-   [Search Result Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352288.html)
-   [Script Execution Time Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161591009480.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
