---
id: "bridgehead_N3017995"
type: "bridgehead"
title: "Watches Debugger Subtab"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Debugger > Debugging SuiteScript 1.0 and SuiteScript 2.0 Scripts > Script Debugger Interface > Script Debugger Subtabs > Watches Debugger Subtab"
parent: "section_N3017822"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3017995.html"
anchors: []
sha256: "df1c745f4f87e035b8ca6602043b78ef1658e987f1d647884e4ba79f0bdfe81a"
---

Note:

The Watches subtab isn't used for SuiteScript 2.1 scripts. Variable watches in SuiteScript 2.1 scripts are done on the Chrome DevTools debugger console. For more information about debugging SuiteScript 2.1 scripts, see [Chrome DevTools for SuiteScript 2.1 Script Debugging](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157625775882.html).

The Watches subtab lets you add or remove variables and expressions to a list that's kept up-to-date ("watched") during the time that your script executes.

![The Script Debugger Watches tab.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/watchvariables.png)

The variables and expressions are always evaluated in the current call stack. This means that by default, they're evaluated at the current line of script execution. However, if you switch to a different function in the call stack, they're re-evaluated at that location.

-   To add a variable or an expression, type it into the **Add Watch** field and press the Enter key.
    
-   To remove a watched variable or expression, click on the red **x** icon to the left of the expression.
    
-   To browse sub-properties of a user-defined object, an array, or a NetSuite object expression, click the expand/collapse icon next to the property name.
    

You can also use the Watches subtab to view object properties with a command-line interface. Any property that is viewable from the property browser can be added as a watch expression by referencing the property using dot ( . ) notation, even if the property is private in the script. For example, to watch the ID of a record object (referenced by a variable called _record_), type record._id_ in the **Add Watch** field.

### Related Topics:

-   [Script Debugger Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3017822.html)
-   [Execution Log Debugger Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3017916.html)
-   [Local Variables Debugger Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3017956.html)
-   [Evaluate Expressions Debugger Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3018068.html)
-   [Break Points Debugger Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3018104.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
