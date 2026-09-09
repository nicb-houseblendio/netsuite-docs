---
id: "section_N2741165"
type: "section"
title: "Create Record Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Create Record Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2741165.html"
anchors: ["bridgehead_4144454046", "bridgehead_4144467366"]
sha256: "e5712dcc73e9c22b274218398679d0ddb5cca5225cd8fba1d55cc853bf892a75"
---

Use the Create Record action to create a new record in NetSuite. The record can be a standard NetSuite record or a custom record. The record doesn't need to be the same record type as the base record type for the workflow. You can use this action to create a follow up record that is part of a business process. For example, a workflow with lead as the base record type can use the Create Record action to create call record as soon as the lead is saved.

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Create Record action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Create Record Action Parameters {#bridgehead_4144454046}

When you configure the Create Record action, you specify the record type and the field values of the new record instance.

The following table describes the Create Record action parameters:

| Parameter | Description |
| --- | --- |
| Record Type | Type of record the action will create. |
| Store Result In | Workflow or state field where you can store a reference to the created record. To use this option you must first create the workflow or state field. See [Workflow Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071955161.html) Use this field to subscribe to a created record with the Subscribe To Record action. See [Creating and Subscribing to a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4144476357.html). |
| Field | Field values to populate in the record created by the action. The available fields change dynamically depending on the type of record selected in the **Record Type** dropdown list. For each field, select the field name, set the appropriate properties in the other columns, and click **Add**. For more information, see [Setting Field Values in Action Definitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103787257.html) |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

## Create Record Action Guidelines {#bridgehead_4144467366}

Use the following guidelines when working with the Create Record action:

-   When configuring the Create Record action, you must set values for all the required fields for the selected **Record Type** parameter. To verify the required fields, open the record type's create new record screen in the NetSuite UI and note which fields are necessary. If you do not set all required fields, the Create Record action fails.
    
-   The Create Record action is not available on a Before Record Load trigger for a time entry record.
    

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating and Subscribing to a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4144476357.html)
-   [Setting Field Values in Action Definitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103787257.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
