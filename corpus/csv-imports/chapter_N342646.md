---
id: "chapter_N342646"
type: "chapter"
title: "CSV Imports Overview"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > CSV Imports Overview"
parent: "book_4470700566"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N342646.html"
anchors: []
sha256: "12dd9f8b1449f40cff7895885825291ff5b6f3ac96e9fef5bbd27820e25568b3"
---

CSV import is the most commonly used method for transferring small to medium-sized data sets from other applications into NetSuite. The CSV import process saves time and prevents errors, by submitting data in a CSV (comma-separated value) file. This data can add or update many records at one time, avoiding the need for manual data entry.

Note:

You should scrub your data before importing it.

NetSuite provides an Import Assistant that you can use to step through the process for most CSV imports. If you have full permissions for the Import CSV File permission, the Import Assistant is available at _Setup > Import/Export > Import CSV Files_. The types of data that you can import with the Assistant depend on your role, permissions, and which features are enabled in your account. For more information, see [NetSuite Permissions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N325094.html).

![Import Assistant page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/MainImpAsst.png)

You can save an import job to be run later. After you've saved an import, you can reuse its mapping for future import jobs and share it with other users. When you run an import, you can check the status page to see its progress.

Review the following for information about importing CSV data into NetSuite:

-   For instructions for working with the Import Assistant, see [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html).
    
-   For help preparing files for CSV import and a list of record types that can be imported, see [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html).
    

For details about alternate approaches to import tasks, see the following:

-   After you've saved an import map, you can use a SuiteScript API to import CSV file data with that mapping. For details, see [task.CsvImportTask](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345798668.html).
    
-   See [Additional Import and Export Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N463253.html) for information about other imports that do not use the CSV Import Assistant, including Peachtree data.
    
-   NetSuite SOAP and REST web services are a good option for large or ongoing data migrations, or for record types that CSV import doesn't support yet. For information, see the [SuiteTalk SOAP Web Services Platform Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_156388532579.html).
    

Note the following:

-   You can use simpler versions of the Import Assistant to bring in budget data, single journal entries, inventory worksheets, Microsoft Project tasks, and website redirects into NetSuite.
    
    -   You'll find the **budget import assistant** at _Transactions > Financial > Set Up Budgets_ > Import, if you have the Set Up Budgets permission. For more information, see the [Budget Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433988.html) help topic.
        
    -   The **single journal entry import assistant** is available at _Transactions > Financial > Make Journal Entries > Import_. If you use NetSuite OneWorld, the **single intercompany journal entry import assistant** is at _Transactions > Financial > Make Intercompany Journal Entries > Import_. You need the Make Journal Entry permission. For more information, see the [Single Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433632.html) help topic.
        
    -   The **single inventory worksheet import assistant** is available at _Transactions > Inventory > Adjust Inventory Worksheet > Import_. You need the Adjust Inventory Worksheet permission. For more information, see the [Single Inventory Worksheet Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N434282.html).
        
    -   You'll find the **project tasks import assistant** at _Activities > Scheduling > Project Tasks > Import_, if the Project Management feature is enabled. For more information, see the [Project Tasks Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N438898.html) help topic.
        
    -   The website redirects import assistant is at _Commerce > Hosting > Redirects > Import_, when the Web Site and Host HTML Files features are enabled. You need the Set Up Web Site permission. For more information, see [Importing Website Redirects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2638492.html).
        
-   These CSV imports use templates and aren't available in the Import Assistant: [Bulk Fulfilling Orders Using a CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1226924.html) , [Importing a Vendor Price List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2368077.html), [Importing Employee Commission Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1154345.html), and [Importing Single-Use Coupon Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519291829.html#subsect_1519731916).
    
-   You can use a SuiteScript API to automate CSV imports with scripts instead of the Import Assistant. See [task.CsvImportTask](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345798668.html). Note that scripted imports aren't supported for data you'd normally import with the simple (2-step) assistants.
    

### Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [CSV Import Error Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4568635774.html)
-   [Additional Import and Export Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N463253.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
