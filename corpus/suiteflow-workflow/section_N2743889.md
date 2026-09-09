---
id: "section_N2743889"
type: "section"
title: "Show Message Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Show Message Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2743889.html"
anchors: ["bridgehead_4150441827"]
sha256: "0e0d0fd05920f09d37a8ea1ab3226dd49eb2d14d0ff60d6145f0c021b751d40c"
---

Use the Show Message action to display a message to the user, such as when you want to validate values entered on a record form. The action displays the message in a popup window with an **OK** button. Unlike the Return User Error or Confirm actions, the Show Message action does not prevent subsequent user actions on the record form.

The following screenshot shows the behavior of the Show Message action:

![A screenshot showing an example of a Show Message action displaying a message based on user input.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/ShowMessageActionExample.png)

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Show Message action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Show Message Action Parameters {#bridgehead_4150441827}

The following table describes the Show Message action parameters:

| Parameter | Description |
| --- | --- |
| Text | Text to display in the browser popup when the action executes. If the Multi-Language feature is enabled on your account, you can add label translations. For more information, see [Configuring Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N247147.html) |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Confirm Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2744159.html)
-   [Return User Error Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2745741.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
