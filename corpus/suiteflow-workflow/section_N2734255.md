---
id: "section_N2734255"
type: "section"
title: "Exit States"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > States Reference > Exit States"
parent: "section_4103784416"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2734255.html"
anchors: ["bridgehead_4153137525", "bridgehead_4153056311"]
sha256: "686990f726a3541f0294e346a376a1b4523bec741da36f2ecee7800bd630cada"
---

An exit state in a workflow is the final state the record enters before a workflow completes. Depending on the layout of a workflow, a single workflow may have multiple exit states. The diagrammer designates any state without a transition to another state as an **End**, or exit, state.

The following screenshot shows a workflow with two exit states, **State 3b Approved** and **State 4 Rejected**:

![An example of a workflow with two exit states.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/StateReferenceEndStates.png)

The diagrammer removes the **End** state designation when you create a transition from an exit state to another state or you enable the **Do Not Exit Workflow** property on the state.

## Trigger Execution in Exit States {#bridgehead_4153137525}

NetSuite only executes the actions for the server trigger on which a record entered an exit state and then completes the workflow. Subsequent server triggers do not run.

For example, if a record enters an exit state on a Before Record Load trigger, only actions set to trigger on Entry or Before Record Load run. Then, the record exits the workflow. The Before Record Submit and After Record Submit triggers do not run. For more information about the order of trigger execution in a state, see [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).

You can use one of the following methods to control which actions may run in an exit state:

-   Enable the **Do Not Exit Workflow** property for the state. Consequently, the record stays in the state and the workflow never completes.
    
-   Create a new state as the exit state. On the transition into the new exit state, set the trigger for the transition to a trigger that allows the actions in the exit state to run. For example, if you have actions that trigger on After Record Submit, make sure the transition into the state uses the Before Record Submit or After Record Submit trigger.
    

## Exit State Guidelines {#bridgehead_4153056311}

Important:

Use the following guidelines when working with exit states.

Scheduled actions do not run in the exit state. The workflow completes and leaves the exit state before scheduled actions can run. See [Scheduling an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103059488.html).

### Related Topics

-   [States Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103784416.html)
-   [Workflow States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071953710.html)
-   [Working with States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103045609.html)
-   [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
