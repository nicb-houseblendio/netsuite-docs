---
id: "section_N2902985"
type: "section"
title: "What You Can Do with the SuiteScript API"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Overview > What You Can Do with the SuiteScript API"
parent: "article_163726005075"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2902985.html"
anchors: ["bridgehead_N2903054", "bridgehead_N2903239", "bridgehead_N2903273"]
sha256: "e3a890e28765dda14cb68e838e9da595aabab306a15105fe0d404ec5fdecb561"
---

SuiteScript is a JavaScript-based API that provides the ability to extend NetSuite beyond its standard capabilities and additional capabilities provided through point-and-click customization.

You can access most NetSuite forms, records, and customization objects through SuiteScript. What you decide to do with SuiteScript depends on which part of NetSuite you're trying to extend, search, or process.

Before using SuiteScript, consider what you want to achieve in NetSuite:

1.  [What You Want to Do](#bridgehead_N2903054)
    
2.  [SuiteScript Modules That Support What You Want to Do](#bridgehead_N2903239)
    
3.  [How To Run a Script in NetSuite](#bridgehead_N2903273)
    

## What You Want to Do {#bridgehead_N2903054}

The following table shows some of SuiteScript uses. Links are provided to the NetSuite script type you can use to programmatically accomplish the tasks.

| Task | Suggested NetSuite Script Type |
| --- | --- |
| Perform custom business processing when NetSuite records are updated, created, or deleted | [SuiteScript 2.1 User Event Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799721.html) |
| Perform custom validations and calculations in the browser | [SuiteScript 2.1 Client Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387798404.html) |
| Create custom user interfaces | [SuiteScript 2.1 Suitelet Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799600.html) or [SuiteScript 2.1 User Event Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799721.html) and [SuiteScript 2.1 UI Modules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518470197.html) |
| Run batch processes | [SuiteScript 2.1 Scheduled Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799491.html) |
| Run NetSuite searches | [SuiteScript 2.1 User Event Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799721.html) or [SuiteScript 2.1 Scheduled Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799491.html) |
| Perform utility processing, such as sending email and faxes, creating and uploading files, or working with XML documents | [SuiteScript 2.1 Suitelet Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799600.html) or [SuiteScript 2.1 User Event Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799721.html) |
| Create custom dashboard portlets | [SuiteScript 2.1 Portlet Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799288.html) |
| Perform processing in target accounts for packaged SuiteApps as part of SuiteApp installation or update | [SuiteScript 2.1 Bundle Installation Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460460309.html) and [SuiteScript 2.1 SDF Installation Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1544719586.html) |

## SuiteScript Modules That Support What You Want to Do {#bridgehead_N2903239}

The SuiteScript API documentation is organized by the types of tasks most developers want to perform. See [SuiteScript 2.x API Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_4140956840.html) to get started with the SuiteScript API.

See [SuiteScript 2.1 Modules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4220488571.html) to see how all the SuiteScript 2.x API is organized into modules. The documentation for each module lists whether it can be used in client, user event, scheduled, Suitelet, or portlets scripts.

## How To Run a Script in NetSuite {#bridgehead_N2903273}

There are two ways to run SuiteScript scripts:

-   **The SuiteCloud Development Framework (SDF)** - Using SDF with the SuiteCloud Software Developer Kit (SDK) is the best solution for creating a script as a part of an overall NetSuite customized solution packaged with other items, such as custom records, custom forms, other scripts, or more. For more information about SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html).
    
-   **The NetSuite UI** - You can manually upload your script file, create a script record, and deploy the script.
    

#### To upload and deploy a script in the NetSuite UI:

1.  Write and save your script as a JavaScript file.
    
2.  Upload the JavaScript file to NetSuite.
    
3.  Create a script record for your script.
    
4.  Create a script deployment record to define script runtime options and deploy the script.
    

To learn about each step in the above process, see [SuiteScript 2.1 API Introduction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4387172221.html). This topic includes information about script basics, the script creation process, and a sample Hello World! script.

### Related Topics

-   [SuiteScript Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163726005075.html)
-   [Using SuiteScript with NetSuite Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2903330.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
