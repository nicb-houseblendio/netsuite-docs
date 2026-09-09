---
id: "section_N2786649"
type: "section"
title: "Testing Actions and Transitions"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Testing and Troubleshooting Workflows > Testing a Workflow > Testing Actions and Transitions"
parent: "section_N2786153"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2786649.html"
anchors: ["bridgehead_N2786821", "bridgehead_N2786904"]
sha256: "1ddd86cf4a36a0182396cbc8d1bade4de5f3da773d46aca645a43b520942ee53"
---

When you test a workflow, review the workflow execution log to see which actions and transitions did or didn't process during the run of your workflow. Based on log details, you can make changes to the workflow to resolve issues with actions or transitions. For more information about the workflow execution log, see [Workflow Execution Log](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4472471134.html).

Actions and transitions can have one the following statuses:

-   Executed
    
-   Failed
    
-   Skipped
    
-   Considered
    

In addition, an event or transition may not appear in the log because they didn't run. SuiteFlow will only attempt to process actions of the appropriate trigger type. Make sure that you understand triggers and the Suiteflow triggering model. For more information, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html).

## Tip {#bridgehead_N2786821}

To test the execution of one specific action within a state, set all other actions in the state to **Inactive**. For each action, select the **Inactive** box on the action definition page and save the action. After you test, you can re-activate the actions. You can also change the trigger type for the action to make sure the action trigger type didn't cause the failure.

## Skipped Actions {#bridgehead_N2786904}

When SuiteFlow skips an action, it may be because that action isn't supported for the server trigger on which the workflow entered the state.

The following screenshot shows a record that entered a state on a Before Record Load trigger and consequently, the Send Email action was skipped:

![A portion of the workflow execution log that highlights that the Send Email action was skipped.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/SkippedSendEmailAction.png)

You can view the options for the Send Email trigger on the Send Email action definition page in the **Trigger On** dropdown list:

![A portion of the Send Email action definition page with the Trigger On options highlighted. Options include Entry, Exit, After Record Submit, and Scheduled.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/SendEmailTrigger.png)

This action can be executed on any of the four triggers listed, depending on the server trigger on which the record enters the state. Since Before Record Load isn't an option for the action, the workflow skips the action when running ONENTRY trigger under BEFORELOAD.

Note:

The absence of the Before Record Load trigger type for the Send Email action means that even with the trigger type set to Entry or Exit, this action will be skipped if the record enters the state on a Before Record Load or Before Record Submit trigger.

### Related Topics

-   [Testing a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2786153.html)
-   [Setting Up a Workflow for Testing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471802671.html)
-   [Testing Workflow Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2786511.html)
-   [Testing Buttons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471796885.html)
-   [Testing a Send Email Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4472473260.html)
-   [Testing Scheduled Workflows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3873172773.html)
-   [Testing Scheduled Actions and Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4472474105.html)
-   [Testing for User Accessibility](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2787197.html)
-   [Testing and Troubleshooting Workflows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2786070.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Workflow Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954244.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
