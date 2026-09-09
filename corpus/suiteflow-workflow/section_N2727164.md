---
id: "section_N2727164"
type: "section"
title: "Step 6 Create a Transition"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Creating Your First Workflow > Step 6 Create a Transition"
parent: "chapter_N2725813"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2727164.html"
anchors: []
sha256: "cf5ec2426e9bff3ebb4dbbce217dfcd3b26c8e4fe091ec9f40a41b7929d6582c"
---

This step shows you how to create and edit a transition. You can use the diagrammer to drag and drop a transition between states and then edit the transition properties. Any changes made in the diagrammer are immediately saved.

In this step, you will create a transition between **State 1 Entry** and **State 2 See Opportunities** that executes after an opportunity record is saved for the first time.

#### To create and edit a transition:

1.  If you haven't already, complete [Step 5 Create Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726890.html).
    
2.  In the diagrammer, hover over the **End** icon on **State 1 Entry**. The cursor becomes a filled half-circle.
    
3.  Drag and hover over **State 2 See Opportunities**. The following screenshot shows how the cursor becomes an arrow and you can drag it to the required state:
    
    ![The cursor becoming an arrow that you can drag after you hover over the End icon.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/TutorialStep6ClickAndDrag.png)
    
    The diagrammer creates a transition when you release the mouse and **State 2 Opportunities** becomes the new exit (End) state. You can also click and drag the states to new locations. The following screenshot shows a transition between state 1 and state 2:
    
    ![A transition between state 1 and state 2. State 1 is the start of the workflow and state 2 is the end of the workflow.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/TutorialStep6DiagrammerFinal.png)
    
    Note:
    
    You can also create and edit a transition by editing the state properties for the state that you want to transition from and clicking the **New Transition** button.
    
4.  Select the transition in the diagrammer and click the **Edit** icon in the context panel.
    
5.  In the **Workflow Transition** window, select **After Record Submit** for the **Transition On** property.
    
6.  Click **Save**.
    
7.  Make sure that the transition in the context panel matches the following screenshot:
    
    ![A view of the Transition tab on the context panel that shows a transaction on the After Record Submit action. Edit and delete icons are located to the right of the transition information.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/TutorialStep6TransitionFinal.png)
8.  To continue with the tutorial, proceed to [Step 7 Initiate and Validate the Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2727383.html).
    

### Related Topics

-   [Creating Your First Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2725813.html)
-   [Step 1 Define Workflow Basic Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726220.html)
-   [Step 2 Define Workflow Initiation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726358.html)
-   [Step 3 Define the Workflow Condition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726518.html)
-   [Step 4 Create Workflow States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726745.html)
-   [Step 5 Create Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726890.html)
-   [Step 7 Initiate and Validate the Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2727383.html)
-   [Workflow Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954244.html)
-   [Working with Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103063317.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
