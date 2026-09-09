---
id: "chapter_N3361037"
type: "chapter"
title: "General Development Best Practices"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Best Practices > General Development Best Practices"
parent: "part_N3360914"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361037.html"
anchors: []
sha256: "9aa60b63817c1000c0a9b74d623a797a006f6a2495d2c442e49a0ac852a44659"
---

Important:

If you're using SuiteScript 1.0 or SuiteScript 2.0 for your scripts, consider converting these scripts to SuiteScript 2.1. Use SuiteScript 2.1 to take advantage of a new runtime engine which may improve performance, new features, and functionality enhancements, including newer ECMAScript language features. SuiteScript 2.1 server supports ES2023 and SuiteScript 2.1 client supports the ES version supported by the browser. For more information, see [SuiteScript Versioning Guidelines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4417231053.html) and [SuiteScript 2.1](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156042690639.html). To help you create SuiteScript 2.1 code, you can use the SuiteCloud Developer Assistant, an AI-powered coding assistant that provides coding support as you build NetSuite customizations in Visual Studio Code with the Cline extension. For more information about the SuiteCloud Developer Assistant, see _Using SuiteCloud Developer Assistant to Create SuiteScript 2.1 Scripts_.

Here are some general best practices for writing SuiteScript scripts:

| Using SuiteScript modules | 
-   When you specify the modules that your script uses, make sure that the order of the modules matches the order of the parameters in your main function. For example, if your script uses the N/error, N/record, and N/file modules and you specify them in this order, make sure that your function parameters are in the same order, as follows: `require(['N/error', 'N/record', 'N/file'], function(error, record, file) { ... });`

 |
| --- | --- |
| Code organization and structure | 

-   Good code is well organized. Data and operations in each function or class fit together. Organize your code into reusable chunks. Many functions can be used in a variety of forms. Any reusable functions should be stored in a common library file and then called into specific event functions for the required forms as needed.
-   Good code is written using small, readable, reusable functions. Including too many lines of code in one function makes it harder to understand and debug. Consider refactoring your code to keep all functions reasonable in size.
-   Use nesting judiciously. Extensive nesting may make your script unreadable. Try to keep your scripts as readable as possible.
-   During script development, use components, load them individually and then test each one -- inactivating all but the one you are testing when multiple components are tied to a single user event.

 |
| Naming conventions | Good code uses meaningful naming conventions. A well written script containing descriptive names for functions, variables, IDs, provides a good structure for building comments around. Functions:

-   Although you can use any desired naming conventions for functions within your code, you should use custom name spaces or unique prefixes for all your function names.
-   When working with the top-level NetSuite functions in Client SuiteScript (for example the pageInit function), you should name the new function to correspond to the NetSuite name. For example, a pageInit function can be named pageInit or formAPageInit. If your code is already established, you can wrap it with a top-level function that has the appropriate naming convention.
-   Function Names: All function names should be written in lower camel case which means the first letter of each word (except the first) is capitalized.
-   For IDs, enter all record, field, sublist, tab, and subtab IDs in lower case in your SuiteScript code. Prefix all custom script IDs and deployment IDs with an underscore (\_).

Variables and Constants:

-   Avoid using a single character as a variable name.
-   Name your variables to identify the data type and describe the data stored in the variable. For example,
    -   String variables - prefix with "st", such as stTitle
    -   Integer variables - prefix with "int", such as intTotalCount
    -   Float variables - prefix with "fl", such as flPrice
    -   Boolean variables - prefix with "b", such as bIsDone
    -   Array variables - prefix with "arr", such as arrPhoneCalls
    -   Object variables - prefix with "Obj", such as ObjNewPet
    -   Record variables - prefix with "rec", such as recCustomer
    -   Date variables - prefix with "dt", such as dtFirstBillingDate
-   Local variable scope is only within the function. Use standard camelCase naming.
-   Global variable scope is within the whole file or more files if declared under included library. Use a variable in upper case spaced by underscore.
-   To represent a pseudo constant, use a variable in upper case spaced by underscore. Constants are to be used to make code more readable.

IDs:

-   For IDs, enter all record, field, sublist, tab, and subtab IDs in lower case. Prefix all custom script IDs and deployment IDs with an underscore (\_).

