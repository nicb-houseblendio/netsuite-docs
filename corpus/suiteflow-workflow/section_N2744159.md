---
id: "section_N2744159"
type: "section"
title: "Confirm Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Confirm Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2744159.html"
anchors: ["bridgehead_4144428834"]
sha256: "06ccabd8cf7ce7d7145b9fe094df55d3451fecd979b843e94b11942293147c83"
---

Use the Confirm action to display a popup message with **OK** and **Cancel** buttons. A user can acknowledge the message and continue working or cancel the previous activity.

The Confirm action supports the Before Field Edit and Before User Submit client triggers. The behavior of the Confirm action buttons depends on which trigger you use:

| Client Trigger | Button Behavior |
| --- | --- |
| Before Field Edit | 
-   **OK.** The field value remains set.
-   **Cancel.** The field value reverts to the previous value.

 |
| Before User Submit | 

-   **OK.** NetSuite saves the record.
-   **Cancel.** NetSuite does not save the record. The user can continue editing the record.

 |

The following screenshot shows the Confirm action on a Before User Submit trigger:

![Image of a Sales Order record with the Confirm action message displayed. The Confirm action message asks users to confirm that they want to save the record and includes the options to proceed with the action or cancel it.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/ConfirmActionExample.png)

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Confirm action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Confirm Action Parameters {#bridgehead_4144428834}

The following table describes the Confirm action parameters:

| Parameter | Description |
| --- | --- |
| Text | Text to appear in the popup window when the Confirm action executes. The field accepts a maximum of 999 characters. If the **Multi-Language** feature is enabled on your account, you can add label translations. For more information, see [Configuring Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N247147.html) |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Return User Error Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2745741.html)
-   [Show Message Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2743889.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
