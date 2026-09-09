---
id: "bridgehead_N3017956"
type: "bridgehead"
title: "Local Variables Debugger Subtab"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Debugger > Debugging SuiteScript 1.0 and SuiteScript 2.0 Scripts > Script Debugger Interface > Script Debugger Subtabs > Local Variables Debugger Subtab"
parent: "section_N3017822"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3017956.html"
anchors: []
sha256: "6379d651b0b6ba36f0592ade17a550e7a431f2ad56c608ce788d20a8f77ed3bf"
---

Note:

The Local Variables subtab iisn't used for SuiteScript 2.1 scripts. Logging of SuiteScript 2.1 scripts is done on the Chrome DevTools debugger console. See [Chrome DevTools for SuiteScript 2.1 Script Debugging](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157625775882.html) for more information about debugging SuiteScript 2.1 scripts.

The Local Variables subtab shows a list of all local variables (primitives, objects, and NetSuite objects) currently in scope. Note that for NetSuite objects, all properties are private, even though they can be seen on the Local Variables subtab. Don't try to reference these properties directly in your script. Use the appropriate getter/setter functions instead.

The Local Variables subtab includes a call stack that shows the current execution stack of the script. The function call and current line number for that function are included in the list. Use the Call Stack list to switch between call stacks to view different local variables. In addition, watch expressions and expression evaluations are automatically performed in the context specified by this field.

Important:

Due to performance considerations, the display limit for all variables is 1000. In addition, only the first 500 characters of a String are displayed. For large variables, use a watch to see the full member display (see [Watches Debugger Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3017995.html) for additional information).

![A sample script being debugged with a breakpoint set on a variable assignment statement and the same variable displayed on the Local Variables tab.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/localvariables.png)

### Related Topics:

-   [Script Debugger Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3017822.html)
-   [Execution Log Debugger Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3017916.html)
-   [Watches Debugger Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3017995.html)
-   [Evaluate Expressions Debugger Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3018068.html)
-   [Break Points Debugger Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3018104.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
