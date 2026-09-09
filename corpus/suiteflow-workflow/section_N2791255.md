---
id: "section_N2791255"
type: "section"
title: "Canceling a Single Workflow Instance"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Administration > Canceling a Single Workflow Instance"
parent: "chapter_4103088279"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2791255.html"
anchors: []
sha256: "ea06250b5f7f0e73642195007a6b608621a23397ae5b43427b74279394e64d8b"
---

You can cancel a single workflow instance from the record on which the workflow instance runs. Users with the Administrator role can cancel workflow instances. You can also cancel multiple workflow instances simultaneously. See [Mass Canceling Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103260636.html).

Important:

When you cancel a workflow instance for a single record, NetSuite reloads the record. Therefore, when a workflow is set to initiate **On Update** and uses the All or Before Record Load server triggers, the workflow instance re-initiates when you cancel it. To avoid this, use the Before Record Submit or After Record Submit server triggers on workflows set to initiate **On Update**. Mass canceling workflow instances doesn't have this limitation.

#### To cancel a single workflow instance:

1.  Edit or view the record on which the workflow instance runs.
    
2.  Click the **Workflow** subtab. The **Active Workflows** subtab appears by default.
    
3.  Click **Cancel** next to the workflow instance that you want to cancel.
    
    ![A portion of the Active Workflows subtab showing an example of the Cancel button, which is located on the far right of the screen on each line for every active workflow.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/CancelSingleWorkflowInstance.png)
    
    Note:
    
    Any other workflow instances still run; you must cancel each one individually.
    
4.  Click **Yes** in the popup.
    
5.  Optionally, click the **Workflow History** subtab to see the canceled instance. The **Notes** column displays the name of the user who canceled the instance.
    

### Related Topics

-   [Workflow Administration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4103088279.html)
-   [Workflow Instance and History Record Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1562606255.html)
-   [Workflow Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103089023.html)
-   [Workflow Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2796043.html)
-   [Bundling a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103266281.html)
-   [Editing a Locked Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4846726513.html)
-   [Mass Canceling Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103260636.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
