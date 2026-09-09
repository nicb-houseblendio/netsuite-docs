---
id: "section_N2730900"
type: "section"
title: "Initiating a Workflow on a Schedule"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Overview > Workflow Initiation > Initiating a Workflow on a Schedule"
parent: "section_4080797941"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2730900.html"
anchors: []
sha256: "eb31f05cb7cd7f22371fd516031a630e1103756e9b460d0bd94ee78d5d971df1"
---

When you set up a workflow to run on a schedule, the workflow executes on the results of a saved search. You can schedule the workflow to run one time, run every 30 minutes, or run at a certain time on a daily, weekly, monthly, or yearly basis. When you choose to initiate workflows on a scheduled basis, you select a saved search and then define the schedule on which the workflow runs.

Before you define the schedule for the workflow, you must create the saved search. The saved search must run on the same record type as the base record type for the workflow. The saved search must also include at least one filter set on the **Criteria** subtab for the saved search. On the workflow definition page, select the **Scheduled** option, select the saved search, and set the schedule for the workflow.

Important:

When you create a saved search, be sure to add enough filters on the Criteria subtab to limit the results to only the records you want. If you don't, the saved search might return too many results and the scheduled workflow might not execute as expected. For example, it could take longer to run than you planned, which could affect the performance of other workflows.

At the scheduled time, NetSuite runs the saved search and initiates a workflow instance to run on each of the records in the search results. For example, if the saved search returns 10 records, NetSuite initiates 10 instances of the workflow. Scheduled workflows always run on all of the records in the search results, not only the records you can see on the main page (for summary type result) of the saved search.

To set up a scheduled workflow, select the saved search it should run on and select the schedule options. You can schedule the saved search and workflow to run one time, or use the **Repeat** option for a repeating schedule. If you want the workflow to run one time, select the saved search, clear the **Repeat** box, and set the **Execution Date** and **Execution Time**. If you want the workflow to run more than one time, select the saved search, check the **Repeat** box, and set the related options.

Consider the following when you create scheduled workflows:

-   NetSuite runs multiple workflows in parallel. Each workflow instance runs as an administrator, and any system note shows 'System' as the user name.
    
-   There is no set order for when scheduled workflows start and finish. For example, three scheduled workflows, A, B, and C, are all scheduled at the same time. NetSuite simultaneously runs each saved search and initiates workflows on the results. Depending on the workflow and the number of search results, any of the workflows may complete before the other two.
    
-   Only scheduled workflows with a **Released** status run on a schedule.
    
-   Schedule workflows to run on saved searches that return narrow search results by setting filters on the Criteria subtab. If you don't add enough filters, the saved search could return too many results, and the workflow may not execute as expected.
    
-   You must set all workflow initiation criteria when you create the saved search. You can't set a condition to initiate a scheduled workflow.
    
-   If you schedule workflows to run on saved searches from SuiteApps, you need the SuiteApp Marketplace permission assigned or the scheduled workflow won't run correctly.
    

For a detailed instruction about how to create a scheduled workflow, see [Scheduling a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4108268619.html).

For more information about how NetSuite runs scheduled workflows, see [Scheduled Trigger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103739399.html).

The following screenshot shows a lead nurturing workflow scheduled to run against Customer Lead records on a daily basis:

![A screenshot depicting the Schedule settings required to set a workflow to run against a record on a daily basis.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/ScheduledInitiation.png)

For an example of how to create a saved search and use it in a scheduled workflow, see [Welcome Email Sent to Customers Three Days After First Order Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2806856.html).

### Related Topics

-   [Workflow Initiation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4080797941.html)
-   [Initiating a Workflow on an Event](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2730601.html)
-   [Using SuiteScript to Initiate a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2731126.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
