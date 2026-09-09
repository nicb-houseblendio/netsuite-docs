---
id: "section_N2743465"
type: "section"
title: "Initiate Workflow Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Initiate Workflow Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2743465.html"
anchors: ["bridgehead_4146943699", "bridgehead_4146944529"]
sha256: "419b54c86275ece8e5b01c5c32624e62d1bb016143cea9e96813e019642eb275"
---

Use the Initiate Workflow action to initiate another workflow instance (child) from the current workflow instance (parent). The child workflow must be active and match the same base record type as the parent workflow. Plus, the child workflow initiated by the parent workflow runs on the same record instance as the parent. For example, if the parent workflow runs on a purchase order, the actions in the child workflow run on the same purchase order instance.

You can also use the completion of a child workflow as a transition trigger in the parent workflow. Select the child workflow on the transition's **Wait for Workflow** field.

For more information about the best practices to follow when using the Initiate Workflow action, see [SuiteFlow Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540490044.html) and [Specifying States for Child Workflow Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103799214.html).

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Initiate Workflow action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Initiate Workflow Action Parameters {#bridgehead_4146943699}

The following table describes the Initiate Workflow action parameters:

| Parameters | Description |
| --- | --- |
| Workflow | Name of the workflow definition to initiate when the action executes. |
| Field | A list of workflow fields available in the child workflow. You can pass values from the parent workflow to the workflow fields belonging to the child. These values can be either static or set through a join. |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

## Initiate Workflow Action Guidelines {#bridgehead_4146944529}

Use the following guidelines when working with the Initiate Workflow action.

-   The Initiate Workflow action is not available on a Before Record Load trigger for a time entry record.
    
-   For more information about the best practices to follow when using the Initiate Workflow action, see [SuiteFlow Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540490044.html) and [Specifying States for Child Workflow Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103799214.html).
    

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Specifying States for Child Workflow Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103799214.html)
-   [Setting Field Values in Action Definitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103787257.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
