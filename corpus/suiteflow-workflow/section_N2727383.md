---
id: "section_N2727383"
type: "section"
title: "Step 7 Initiate and Validate the Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Creating Your First Workflow > Step 7 Initiate and Validate the Workflow"
parent: "chapter_N2725813"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2727383.html"
anchors: []
sha256: "4bbb53d00115cc47d5acec51aca0182924fa53ac6f324909e08eef37867da8a3"
---

This step shows you how to initiate the workflow by creating an Opportunity record. After a user creates and saves an opportunity with a status of **In Discussion**, **In Negotiation**, **In Progress**, and **Qualified**, NetSuite initiates an instance of the workflow on the record.

Use the behavior of NetSuite and the workflow activity information to validate the tasks performed by the workflow.

#### To initiate and validate the First Workflow workflow:

1.  If you haven't already, complete [Step 6 Create a Transition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2727164.html).
    
2.  Go to Transactions > Sales > Create Opportunities. A new Opportunity record form opens:
    
    -   The default value of the **Opportunity Status** field on an opportunity is **Qualified**, so the initiation condition for the workflow was met.
        
    -   The **Title** field appears with an asterisk, indicating it is a required field. This indicates that the record entered **State 1 Entry** in the workflow and the Set Field Mandatory action executed.
        
3.  On the Opportunity record form, select a company, enter a value in the **Title** field, and click **Save**.
    
    The Opportunities list page appears, indicating the After Record Submit trigger executed, the record transitioned to **State 2 See Opportunities**, and the Go To Record action executed.
    
4.  On the Opportunities list page, open the recently created opportunity, click the **System Information** subtab, and then click the **Workflow History** subtab.
    
    The **Workflow History** subtab shows the two states for the workflow, the date and time each state was entered and exited by the workflow, and the workflow execution log for each state:
    
    ![The Workflow history tab, which shows the two states of the workflow, the date and time each state was entered and exited by the workflow, and the workflow execution log for each state.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/TutorialStep7WorkflowHistorySubtab.png)
5.  Click **Log** for **State 1 Entry**. The workflow execution log shows the triggers, actions, and transitions executed:
    
    ![An example of the workflow execution log and the types of information found there.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/TutorialStep7WorkflowHistorySubtab_19.1.png)
    
    Note:
    
    If the workflow does not run as expected, you can use the workflow execution log to troubleshoot issues.
    

### Related Topics

-   [Creating Your First Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2725813.html)
-   [Step 1 Define Workflow Basic Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726220.html)
-   [Step 2 Define Workflow Initiation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726358.html)
-   [Step 3 Define the Workflow Condition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726518.html)
-   [Step 4 Create Workflow States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726745.html)
-   [Step 5 Create Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726890.html)
-   [Step 6 Create a Transition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2727164.html)
-   [Workflow Initiation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4080797941.html)
-   [Testing a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2786153.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
