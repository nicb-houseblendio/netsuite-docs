---
id: "chapter_N2999784"
type: "chapter"
title: "Referencing Script Parameters"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > Creating Script Parameters (Custom Fields) > Referencing Script Parameters"
parent: "part_1542289448"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999784.html"
anchors: []
sha256: "680810540fff76845696b6fac3aa0977f47104a792e1123894479545f620caed"
---

You can use the [Script.getParameter(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296661592.html) method to reference script parameters that you create. This method is included in the N/runtime module, and you can use other methods in this module to work with scripts and script objects. For example, use [runtime.getCurrentScript()](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296529387.html) to get a [runtime.Script](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296527813.html) object representing your script. For more information, see [N/runtime Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296359529.html).

Before you can reference script parameters in your script, you must create them using the NetSuite UI. To learn how, see [Creating Script Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999459.html). Remember the ID you used (or the ID that was generated automatically for you) when creating a script parameter. Use this ID in your script to get the script parameter's value.

The following example from a Suitelet obtains the value of a script parameter called `custscript_mycheckbox`:

          `// Add a script parameter called Check Box Required var myField = Form.addField({     id: 'custscript_mycheckbox',     label: 'Check Box Required',     type: serverWidget.FieldType.CHECKBOX });  // Obtain an object that represents the current script var myScript = runtime.getCurrentScript();  // Obtain the value of the Check Box Required script parameter var scriptParameterValue = myScript.getParameter({     name: 'custscript_mycheckbox' });` 
        

You cannot write to a script parameter using SuiteScript. You can read from these fields, but not write to them. You can pass a value to a script parameter outside of the UI only when you call [task.create(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4392320106.html) to schedule a script.

For a complete example working with script parameters in a SuiteCloud project, see [Disable Tax Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157174758775.html).

### Related Topics

-   [Creating Script Parameters Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999300.html)
-   [Creating Script Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999459.html)
-   [Script Parameter Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999849.html)
-   [Setting Script Parameter Preferences Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3000000.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
