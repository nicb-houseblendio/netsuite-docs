---
id: "section_N3352047"
type: "section"
title: "Monitoring Script Usage"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Governance and Limits > Monitoring Script Usage"
parent: "chapter_N3350651"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352047.html"
anchors: ["subsect_160217718975", "subsect_160217721876"]
sha256: "ad137119124856849b5838a9106fc2516bb87cce30bafaa62bcae9ea05dd2a3d"
---

You can monitor SuiteScript unit usage using the [Script.getRemainingUsage()](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296661153.html) method as shown in the following examples.

## Example 1 {#subsect_160217718975}

This example shows how to instantiate the current script object and call [Script.getRemainingUsage()](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296661153.html) to write the script's remaining usage units to the execution log.

            `var scriptObj = runtime.getCurrentScript(); log.debug({     title: "Remaining usage units: ",     details: scriptObj.getRemainingUsage() });` 
          

## Example 2 {#subsect_160217721876}

This example shows how to instantiate the current script object and checks the remaining usage units. If there are more than 50 usage units remaining, the script will execute a certain set of instructions.

            `var scriptObj = runtime.getCurrentScript(); var unitsRemaining = scriptObj.getRemainingUsage(); if (unitsRemaining > 50) {     //execute code here }` 
          

You can also monitor script unit usage by running the script in the SuiteScript Debugger. After a script completes execution, you can view unit usage details on the Execution Log subtab in the SuiteScript Debugger console. If usage units are exceeded, usage limit error messages are emailed to the script owner indicating the number of usage units that were executed in the script before the usage limit error occurred.

For more information about the SuiteScript Debugger, see the help topic [SuiteScript Debugger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3014215.html).

### Related Topics

-   [SuiteScript Governance and Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3350651.html)
-   [SuiteScript 2.1 API Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157072844224.html)
-   [Script Type Usage Unit Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3351480.html)
-   [Governance on Script Logging](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352137.html)
-   [Search Result Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352288.html)
-   [Script Execution Time Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161591009480.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
