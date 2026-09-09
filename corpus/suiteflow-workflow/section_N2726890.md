---
id: "section_N2726890"
type: "section"
title: "Step 5 Create Actions"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Creating Your First Workflow > Step 5 Create Actions"
parent: "chapter_N2725813"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726890.html"
anchors: []
sha256: "fa61dc4934c90e35a142db525359046994a548525f56f01dbf00476c6d44412a"
---

This step shows you how to use the **Workflow State** window to add actions to a state. The actions you add to each state run based on their triggers when the record enters that state in the workflow.

In this step, you will add a Set Field Mandatory action in **State 1 Entry** and a Go To Page action in **Step 2 See Opportunities**.

#### To create the actions in the workflow states:

1.  If you haven't already, complete [Step 4 Create Workflow States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726745.html).
    
2.  To create a new action for **State 1 Entry**, in the workflow diagrammer, double-click **State 1 Entry** and click the New Action button in the **Workflow State** window.
    
3.  Click **Set Field Mandatory**.
    
4.  In the **Workflow Action** window, set the following properties:
    
    | Property | Value |
    | --- | --- |
    | **Trigger On** | Entry |
    | **Field**, in the **Parameters** section | Title |
    | **Mandatory**, in the **Parameters** section | Checked |
    
5.  Click **Save**.
    
6.  Make sure that the action in the context panel matches the following screenshot:
    
    ![A view of the context panel that shows the Set Field Mandatory action added to the first state. Trigger On is set to Entry. Under Entry, the formula Set Field Mandatory title equals true is listed.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/TutorialStep5SetFieldMandatory.png)
7.  Repeat step 2 to access the **New Action** window for **State 2 See Opportunities**.
    
8.  Click **Go To Page**.
    
9.  Set the **Trigger On** field to **Entry**.
    
10.  Under **Parameters**, in the **Target Page** field, enter **Opportunities** and select **Opportunities** in the dropdown list that appears.
     
11.  Click **Save**.
     
12.  Make sure that the action in the context panel matches the following screenshot:
     
     ![A view of the context panel that shows the Go to Page action added to the second state. Trigger On is set to Entry. Under Entry, the parameter is set to open the Opportunities page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/TutorialStep5GoToPageFinal.png)
13.  To continue with the tutorial, continue to [Step 6 Create a Transition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2727164.html).
     

### Related Topics

-   [Creating Your First Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2725813.html)
-   [Step 1 Define Workflow Basic Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726220.html)
-   [Step 2 Define Workflow Initiation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726358.html)
-   [Step 3 Define the Workflow Condition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726518.html)
-   [Step 4 Create Workflow States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726745.html)
-   [Step 6 Create a Transition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2727164.html)
-   [Step 7 Initiate and Validate the Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2727383.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Working with Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103048460.html)
-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
