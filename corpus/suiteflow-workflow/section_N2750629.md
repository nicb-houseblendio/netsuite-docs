---
id: "section_N2750629"
type: "section"
title: "Set Field Display Type Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Set Field Display Type Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2750629.html"
anchors: ["bridgehead_4149497882"]
sha256: "f7107d9b663b2dd4c3ed3aaa9ff2c31232e96c91dca298e5a340934ff51d2240"
---

Use the Set Field Display Type action to change a field's display type. For example, use this action in an approval workflow to either disable the approval field, set it to inline, or hide it so only the current approver can modify the field.

For more information about executing the action dynamically if the record meets certain conditions, see [Using Conditional Fields with Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103786961.html).

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Set Field Display Type action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Set Field Display Type Action Parameters {#bridgehead_4149497882}

The following table describes the Set Field Display Type action parameters:

| Parameter | Description |
| --- | --- |
| Body | Select to run the action on one of the fields in the main body of the workflow's base record type. |
| Sublist | Select to run the action on one of the sublists in the workflow's base record type. If selected, choose the correct sublist from the list. |
| Field | Name of the field on which to change the display type. |
| Display Type | Select one of the following display type options:
-   **Hidden.** Field cannot be seen on the record or transaction.
-   **Inline.** Used for informational purposes only. Cannot be edited.
-   **Disabled.** Field cannot be edited.
-   **Normal.** The field is editable.

For more information about each of the display types, see [Setting Display Options for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830238.html). |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Using Conditional Fields with Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103786961.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
