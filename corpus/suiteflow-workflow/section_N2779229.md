---
id: "section_N2779229"
type: "section"
title: "Release Status for Workflow Instances"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Working with Workflows > Creating a Workflow > Release Status for Workflow Instances"
parent: "section_4101527388"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2779229.html"
anchors: []
sha256: "52476ee7f3ea0e8d064aef8bf4e5cc0978071ce7ec2c757886c541a292137f9b"
---

Use the Release Status property to test a workflow, make it available to everyone, or keep it from running.

![A portion of the workflow definition page showing the Release status options: Suspended, Not Initiating, Testing, and Released.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/ReleaseStatus_19.1.png)

The following table describes the workflow release statuses and when you should use each status:

| Release Status | Description | When to Use |
| --- | --- | --- |
| Suspended | No new workflow instances are created and no existing instances run. If there are scheduled workflows, transitions, or actions, none of these run. You can't initiate a suspended workflow using SuiteScript, or using the Initiate Workflow or Mass Update actions in SuiteFlow. To resume a suspended workflow, change its Release Status something other than Suspended. | Use this when you want a workflow to stop running, but you don't want to delete it. |
| Not Initiating (Not initiating mode) | New instances of the workflow don't start, but instances already running continue to run. The workflow still appears on the Workflow list page. It's similar to inactivating a workflow. | Use this when you don't want any new workflow instances to start but you still want existing instances to run. See [Viewing Existing Workflows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4101532858.html). |
| Testing (Testing mode) | A workflow instance initiates only for the workflow owner. However, anyone who accesses the record can see the changes that the workflow made to the record. Workflow actions execute for the user even if they didn't initiate the workflow instance. Scheduled workflows don't run when the workflow is in testing mode. This is the default Release Status when you create a new workflow. | Use when you want to test a workflow. In testing mode, the workflow execution log appears for each state on the **Workflow History** subtab on any record in a workflow. See [Workflow Execution Log](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4472471134.html). |
| Released (Released mode) | An instance of the workflow initiates for any user with access to its base record type. Scheduled workflows, actions, and transitions execute only when the workflow is in released mode. Enable logging on the workflow definition if you want to continue generating execution logs. | Use this when you want the workflow to run for everyone. For more information about which users can initiate a workflow, see [Users Who Can Run Workflows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4073598374.html#bridgehead_4081988777) and [Defining the Workflow Audience](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4082045210.html). |

### Related Topics

-   [Creating a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4101527388.html)
-   [Execute as Admin for Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2780140.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
