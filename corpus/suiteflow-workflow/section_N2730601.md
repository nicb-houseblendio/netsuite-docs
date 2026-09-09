---
id: "section_N2730601"
type: "section"
title: "Initiating a Workflow on an Event"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Overview > Workflow Initiation > Initiating a Workflow on an Event"
parent: "section_4080797941"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2730601.html"
anchors: ["bridgehead_4108930105"]
sha256: "5ab1b8b63fef24f80cf12fe43b6e80e87f05d4363e0e5fee1d51695fe24f75d0"
---

To initiate a workflow instance on an event, select **Event Based** under **Initiation** on the workflow definition page and then select one or both of the following events for the workflow base record type:

-   **On Create.** Initiate an instance of the workflow when the record is created.
    
-   **On Update.** Initiate an instance of the workflow when the record is viewed or updated.
    

You must also select the server trigger type for workflow initiation. See [Workflow Initiation Triggers](#bridgehead_4108930105).

The following table describes optional requirements that you can use to further define when a workflow instance initiates:

| Option | Description |
| --- | --- |
| Event Types | User interface activity used to create, view, or update the record. The trigger type determines which event types are available. See [Workflow Event Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954657.html). |
| Contexts | NetSuite functionality or feature used to create, view, or update the record. See [Execution Contexts and Workflows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4080817850.html). |
| Condition | Use the Condition Builder or Formula Builder to define requirements that must be met for a workflow instance to initiate. See [Workflow Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954369.html). |
| Saved Search | Initiate the workflow if the record for the workflow meets the criteria in the saved search. The saved search must run on the same record type as the base record type for the workflow. The saved search must also include at least one filter set on the **Criteria** subtab for the saved search. |

For example, you can create a lead nurturing workflow to run when a record is created and saved. Select **On Create** for the event based initiation and select the **After Record Submit** trigger. You can also create a condition so the workflow instance only runs on lead records with customer category of **Individual**.

The following screenshot shows the lead nurturing workflow:

![A sample workflow depicting the lead nurturing workflow, with the Record Type, Initation, and Event Definition settings highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/EventBasedInitiation.png)

## Workflow Initiation Triggers {#bridgehead_4108930105}

For a workflow to initiate on a create or update event on a record, you must also set the initiation trigger type in the **Trigger Type** dropdown list.

The following table describes when the workflow initiates for each trigger type:

| Trigger Type | Description |
| --- | --- |
| \- All - | The workflow initiates for any triggering event. For example, the workflow initiates when a record is viewed because the Before Record Load trigger executes when the record is viewed. Best practice is to choose a more specific trigger type for workflow initiation because the workflow initiates for any action on the record with this trigger. |
| Before Record Load | The workflow initiates and the record goes into the entry state when you load a record by clicking **New** or **Edit**, or when you view the record. |
| Before Record Submit | The workflow initiates and the record goes into the entry state after you click **Save** on the record and before NetSuite writes the record data to the database. |
| After Record Submit | The workflow initiates and the record goes into the entry state after the NetSuite writes the record data to the database. |

Note:

For more information, see [Server Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html#bridgehead_4074679460) and [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).

### Related Topics

-   [Workflow Initiation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4080797941.html)
-   [Initiating a Workflow on a Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2730900.html)
-   [Using SuiteScript to Initiate a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2731126.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
