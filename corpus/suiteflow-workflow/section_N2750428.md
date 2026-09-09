---
id: "section_N2750428"
type: "section"
title: "Set Field Display Label Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Set Field Display Label Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2750428.html"
anchors: ["bridgehead_4149498055"]
sha256: "8b7473236abf58159fdc80c7bf4eff39ab567b17d8ac9c53acb616a43ff7b985"
---

Use the Set Field Display Label action to change the UI label of a Sublist Action Group supported sublist. For more information regarding Sublist Action Group supported sublists, see [Using Sublist Action Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1513354324.html).

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Set Field Display Label action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Set Field Display Label Action Parameters {#bridgehead_4149498055}

The following table describes the Set Field Display Label action parameters:

| Parameter | Description |
| --- | --- |
| Body | Select to run the action on one of the fields in the main body of the workflow's base record type. |
| Sublist | Select to run the action on one of the sublists in the workflow's base record type. If selected, choose the correct sublist from the list. |
| Field | Name of the field on which to change the label. |
| Label | String to use to replace the default UI label. If the Multi-Language feature is enabled on your account, you can add label translations. For more information, see [Configuring Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N247147.html) |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Using Conditional Fields with Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103786961.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
