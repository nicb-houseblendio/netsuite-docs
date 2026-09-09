---
id: "section_N2751166"
type: "section"
title: "Set Field Value Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Set Field Value Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2751166.html"
anchors: ["bridgehead_4150383163", "bridgehead_4150381800"]
sha256: "f9f7b637044e3ca3bf5c6ef016cbd8abe80c5da0d7beed831fa9fb73b4fa2df7"
---

Use the Set Field Value action to set the value in a field in the workflow's base record type and sub types. Typically, this action is used to set the value of a field as a record enters a state.

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Set Field Value action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Set Field Value Action Parameters {#bridgehead_4150383163}

The following table describes the Set Field Value action properties:

| Property | Description |
| --- | --- |
| Field | Name of the field of the base record type and sub types of the workflow on which to set the value. |
| Static Value | Set a static value in the field. Use one of the following options:
-   **Text:** Use for free form text fields. Enter the value in the **Text** field.
-   **Checked:** Use with checkbox fields.
-   **Selection:** Select a value or values from the **Selection** list. For multi-select fields, this option only applies for new records. See [Set Field Value Action Guidelines](#bridgehead_4150381800).

 |
| Date | Select a date range when setting a value in a date field. |
| From Field | Sets, in the selected **Field**, the value of a different field from the current record, or from a different record using a join. Set the following options:

-   **Record (Join Field):** The record from which you will pick the field to get the value to set.
-   **Field:** The field from which to get the value to set.

 |
| Formula | Use the Formula Builder to create a formula used to derive the field value. For client triggers, use a JavaScript or SuiteScript formula. For server triggers, use an SQL formula. See [Defining a Condition with Formulas](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103077064.html). |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

## Set Field Value Action Guidelines {#bridgehead_4150381800}

Use the following guidelines when working with the Set Field Value action.

-   You cannot use a Before Record Load trigger to set field values for existing records. Use a custom action to update fields on an existing record.
    
-   The value you specify in a Set Field Value action on a Before Record Load trigger does not override a stored custom field or a field sourced from another record. To set this type of field, use a client trigger.
    
-   Records must be in edit mode to enable you to set field values using the Set Field Value action.
    
-   If you set the value of a multi-select field, the new values replace all the values in the target field.
    
-   You cannot use the Set Field Value action to set the External ID of a record. External IDs are designed to be used as references in NetSuite. If setting the Internal ID is not sufficient for your business needs, you must create a custom field to set the External ID.
    
-   To run the action dynamically if the record meets certain conditions, see [Using Conditional Fields with Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103786961.html).
    

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Using Conditional Fields with Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103786961.html)
-   [Using Conditional Fields with Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103786961.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
