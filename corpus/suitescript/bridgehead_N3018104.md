---
id: "bridgehead_N3018104"
type: "bridgehead"
title: "Break Points Debugger Subtab"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Debugger > Debugging SuiteScript 1.0 and SuiteScript 2.0 Scripts > Script Debugger Interface > Script Debugger Subtabs > Break Points Debugger Subtab"
parent: "section_N3017822"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3018104.html"
anchors: ["procedure_N3018140"]
sha256: "a7006c8a80d44eeb8a6db27ffd0427784517f45f4db288ae8b481bb8fd215b8c"
---

Note:

The Break Points subtab isn't used for SuiteScript 2.1 scripts. SuiteScript 2.1 script logging is done on the Chrome DevTools debugger console. For more information about debugging SuiteScript 2.1 scripts, see [Chrome DevTools for SuiteScript 2.1 Script Debugging](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157625775882.html).

The Break Points subtab shows all your instruction-level (line) break points as well as your user event break points. You can add user event break points by selecting user events from the Break on User Event list.

![The Script Debugger Break Points tab.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/breakpoints.png)

You can set break points in your code using the Script Debugger code window. By setting breakpoints, you can run your code up to a certain point, and then halt the execution at the break point and examine the current state of the execution.

#### To add or remove break points in your code: {#procedure_N3018140}

1.  Click between the line number and the line of code to add a breakpoint:
    
    ![The Script Debugger with a break point on a log.debug statement.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/debugger_setBreakpoint.png)
2.  To remove a break point, click the break point icon as it appears in the code. You can also remove a break point by clicking the red **x** icon next to the break point, as it appears on the **Break Points** tab.
    
    When you debug deployed scripts, you can set break points at each user event in your script. User events possibly invokable during script execution where the program halts execution.
    

### Related Topics:

-   [Script Debugger Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3017822.html)
-   [Execution Log Debugger Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3017916.html)
-   [Local Variables Debugger Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3017956.html)
-   [Watches Debugger Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3017995.html)
-   [Evaluate Expressions Debugger Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3018068.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
