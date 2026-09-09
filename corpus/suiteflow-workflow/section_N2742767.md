---
id: "section_N2742767"
type: "section"
title: "Go To Record Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Go To Record Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2742767.html"
anchors: ["bridgehead_4146259351", "bridgehead_4146445266"]
sha256: "1345d564c6004954825c59fc6afc31cd323687bf7167de4e803ad2e51c65e91d"
---

Use the Go To Record action to redirect users to a record in NetSuite. The record type to redirect to does not have to be the same record type as the workflow's base record type.

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Go To Record action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Go To Record Action Parameters {#bridgehead_4146259351}

The following table describes the Go To Record action parameters and the values you must use to create a record or redirect to a specific record:

| Parameters | Description |
| --- | --- |
| Record Type | Type of record to redirect to. The available fields in the table change dynamically depending on the **Record Type** selection. |
| Open in edit mode | When selected, the record the user is redirected to, opens in edit mode. This property only applies if you specify a value in the **Record ID** field. |
| Record (Join Field) | Use this field to use a join to get the ID of a record to redirect to. Select the record type to create the join from, and the **Value Field** to use from the selected record type. |
| Field | Field values to populate when creating the record on redirection. For each field, select the field name, set the appropriate field value in the applicable column, and click **Add**. For more information, see [Setting Field Values in Action Definitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103787257.html). |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

## Go To Record Action Guidelines {#bridgehead_4146445266}

Use the following guidelines when working with the **Go To Record** action.

-   You're unable to set field values on an existing record if the Go To Record action executes on a Before Record Load trigger. Instead, use a Custom action to update fields on an existing record, and then head to the record with the Go To Record action after it's updated. Instead, use a Custom action to update fields on an existing record, and then head to the record with the Go To Record action after it's updated.
    
-   If you're not using the field definition area to set field values, you're able to add a URL parameter like `record.{field}={value}` on any SuiteScript-supported record, and the system will set up that field, the same as calling `setFieldValue` in a before load event handler.
    
-   The Go To Record action is not available on a Before Record Submit or After Record Submit trigger for a time entry record.
    

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Go To Page Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2742608.html)
-   [Setting Field Values in Action Definitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103787257.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
