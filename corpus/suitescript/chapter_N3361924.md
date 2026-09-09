---
id: "chapter_N3361924"
type: "chapter"
title: "Client Script Best Practices"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Best Practices > Client Script Best Practices"
parent: "part_N3360914"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361924.html"
anchors: []
sha256: "96a0e5e58acb3c394dc93d57c434d87a5b8566f871126a5c630fc8f766fd208d"
---

The following are best practices for both form-level and record-level client SuiteScript development.

| General | 
-   Use global (record-level) client scripts for more flexible deployment models (include in a bundle or SuiteCloud project) than client scripts attached to forms.

 |
| --- | --- |
| Using Record.setValue and Record.setCurrentSublistValue methods | 

-   [Record.setValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4273155868.html) and [Record.setCurrentSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4273171484.html) execution is multi-threaded whenever child field values need to be sourced in. To synchronize your logic, use the `postSourcing` function or set the `forceSyncSourcing` synchronous parameter to `true`.

 |
| Advanced Employee Permissions | 

-   When the Advanced Employee Permissions feature is enabled, the search columns available to users also depends on the permissions assigned to the role.
-   When the Advanced Employee Permissions feature is enabled, the fields and sublists a user has access to can change depending on which employee is being viewed or edited. This is different from other records in NetSuite, where permissions granted to a role determines what the role can see for every instance of that record. In general, scripts should always verify that a field exists before trying to do something with it. Simply calling functions and methods that interact with fields before checking whether the field is there may result in inconsistent behavior. For example, the department field is permitted on the employee record. When you verify that the field exists and you don't have access, a null value is returned, and if the field is empty, an empty string is returned. Unsafe Practice Example `var employeeRecord = record.load ({ type: record.Type.EMPLOYEE, id: 115 }); employeeRecord.setValue({ fieldId: 'department', value: 'marketing' }); employeeRecord.save();` Safe Practice Example To detect if your role has access to a field for a specific employee, load the employee record object and call `getFields()`. If the field exists and you do have access a `true` value is returned. In the below example, the user has access to the department field for the employee with ID: 115. `var employeeRecord = record.load ({ type: record.Type.EMPLOYEE, id: 115 }); var accessToDepartment = employeeRecord.getFields().includes('department');`

 |
| Editing sublists | 

-   When you are editing the current line of a sublist and a nested client script is triggered (for example, when a `fieldChanged` script is triggered by changing a value in the current sublist line), make sure that the nested script doesn't select a different line of the same machine as the current line. Otherwise, the changes made in the parent script may be lost.

 |
| Execution contexts | 

-   Use execution context filtering to specify how and when a client script is executed. Execution contexts provide information about how a script is triggered to run. For example, a script can be triggered in response to an action in the NetSuite application, or an action occurring in another context, such as a web services integration. You can use execution context filtering to ensure that your scripts are triggered only when necessary. For more information, see [Execution Contexts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157960743044.html).

 |
| setValue and setText methods | 

-   Methods that set values accept raw data of a specific type and don't require formatting or parsing. Methods that set text accept strings but can conform to a user-specified format. For example, when setting a numeric field type, `setValue()` accepts any number, and `setText()` accepts a string in a specified format, such as '2,000.39' or '2.00,39'. When setting a date field type, `setValue()` accepts any `Date` object, and `setText()` accepts a string in a specified format, such as '6/9/2016' or '9/6/2016'.

 |
| Debugging | 

-   When debugging client scripts, you can insert a `debugger;` statement in your script, and execution will stop when this statement is reached: `function runMe() { var k = 1; k *= (k + 9); debugger; console.log(k); }` When your script stops at the `debugger;` statement, you can examine your script properties and variables using the debugging tools in your browser.
-   When debugging client scripts, some scripts might be minified. Minified scripts have all unnecessary characters removed, including empty space characters, new line characters, and so on. Minifying scripts reduces the amount of data that needs to be processed and reduces file size, but it can also make scripts difficult to read. You can use your browser to de-minify scripts so that they're more readable. To learn how to de-minify scripts, see the documentation for your browser.

 |
| Testing | 

-   When testing form-level client scripts, use Ctrl-Refresh to clear your browser cache and ensure that the latest scripts are being executed.

 |
| Client Scripts in SuiteApps and Bundles | 

-   If you need to include client scripts in a SuiteBundle or a SuiteApp, don't enable the Hide in SuiteBundle preference on the client script's file record.
-   If a client script included in a SuiteApp or SuiteBundle references another script file, such as a library file:
    1.  First, upload the library file to the File Cabinet. Don't enable the Hide In SuiteBundle preference.
    2.  Next, set your installation preferences, being sure not to hide any client script files or files referenced from client script files.
    3.  Finally, link the library file to the client script file.

 |

### Related Support Articles

-   [SuiteApp Architectural Fundamentals and Examples (SAFE Guide)](https://suiteanswers.custhelp.com/ci/okcsFattach/getFile/1011960/SuiteAppArchitecturalFundamentalsandExamples.pdf)

### Related Topics

-   [SuiteScript Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/part_N3360914.html)
-   [General Development Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361037.html)
-   [Map/Reduce Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0801064715.html)
-   [Scheduled Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361671.html)
-   [Suitelets and UI Object Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361294.html)
-   [User Event Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361453.html)
-   [Optimizing SuiteScript Performance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460387617.html)
-   [SuiteScript Security Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_159804448843.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
