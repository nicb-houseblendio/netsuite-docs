---
id: "section_N2726518"
type: "section"
title: "Step 3 Define the Workflow Condition"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Creating Your First Workflow > Step 3 Define the Workflow Condition"
parent: "chapter_N2725813"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726518.html"
anchors: []
sha256: "4f65f1183b6cc5bd3270170bffa7496c9ee9f1cabe988810915f7a3dc93f732c"
---

This step shows you how to use the Condition Builder in the Workflow Manager to define a condition for a workflow initiation. An instance of the workflow only initiates for records that meet the condition.

#### To define a condition for workflow initiation:

1.  If you haven't already, complete [Step 2 Define Workflow Initiation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726358.html).
    
2.  On the workflow definition page, make sure Visual Builder is selected and click the open icon to open the Condition Builder. The following screenshot shows the location of the open icon:
    
    ![The open icon is located to the right of the Condition Builder field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/ConditionBuilderButton.png)
3.  In the **Workflow Condition** window, enter the following details:
    
    | Property | Value |
    | --- | --- |
    | **Field** | Opportunity/Estimate Status |
    | **Compare Type** | any of |
    
4.  In the **Selection** column, click the Selection box, then click the **Select Multiple** button.
    
    ![The Workflow Condition window, with the Select Multiple button highlighted. The Select Multiple button is located to the right of the Selection field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/TutorialStep3ConditionSelectMultiple.png)
5.  In the **Choose Selection** window, in the **Click Selection to Add** column, select **In Discussion**, **In Negotiation**, **In Progress**, and **Qualified**.
    
    ![The Choose Selection window. Qualified is highlighted in the Click Section to Add column. The Current Selections column includes the In Discussion, In Negotiation, In Progress, and Qualified selections.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/TutorialStep3ConditionChooseSelection.png)
6.  Click **Done**.
    
7.  In the **Workflow Condition** window, click **Add**.
    
    ![The Workflow Condition window with Opportunity/Estimate Status selected in the Field column. Any of is selected in the Compare Type column. In Discussion, In Negotiation, In Progress, and Qualified are listed in the Selection column. The Add button is highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/TutorialStep3ConditionBuilder.png)
8.  Click **Save**. Make sure that the workflow properties look like the following screenshot:
    
    ![The workflow definition page, in the Event Definition section, the Condition field is populated with the formula Opportunity/Estimate Status equals In Discussion, In Negotiation, In Progress, and Qualified.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/TutorialStep3ConditionFinalCondition.png)
9.  Click **Save** to save the workflow. The workflow diagrammer and context panel appears.
    
10.  To continue with the tutorial, continue to [Step 4 Create Workflow States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726745.html).
     

### Related Topics

-   [Creating Your First Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2725813.html)
-   [Step 1 Define Workflow Basic Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726220.html)
-   [Step 2 Define Workflow Initiation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726358.html)
-   [Step 4 Create Workflow States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726745.html)
-   [Step 5 Create Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726890.html)
-   [Step 6 Create a Transition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2727164.html)
-   [Step 7 Initiate and Validate the Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2727383.html)
-   [Workflow Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954369.html)
-   [Working with Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103074843.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
