---
id: "section_N2750923"
type: "section"
title: "Set Field Required Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Set Field Required Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2750923.html"
anchors: ["bridgehead_4149498337", "bridgehead_0318111955"]
sha256: "7ce24935496b99ab80509e4b59942f1cd9be0c1cbbfec04bba377b2360fd6e78"
---

Use the Set Field Required action to set whether a record form field is required or not. Required fields in NetSuite appear with an orange asterisk next to the field name. For more information about executing the action dynamically if the record meets certain conditions, see [Using Conditional Fields with Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103786961.html).

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Set Field Required action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Set Field Required Action Parameters {#bridgehead_4149498337}

The following table describes the Set Field Required action parameter:

| Parameter | Description |
| --- | --- |
| Body | Select to run the action on one of the fields in the main body of the workflow's base record type. |
| Sublist | Select to run the action on one of the sublists in the workflow's base record type. If selected, choose the correct sublist from the list. |
| Field | Name of the field on which to change the required configuration. |
| Mandatory | Makes the field required. |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

## Set Field Required Action Guidelines {#bridgehead_0318111955}

If you use the Set Field Required action on a box field, NetSuite does not make the field required on the record form when you save the record.

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Using Conditional Fields with Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103786961.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
