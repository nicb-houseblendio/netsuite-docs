---
id: "chapter_N3917921"
type: "chapter"
title: "SuiteScript FAQ"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript FAQ"
parent: "book_14946590423"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3917921.html"
anchors: ["subsect_156268278195", "question_N3917986", "question_N3918016", "question_N3918046", "question_N3918076", "subsect_0626023810", "subsect_156268280620", "question_N3918114", "question_N3918279", "question_N3918311", "question_N3918345", "subsect_0626030428", "subsect_156268266149", "question_N3918155", "question_N3918191", "subsect_156268286759"]
sha256: "b939dbd9d339dfbeed9f0e284f7712f796474bfedd2b3a5b1b6e58c23a7757f9"
---

This FAQ covers several topics:

-   [General](#subsect_156268278195)
    
-   [SDF and SuiteApps](#subsect_0626023810)
    
-   [Code](#subsect_156268280620)
    
-   [Additional tools to work with along with SuiteScript](#subsect_0626030428)
    
-   [Errors](#subsect_156268266149)
    
-   [Logs](#subsect_156268286759)
    

For FAQ information related to SOAP web services, see [SOAP Web Services Frequently Asked Questions (FAQ)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1554821898.html).

## General {#subsect_156268278195}

### Can I use the SuiteCloud Developer Assistant?

Yes, if you are using the Visual Studio Code IDE. For more information, see [Using SuiteCloud Developer Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_21152355242.html).

### How often is the SuiteScript API documentation updated? {#question_N3917986}

The SuiteScript API documentation is updated frequently and pushed to the NetSuite Help Center.

For the most current API documentation, see [SuiteScript 2.x API Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_4140956840.html).

### Which records are supported in SuiteScript? {#question_N3918016}

You can find all information about SuiteScript-supported records, fields, tabs, sublists, search filters, and search columns in the NetSuite Help Center.

See [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html) for information about supported records.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/index.html) for details related to SuiteScript-supported records.

### Which sublists are supported in SuiteScript? {#question_N3918046}

You can find all information about SuiteScript-supported records, fields, tabs, sublists, search filters, and search columns in the SuiteScript Records Browser.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/index.html) for details related to SuiteScript-supported sublists and their internal IDs.

### What is the difference between SuiteScript 1.0 and SuiteScript 2.x?

SuiteScript 1.0 uses global functions whereas SuiteScript 2.x is modular. The functions in SuiteScript 1.0 are synchronous on client, but SuiteScript 2.x can use asynchronous processing. SuiteScript 2.x offers more APIs. New functionality is added to SuiteScript 2.x only.

See the [SuiteScript 1.0 to SuiteScript 2.1 API Map](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4752722762.html) for more details on the differences.

A new version of SuiteScript, SuiteScript 2.1, is also available. This version is the latest minor version of SuiteScript. It extends SuiteScript 2.x by supporting additional ECMAScript language features and syntax. For more information, see [SuiteScript 2.1](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156042690639.html).

### What version of SuiteScript should I use?

Use SuiteScript 2.x for new scripts that you develop, and consider converting your SuiteScript 1.0 scripts to SuiteScript 2.0 or SuiteScript 2.1.

SuiteScript 1.0 isn't being updated with new features or enhancements. SuiteScript 1.0 scripts are still supported, but for new or revised scripts, use SuiteScript 2.x to get the latest features and enhancements.

A new version of SuiteScript, SuiteScript 2.1, is also available. This version is the latest minor version of SuiteScript. It extends SuiteScript 2.x by supporting additional ECMAScript language features and syntax. For more information, see [SuiteScript 2.1](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156042690639.html).

### Does SuiteScript support the use of multiple library files? {#question_N3918076}

Yes. Multiple library files can be loaded onto the Script record page. The Script record page is where you set up your SuiteScript .js file and any required library files.

Also be aware that the system reads your library files in the order they appear on the Library Script File subtab on the Script record page. For example, if your first library file references the second library file, an error will be thrown, since the first library file is loaded before the second.

If you're unsure about creating a Script record or loading library files, go to the topic [Creating a Script Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489062315.html) in the NetSuite Help Center.

### What is the difference between Standard and Dynamic mode?

When a SuiteScript 2.x script creates, copies, loads, or transforms a record in standard mode, the record's body fields and sublist line items are not sourced, calculated, and validated until the record is saved. In dynamic mode, the record's body fields and sublist line items are sourced, calculated, and validated in real-time.

See [SuiteScript 2.x Standard and Dynamic Modes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1524156901.html) for more details.

### What are the best practices when using Standard and Dynamic mode?

Standard mode is usually faster, so use it for read-only operations.

Dynamic mode may be needed when doing write operations of fields on which other field depend.

See [SuiteScript 2.x Standard and Dynamic Modes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1524156901.html) for more details.

### How do I use require Configuration?

If you set up a valid `@NAmdConfig` JSDoc tag, SuiteScript implements the require configuration settings _before_ loading dependencies.

See [require Configuration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4599733337.html) for more details.

### What is SuiteScript governance?

Governance checks scripts for issues like infinite loops and stops them if necessary.

NetSuite uses a governance model to optimize performance, based on usage units. If you exceed the allowed units, the script will be terminated.

See [SuiteScript Governance and Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3350651.html) for more details.

### What is SuiteCloud Processors?

SuiteCloud Processors is the current system used to process scheduled scripts and map/reduce scripts. Before SuiteCloud Processors was introduced, scheduled scripts and map/reduce scripts were exclusively processed by scheduling queues.

See [SuiteCloud Processors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1498571420.html) for more details.

### Which is better to use: Scheduled script or Map Reduce script?

Use scheduled scripts for simple tasks that can't run at the same time. Map/Reduce script is better suited for processing massive data in parallel, since it is faster then Scheduled script.

See [SuiteScript 2.1 Scheduled Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799491.html) and [SuiteScript 2.1 Map/Reduce Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799161.html) for more details.

### What version of ECMAScript does SuiteScript support?

SuiteScript 1.0 and SuiteScript 2.0 support ECMAScript 5.1.

SuiteScript 2.1 supports ECMAScript 6. This version is the latest minor version of SuiteScript. It extends SuiteScript 2.x by supporting additional ECMAScript language features and syntax. For more information, see [SuiteScript 2.1](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156042690639.html).

### Can a User Event script be used to trigger another User Event script?

Nested user event script execution is not supported.

See [SuiteScript 2.1 User Event Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799721.html) for more details.

## SDF and SuiteApps {#subsect_0626023810}

### What is SDF and how does it help me develop with SuiteApps?

SuiteCloud Development Framework (SDF) is a framework that lets you create SuiteApps from your local computer using an integrated development environment (IDE). Using SDF lets you manage client and server scripts as part of file-based customization projects. You can also use SDF with the SuiteCloud Software Developer Kit (SDK) as the best solution for creating a script as a part of an overall NetSuite customized solution packaged with other factors, such as custom records, custom forms, other scripts, or more. For more information about SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html),

### Is there a special script type for installing SDF projects?

Yes, the SDF installation script type helps with tasks when developing a SuiteApp from SDF to your target account. You can use the SDF installation script type to perform setup, configuration, and data management tasks that otherwise would have to be completed by account administrators. For more information about the SDF installation script type, see [SuiteScript 2.1 SDF Installation Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1544719586.html).

### Does SuiteScript have a module that I can use to see information about my SuiteApp?

Yes, the N/suiteAppInfo module provides information about your SuiteApp, including whether a specific SuiteApp is installed and a list of all SDF SuiteApps that are installed, along with the ID for the SDF SuiteApp that contains a specific script (for multiple scripts specified). For more information about the N/suiteappInfo module, see [N/suiteAppInfo Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_160236086332.html).

## Code {#subsect_156268280620}

### How can I control the execution order of scripts deployed on a record?

To control script execution order, log in to NetSuite, go to _Customization > Scripting > Scripted Records_, select your record type, and drag the scripts up or down

### How many client and user event scripts can I deploy in a record?

You can deploy as many scripts as you need, but be aware that too many scripts deployed on single record can cause performance issues.

### How do I add a button in a User Event script that redirects to a Suitelet in SuiteScript 2.x?

In the `beforeLoad` callback, you get a form object on which any button can be added. That button can run an arbitrary function. The function must use `document.location = <url of a suitelet>` for redirect.

See [SuiteScript 2.1 User Event Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799721.html) or [SuiteScript 2.1 Suitelet Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799600.html) for more details.

### Can I write to a script parameter field I have created in my code? {#question_N3918114}

You can read script parameter field values, but you can't set them programmatically. The only time you can specify a value outside of the UI is when you call [task.create(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4392320106.html).

                `var myTask = task.create({task.TaskType.SCHEDULED_SCRIPT}); myTask.scriptId = <id of your script>; myTask.deploymentId = <id of your script deployment>; myTask.params = <your params>; myTask.submit();` 
              

See [Creating Script Parameters Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999300.html) for more information about creating and working with script parameters.

### How do I mass delete records using SuiteScript? {#question_N3918279}

Currently, there's no way to mass delete records. You need to delete each record individually using [record.delete(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267283372.html).

### Which certificate authorities (CAs) does NetSuite support? {#question_N3918311}

NetSuite supports the same list of trusted third-party certificate authorities (CAs) as Mozilla Included CA Certificate List.

The endpoint you're connecting to must use a trusted CA, or the connection won't work. When connecting to an endpoint from NetSuite, make sure it provides a full certification chain, including intermediate certificates.

For a list of certificate authorities, see [https://wiki.mozilla.org/CA/Included\_Certificates.](https://wiki.mozilla.org/CA/Included_Certificates)

### Can I throw an alert in a Suitelet? {#question_N3918345}

You can attach a client script by using the [N/ui/message Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4497735093.html).

                `/**  * @NApiVersion 2.1  * @NScriptType Suitelet  */ define(['N/ui/serverWidget', 'N/ui/message'], function(serverWidget, message){     function onRequest(context){         let form = serverWidget.createForm('Alert Form');         let msg = message.create({             type:message.Type.WARNING,             title:"Alert",             message: "Something occurred",             duration: 5000         });         form.addPageInitMessage(msg);         context.response.writePage(form);     }      return{         onRequest: onRequest     } });` 
              

[N/ui/message Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4497735093.html) and [N/ui/dialog Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4497725142.html) only work in client scripts.

### Is there a change in creating subrecords in SuiteScript 2.x?

Yes, SuiteScript 2.x has changes in how you create subrecords.

See [Subrecord Scripting in SuiteScript 2.x Compared With 1.0](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4675627975.html) for more details.

### How do I optimize SuiteScript performance?

There are several guidelines that you can follow to optimize SuiteScript performance.

See [Optimizing SuiteScript Performance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460387617.html) for more details.

### Should I use record-level or form-level scripts?

There are different forms used for different users. Use them when you need to run different scripts for different users. Record-level script is always used regardless of the user. Based on that, you can decide which type of script should be used.

See [Record-Level and Form-Level Script Deployments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4576055055.html) for more details.

### Where can I find the records and their scripts?

The Scripted Records page shows all records with associated user event or global client scripts.

See [The Scripted Records Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2936246.html) for more details.

### What is the difference between Map Reduce and Scheduled Script?

Use map/reduce scripts for handling large datasets that can be broken down into smaller, independent parts.

Scheduled scripts are server scripts that run sequentially on SuiteCloud Processors, whereas map/reduce scripts run in parallel.

See [SuiteScript 2.1 Script Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4387172495.html) for more details.

### Is DOM supported in SuiteScript?

You can't access the NetSuite UI directly using Document Object Model (DOM). Use SuiteScript APIs instead.

### What are the required SuiteScript 2.x JSDoc Tags?

For entry point scripts, you need to include `NApiVersion` and `NScriptType` JSDoc tags. For more information about JSDoc tags, see the help topic: [SuiteScript 2.1 JSDoc Validation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4387175355.html).

### What are the stages required in a Map Reduce script?

You need to include at least `getInput` and one of map/reduce stages.

### What does the script context seen in System Notes represent regarding the action on the record?

The script context shows where the operation that changed the field came from - it's the second-most nested scope in the stack of operations.

For example, if in the UI, the `pageInit` callback is used on a record to call `nlapiRequestURL` to trigger a Suitelet. This calls another `nlapiRequestURL` to trigger a RESTlet, which loads a record that triggers a user event that changes the field, then the context is RESTlet. The stack will be `UI/Client/Suitelet/Restlet/UserEvent`. RESTlet is the second most nested scope.

### How do you reference Custom Modules in SuiteScript 2.x?

Add custom modules to your `define` callback dependencies by path.

### What is the difference between scriptContext.newRecord and scriptContext.oldRecord in SuiteScript 2.x?

`scriptContext.oldRecord` stores the original record before any changes

`scriptContext.newRecord` stores the record which can be modified in the `beforeSubmit` callback, so you can save it differently than what's shown in the UI. For example, you can override a memo before the record is saved.

## Additional tools to work with along with SuiteScript {#subsect_0626030428}

### What other tools are available to help me write my SuiteScript scripts?

You have several tools at your disposal, such as SDF, SDK, Records Catalog, and Records Browser.. For more information about SDF and SDK, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html). For more information about the Records Catalog and the Records Browser, see [Records Catalog](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_160276344912.html) and [SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1218120414.html#section_1527577879). For more information about additional SuiteCloud tools, see [SuiteCloud Reference Tools](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1527577831.html).

## Errors {#subsect_156268266149}

You can find SuiteScript error descriptions in [SuiteAnswers](https://suiteanswers.custhelp.com/). Type the error in the search box and click **Search**.

### How does 'Record Has Been Changed' error get triggered in SuiteScript execution?

This error occurs when someone else (or another script) changes the record at the same time.

See the SuiteAnswers article [Prevent losing data because of the error "Record has been changed"](https://suiteanswers.custhelp.com/app/answers/detail/a_id/34404) for more details.

### What is the 'You do not have privileges to view this page' error message on the script deployments page? {#question_N3918155}

Users will get this error if any of the **Select All** box on the Audience subtab on the Script Deployment page isn't checked. This applies to both internal and external users, even those accessing the Suitelet without logging in.

See [Errors Related to the Available Without Login URL](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1524084097.html) for more details.

### What is the 'You are not allowed to navigate directly to this page' error message when accessing Suitelet? {#question_N3918191}

Users will get this error if the Suitelet's **Status** isn't set to Released, even if they're accessing it externally.

See [Errors Related to the Available Without Login URL](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1524084097.html) for more details.

### Why am I getting an 'SSS\_USAGE\_LIMIT\_EXCEEDED ID' error?

You'll get this error if your script uses too many usage points in one go. ii it happens twice, the script will stop running.

For more information about usage limits, see the help topic [SuiteScript Governance and Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3350651.html)

Keep an eye on your script usage, as there are limits in place. For more information, see [Monitoring Script Usage](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3352047.html).

### Why am I getting an 'SSS\_REQUEST\_LIMIT\_EXCEEDED' error?

You'll get this error if your server script or application takes too long to run.

For more information about usage limits, see the help topic [SuiteScript Governance and Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3350651.html)

### Why am I getting 'SSS\_INVALID\_SUBLIST\_OPERATION' error?

This error happens when you try to set a value on a line that doesn't exist, or if the sublist isn't editable.

See the SuiteAnswers article [SuiteScript Error SSS\_INVALID\_SUBLIST\_OPERATION](https://suiteanswers.custhelp.com/app/answers/detail/a_id/45324) for more details.

## Logs {#subsect_156268286759}

### How long will the script execution logs be available on my account?

You can find script execution logs in two places:

-   **Execution Log** subtab on Script and Script Deployment records - Shares log storage with other customers on the same database. To prevent excessive logging, there's a storage limit for script execution logs on each NetSuite database instance. If the log storage limit is reached on a server, all logs for all customers on that server will be deleted. You might have logs older than 30 days if the volume is low, but if it's high, you might only have logs from the past week. To keep important log information, consider storing it in custom records.
    
-   **Script Execution Log** page - The execution logs at _Customization > Scripting > Script Execution Logs_ stores logs for up to 30 days, no matter how many logs there are. This page can only show up to 10,000 log results at a time. If you have more than 10,000 logs, you can filter the page to see the ones you need. Use the **Filters** section at the top of the page to narrow down the logs by date, script, or log level. Keep in mind that you can't do a full search or customize the view on this page.
    

### Can I use execution logs in a client script?

Yes, you can use execution logs in client script. For SuiteScript 1.0, use `nlapiLogExecution` (see [SuiteScript 1.0 Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7151939532.html)). For SuiteScript 2.x, use [N/log Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4574548135.html).

### Related Topics

-   [SuiteScript 1.0 Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7151939532.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [Setting Runtime Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2996991.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
