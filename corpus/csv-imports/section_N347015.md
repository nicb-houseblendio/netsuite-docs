---
id: "section_N347015"
type: "section"
title: "Use Multiple Threads and Multiple Queues to Run CSV Import Jobs"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Step Two Import Options > Use Multiple Threads and Multiple Queues to Run CSV Import Jobs"
parent: "section_N344550"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347015.html"
anchors: ["bridgehead_N347120", "bridgehead_N347144"]
sha256: "90d1d127ada6d2f340375c84f35366f1ec22dabaa5e537aa8859df57b6e0239c"
---

In accounts that have purchased one or more SuiteCloud Plus licenses, the Import Assistant includes two advanced import options that you can set to improve import performance.

For a summary of SuiteCloud Plus capabilities, see [SuiteCloud Plus Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N259503.html).

-   You can check the Use Multi-threading box, to use multiple threads instead of a single thread to process an import job. See [Using Multiple Threads](#bridgehead_N347120).
    
-   You can set a queue number from 1 to 5, to spread the processing of import jobs across multiple queues, instead of using a single queue for all jobs. See [Using Multiple Queues](#bridgehead_N347144).
    

These options are available on step two the Import Options page of the Import Assistant, under Advanced Options. For instructions for completing them, see [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html).

![Use Multi-Threading box on the Import Assistant Import Options page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/CSVmultioption_2014_2.png)

Note:

In addition to supporting import job performance enhancement, the SuiteCloud Plus license also supports access to more concurrent web services sessions and to multiple processors for scheduled scripts and map/reduce scripts. To learn more about SuiteCloud Plus, or to purchase this add-on module, contact your NetSuite account manager.

## Using Multiple Threads {#bridgehead_N347120}

By default, CSV import uses a single thread and processes each row in order. If your account has SuiteCloud Plus licenses, you can enable multi-threading. When you enable this option, the import runs across multiple threads for better performance, but the row order isn't guaranteed. Only use multi-threading if the order the rows are submitted doesn't matter, meaning later CSV file row data does not depend on any earlier row data.

Note:

If you enable this option for an import where order does matter, some records may fail to import, because they depend on records which have yet to be imported. When this situation occurs, you can run the job a second time to import the dependent records.

If you purchase one SuiteCloud Plus license, two threads are available for each import job. In some cases, you may be able to purchase three, six, or 12 licenses to support 10 threads per job.

For more information, see [SuiteCloud Plus Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N259503.html).

For information about service tiers, see [NetSuite Service Tiers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1539959231.html).

## Using Multiple Queues {#bridgehead_N347144}

By default, all CSV import jobs use a single queue. This queue is defined as queue 1. Accounts that have purchased a SuiteCloud Plus license, have five queues for import jobs, instead of a single queue. You can choose which queue to use for each import job from a dropdown in the Import Assistant. This lets you spread out jobs across multiple queues to boost performance.

Important:

You can never have more than five import queues, no matter how many SuiteCloud Plus licenses you buy..

Import jobs in each queue run one after the other. So if you have two jobs in queue 1, the second one waits for the first to finish. But across all five queues, jobs run at the same time-so if you have one job in each queue, they all run together.

If you buy SuiteCloud Plus, all your saved import jobs start out in queue 1 by default. You must go to step two on the Import Options page for each job and choose a different queue if you want. If you don't choose a queue for the new import, it'll go to queue 1 automatically.

The import Job Status page has a Queue column to show which queue is handling each job. You can also use the Queue filter to sort jobs by queue number.

### Related Topics

-   [Step Two Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344550.html)
-   [Choose Data Handling for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345294.html)
-   [Required Permissions for CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345544.html)
-   [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html)
-   [SuiteCloud Plus Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N259503.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