File names:

-   If you write SuiteScript code for multiple accounts, consider using the following file name convention: <Company Name/Abbreviation>\_<Script Type>\_<Requirement Description>.js. For example, MyCompany\_CS\_SetTaxable.js. The following are suggested Script Types:
    -   CS - client scripts
    -   UE - user events
    -   SL - Suitelet
    -   RL - RESTlet
    -   PL - Portlet
    -   SC - Scheduled
    -   MR - Map/Reduce
    -   Gl - SuiteGL
    -   WA - Workflow Action
    -   MU - Mass Update
    -   BI - Bundle Installation

 |
| Commenting | 

-   Thoroughly comment your code. Include comments about what the script is doing and who authored it. This practice helps with debugging and development and assists NetSuite Customer Support in locating problems, if necessary. It also helps anyone else who works with the script.
-   Write useful comments. Good code comments explain what is being done and why it's being done.
-   When documenting functions try to provide a good abstract of the actions of the function without restating the function name.
-   A good way to write relevant comments is to plan your scripts using pseudo code and replace the pseudo code with a relevant comment where necessary.
-   At a minimum, you should include comments: (1) for the file level disclaimer, (2) for version control, (3) at the function level, and (4) at the logic level.
-   Note that in SuiteScript 2.x, inline comments aren't allowed within an object. You may not see a specific error, however, your script won't function properly if you include inline comments within an object.

 |
| Empty space and formatting | 

-   Use empty space and formatting to enhance readability rather than to minimize typing effort. The following rules should always apply:
    -   All line returns within a function should be terminated with a ; (semicolon).
    -   Code blocks should be tab indented.

 |
| Using IDs | 

-   Use **static** ID values in your API calls where applicable because name values can change.

 |
| Passwords | 

-   Don't hard-code any passwords in scripts. The password and password2 fields are supported for scripting. For additional information, see [SuiteScript Security Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_159804448843.html).

 |
| Error and exception handling | 

-   Include proper error handling sequences in your script wherever data may be inconsistent, not available, or invalid for certain functions. For example, if your script requires a field value to validate another, ensure that the field value is available.
-   Use try-catch blocks. Try-catch blocks provide a way to 'catch' an exception object thrown with the try block. As soon as an exception is thrown the catch block starts. An optional finally clause can also be used to run (guaranteed) if any exception occurs or not.

 |
| URLs | 

-   Don't hard-code URL links. If the domain name changes, hard-coded URLs won't work. To prevent issues with links, use the [N/url Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157072993576.html).

 |
| Date and Currency fields | 

-   Use the built-in library functions whenever possible for reading/writing Date/Currency fields and for querying XML documents.

 |
| Script parameters | 

-   Use script parameters or configuration files wherever possible, instead of hard coding values, to ensure that scripts can be configured easily
-   You can use the [runtime.getCurrentScript()](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296529387.html) function in the runtime module to reference script parameters. For example, use the following code to obtain the value of a script parameter named custscript\_case\_field: `define(['N/runtime'], function(runtime) { function pageInit(context) { var strField = runtime.getCurrentScript().getParameter('SCRIPT', 'custscript_case_field'); ... });`
-   For security reasons, don't include confidential information in script parameters. Information saved in script parameters can be indexed by search engines and therefore be viewable by the public. This means, for example, that the information could be found in Google searches. For more information, see [Creating Script Parameters Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999300.html).

 |
| Reserved words | 

-   Ensure that your scripts don't use any reserved words in SuiteScript. For more information, see [SuiteScript Reserved Words](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158687368641.html).

 |
| Execution contexts | 

-   Consider the most appropriate script execution context for your script. The script execution context specifies how and when a script is triggered to run. If you don't use the appropriate context, blocks of scripts run when they shouldn't and result in unexpected errors in the data and the script. For more information, see [Execution Contexts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157960743044.html).

 |
| Loading records | 

-   For record Create or Edit operations, you should load records in dynamic mode. This is required to make updates on record object. Load records in a non-dynamic mode if you want to only get field values from the record and update on record isn't needed.
-   Don't use [record.load(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258486.html) to load a whole record when you only need to get the value of a few fields. The performance of the load record API is similar to loading the record in the user interface without field rendering since it loads all configuration fields and sublists for the record. To avoid slowing down the execution of the script, use [search.lookupFields(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345776651.html) to get the value of a few fields.

 |
