---
id: "section_N2752089"
type: "section"
title: "Custom Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Custom Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2752089.html"
anchors: ["bridgehead_0306113804", "bridgehead_0307042808", "bridgehead_4150524508"]
sha256: "03ab9c1301be19b14a6f07d658d5adc3645e28d95fa2cfd2e62704897704c776"
---

Use the Custom action to define an action with a SuiteScript Workflow Action script. The SuiteScript script will define the Custom action's behavior. Therefore, to use a Custom action in a workflow, first you will need to develop and deploy a SuiteScript Workflow Action script.

For information about SuiteFlow Workflow Action scripts and to see sample code, see [SuiteScript 2.1 Workflow Action Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460429314.html).

## To create a custom action {#bridgehead_0306113804}

1.  Create and deploy a Workflow Action script to define the action's functionality.
    
2.  In the Workflow Manager, create a new action. The custom action only appears if the Workflow Action script was deployed for the base record type of the workflow. Workflow Action scripts display in the New Action's Type section with the **(Custom)** identifier:
    
    ![Image of the New Action window for a Workflow Action script called Workflow Line Item.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/NewActionCustomActionV2.png)

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Custom action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Custom Action Parameters {#bridgehead_0307042808}

The following table describes the Custom action parameters:

| Parameter | Description |
| --- | --- |
| Store Result In | A workflow or state field where you can store the Workflow Action script return value. To use this option you must first create the workflow or state field. See [Workflow Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071955161.html) |
| Field | Parameter fields that are defined in the Workflow Action script deployment record. Here you can assign values to these fields so you can access them in the Workflow Action script using the SuiteScript N/runtime module. For more information, see [N/runtime Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296359529.html). |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

## Custom Action Guidelines {#bridgehead_4150524508}

Use the following guidelines when working with Custom actions:

-   For a Custom action to be available to all workflows, set the **Applies To** field on the deployment record of the Workflow Action script to **All Records**.
    
-   Custom actions are skipped in workflows initiated by users not included in the custom script's audience. The skipped action scripts are listed in the [Workflow Execution Log](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4472471134.html).
    
-   Check out this example of storing a return value from a **Workflow Action** script in a workflow: [Storing a Return Value from a Custom Action Script in a Workflow Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2807069.html).
    

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [SuiteScript 2.1 Workflow Action Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460429314.html)
-   [Storing a Return Value from a Custom Action Script in a Workflow Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2807069.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
