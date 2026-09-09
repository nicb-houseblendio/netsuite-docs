---
id: "section_N2745741"
type: "section"
title: "Return User Error Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Return User Error Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2745741.html"
anchors: ["bridgehead_4147132243", "bridgehead_4147132465"]
sha256: "fea31b53799e70b7c8a371543de8cd934a289bba963a3b7293a05586606594f6"
---

Use the **Return User Error** action to display an error message to users. Use this action with field or record validation to prevent the user from saving the record with invalid data. To create the **Return User Error** action, create validation conditions on the action definition.

How the error message displays depends on the type of trigger used in the action definition:

| Trigger Type | Use Case | Error Message Format |
| --- | --- | --- |
| Before Record Load | Validate record form field values before the record loads in the browser. | Displays as browser page with a **Go Back** button. |
| Any client trigger | Validate record form field values as user interacts with the record form fields. | Displays as popup window with an **OK** button. |
| Before Record Submit | Validate record form field values after the user clicks **Save**. | Displays as browser page with a **Go Back** button. |

The following screenshot shows the Return User Error action on a client trigger:

![An image of the execution of the Return User Error action on a client trigger. The error message says that the Customer Rank cannot be greater than 10.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/ReturnUserErrorActionClient.png)

The following screenshot shows the Return User Error action on a server trigger:

![The execution of the Return User Error action on a server trigger.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/ReturnUserErrorActionServer.png)

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Return User Error action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Return User Error Action Parameters {#bridgehead_4147132243}

The following table describes the Return User Error action parameters:

| Parameter | Description |
| --- | --- |
| Text | The error message text. If the Multi-Language feature is enabled on your account, you can add text translations. For more information, see [Configuring Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N247147.html) |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

## Return User Error Action Guidelines {#bridgehead_4147132465}

Use the following guidelines when working with the Return User Error action.

-   It's smoother to use client-side triggers to catch errors on individual fields as they're entered, instead of server-side triggers on save. With server-side triggers, the user has to re-enter all data since the last successful save.
    
-   The **Return User Error** action is not available on a Before Record Load trigger for a time entry record.
    
-   When the user clicks **Go Back**, all field values entered since the record was last saved are removed.
    

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Confirm Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2744159.html)
-   [Show Message Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2743889.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