| Invoking methods | 

-   You should use parameter id's instead of parameter sequence.
-   You should use defined SuiteScript 2.0 native enums. You may find the list of valid enums on Help and SuiteScript 2.0 API pdf.

 |
| Asynchronous programming | 

-   When using promises in your SuiteScript scripts to implement asynchronous programming, you should consider the best practices listed in the [Best Practices for Asynchronous Programming with SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387812940.html#subsect_161428571495) help topic.

 |
| Custom code | 

-   Place all custom code and markup, including third party libraries, in your own namespace. Important: Custom code must not be used to access the NetSuite DOM. Developers must use SuiteScript APIs to access NetSuite UI components.
-   Use Subresource Integrity when you include content from external sources in Inline HTML fields. For more information, see [Subresource Integrity](https://developer.mozilla.org/en-US/docs/Web/Security/Subresource_Integrity).

 |
| Testing | 

-   Good code is well-tested. Testing serves as an executable specification of the code and examples of its use.
-   Always thoroughly test your code before using it on your live NetSuite data.
-   If the same script is used across multiple forms, ensure that you test any changes to the code for **each** form that the code is associated with.
-   During testing, the Deployment Status should be Testing to limit the script processing to the script owner only. If several users are testing a script (or if a Sandbox Account is being used), the Deployment Status can be set to Released, but you must choose the appropriate Audience so that the script doesn't run for users who aren't involved in the testing process. For production, the Deployment Status should set be Released. Again, it's critical to set the appropriate Audience so that the script doesn't run for unintended users.
-   During testing, the Log Level should be set to Debug.

 |
| Logging | 

-   Log messages in the script should make business sense; include the record id, record type and other important details in your log messages. Each log message should provide a clear picture of the functionality that the script is designed to achieve.
-   Key steps in each script should be logged as Audit.
-   Proper logging adds to the readability of the code and also significant on issue/error debugging.
-   During testing, the Log Level should be set to Debug. For a Production Deployment, the Log Level should be set to Audit. Note that if there are production issues that require diagnosis/debugging, the Deployment Log Level can be set back to Debug.

 |
| Other | 

-   Consider the time zone that your scripts must use. By default, server scripts use the time zone that is specified in your NetSuite account. Be sure to convert your time values to the correct time zone before you use them, if necessary.
-   Consider field limits and translation when creating your scripts. Fields that use special characters used in some languages may support fewer characters than the field limit specified. For example, the Reference No. field (tranid) supports 45 English characters, but supports fewer Chinese characters.
-   Be sure to use BigInt values in your scripts to avoid potential errors. Integers larger than [MAX\_SAFE\_INTEGER](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number/MAX_SAFE_INTEGER) and smaller than [MIN\_SAFE\_INTEGER](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number/MIN_SAFE_INTEGER) must be enclosed in quotations or appended with '_n_' at the end of the integer literal. For more information about BigInt values, see [BigInt](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/BigInt).

 |

You can also refer to the following Internet resources for JavaScript coding best practices:

-   [JavaScript Best Practices (w3)](https://www.w3.org/wiki/JavaScript_best_practices)
    
-   [JavaScript Best Practices (w3 schools)](https://www.w3schools.com/js/js_best_practices.asp)
    

### Related Support Articles

-   [SuiteApp Architectural Fundamentals and Examples (SAFE Guide)](https://suiteanswers.custhelp.com/ci/okcsFattach/getFile/1011960/SuiteAppArchitecturalFundamentalsandExamples.pdf)

### Related Topics

-   [SuiteScript Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/part_N3360914.html)
-   [Client Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361924.html)
-   [Map/Reduce Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0801064715.html)
-   [Scheduled Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361671.html)
-   [Suitelets and UI Object Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361294.html)
-   [User Event Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361453.html)
-   [Optimizing SuiteScript Performance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460387617.html)
-   [SuiteScript Security Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_159804448843.html)
-   [SuiteScript Versioning Guidelines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4417231053.html)
-   [SuiteScript 2.1](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156042690639.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
