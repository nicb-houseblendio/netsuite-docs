---
id: "section_N2734116"
type: "section"
title: "Non-Exiting Workflow States"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > States Reference > Non-Exiting Workflow States"
parent: "section_4103784416"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2734116.html"
anchors: []
sha256: "1d3323e5d8114e68439a06e1e3ee6c4b4edaca77190843d709c29a336b58c038"
---

Use non-exiting states to run a workflow indefinitely. You can set a state that has no transitions as a non-exiting state with the **Do Not Exit Workflow** property. The diagrammer shows non-exiting states with a circular arrows icon:

![A portion of the workflow diagrammer with the non-exiting states icon highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/StateReferenceNonExitingState.png)

Note:

If you create a transition from the state, the **Do Not Exit Workflow** property is unchecked. In addition, the property cannot be set if a state has any transitions.

Use non-exiting states in the following types of workflows:

-   Single state workflows. Use the state to run an action or actions any time a record of a specific type is created or edited.
    
-   Approval-based workflows. For example, after a request has been rejected, set the record to enter a non-exiting state with a Lock Record action. If a user or specific group of users accesses the record, the record cannot be edited.
    

### Related Topics

-   [States Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103784416.html)
-   [Workflow States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071953710.html)
-   [Working with States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103045609.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
