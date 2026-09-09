---
id: "chapter_N3361453"
type: "chapter"
title: "User Event Script Best Practices"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Best Practices > User Event Script Best Practices"
parent: "part_N3360914"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361453.html"
anchors: []
sha256: "f562119eb3bee0bd6c9ac69570e59af788f16c39bafca12e5bdf633170d4d63d"
---

The following are best practices for developing user event scripts.

| General | 
-   For critical business logic, use a scheduled script to clean up after user events in case of errors.
-   Don't try to run a user event script from another one - instead, create a module with common code.
-   Make sure that the user event script doesn't access any sensitive field values.

 |
| --- | --- |
| Context | 

-   Use the `type` argument, the `context` object, and `context.UserEventType` enum to define and limit the scope of your user event logic. See [context.UserEventType](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4407992596.html).

 |
| Entry points | 

-   For operations that depend on on the submitted record being committed to the database should happen in an `afterSubmit` script.
-   When updating transaction line items in a `beforeSubmit` script, ensure that the line item totals, net taxes, and discounts are equal to the `summarytotal`, `discounttotal`, `shippingtotal`, and `taxtotal` amounts.
-   Avoid assigning too many functions to one record type, as it can slow things down. This could negatively affect the user experience with that record type. For example, if there are ten `beforeLoad` scripts that must complete their execution before the record loads into the browser, the time needed to load the record may increase significantly. Be aware of the number of user events scripts used, including bundled user event scripts.
-   Use beforeSubmit to update fields or change the record before it's submitted.
-   Perform all post-processing operations of the current record on an `afterSubmit` event.

 |
| Storing values | 

-   If you want to store a value during a `beforeLoad` operation and then read that value during an `afterSubmit` operation in the same script, consider using a hidden custom field to store the value. You can add a hidden custom field to the form and store your value during the `beforeLoad` operation, and you can retrieve the value from the same field during the `afterSubmit` operation.

 |
| Execution contexts | 

-   Use execution context filtering to control how and when a user event script is executed. Execution contexts provide information about how a script is triggered. For example, a script can be triggered in response to an action in the NetSuite application, or an action occurring in another context, such as a web services integration. You can use execution context filtering to ensure that your scripts are triggered only when necessary. For more information, see [Execution Contexts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157960743044.html).

 |
| Performance | 

-   Try to keep user event script execution under 5 seconds, as they run frequently. You can use the Application Performance Management (APM) SuiteApp to test the performance of your scripts deployed on a specific record type. See [Application Performance Management (APM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4283522055.html).

 |
| Debugging | 

-   To debug a client script, include a debugger; statement as the first line in the script. When execution reaches that statement, you can examine your script properties and variables using the debugging tools in your browser. You can also use the `debugger;` statement in the SuiteScript Debugger to help you debug server scripts. For more information about the SuiteScript Debugger, see [SuiteScript Debugger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3014215.html).

 |
| Hosted websites | 

-   Activities (user events) on a hosted website can trigger server SuiteScripts. In addition to sales orders, scripts on case records and customer records also run in response to web activities.

 |

### Related Support Articles

-   [SuiteApp Architectural Fundamentals and Examples (SAFE Guide)](https://suiteanswers.custhelp.com/ci/okcsFattach/getFile/1011960/SuiteAppArchitecturalFundamentalsandExamples.pdf)

### Related Topics

-   [SuiteScript Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/part_N3360914.html)
-   [General Development Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361037.html)
-   [Client Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361924.html)
-   [Map/Reduce Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0801064715.html)
-   [Scheduled Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361671.html)
-   [Suitelets and UI Object Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361294.html)
-   [Optimizing SuiteScript Performance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460387617.html)
-   [SuiteScript Security Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_159804448843.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
