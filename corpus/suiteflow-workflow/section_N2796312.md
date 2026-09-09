---
id: "section_N2796312"
type: "section"
title: "Mass Processing Records in a Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Administration > Workflow Mass Updates > Mass Processing Records in a Workflow"
parent: "section_N2796043"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2796312.html"
anchors: []
sha256: "865b17f80842cf7988df0d07b1d15d8a289d47cade8589177b49cb9795e6e2ef"
---

You can process multiple instances of a specific workflow simultaneously for the same record type in NetSuite. You can mass process instances of a workflow to transition them from the current state of the workflow instance to the next state. You can use this feature to reevaluate transitions or run a transition that executes on a button. This feature only applies to records that are already in a running workflow instance.

For example, you want to transition all employee records in a workflow named **New Employee Process** from **State 2 Approve Training** to **State 3 Training Approved**. The workflow contains an Approve Training button, added with the Add Button action, that approves the records and transitions them to State 3. Instead of opening each employee record and approving the training, you can mimic the click of the Approve Training button to approve all or a subset of the records and transition them to State 3.

#### To mass process a workflow for multiple records:

1.  Go to Lists > Mass Update > Mass Updates.
    
2.  On the Mass Updates page, expand **Workflow**.
    
    For each record type in NetSuite, the Mass Updates page lists the workflows that you can initiate, process, cancel, or transition for each record type.
    
3.  Click **Process <workflow name>** to process the appropriate workflow. The **Mass Update** page displays.
    
4.  On the **Mass Updates** page, enter a **Title**.
    
5.  If you want to mimic the click of a button to transition the record to the next state, select the button name in the **Button** dropdown list.
    
    Note:
    
    This must be a button added with the Add Button action to the current state of the workflow instance.
    
6.  Define the filters and other options on the following subtabs:
    
    | Subtab | Required / Optional | Description |
    | --- | --- | --- |
    | Criteria | Required | Select a field or formula in the dropdown list and enter values in the popup that appears. See [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html). |
    | Results | Optional | Set display options for mass update results. The results appear when you preview the records for the mass update. See [Search Results Display Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648053.html). |
    | Audience | Optional | Choose the users who can perform the mass update. |
    | Schedule | Optional | Define a schedule on which to perform the update. See [Scheduling a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668529.html). |
    
    The following screenshot shows the **Mass Updates** page for employee records created between two dates:
    
    ![A portion of the Mass Updates page for employee records created between two dates.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/MassProcessWorkflowFilters.png)
7.  Click **Preview** to view the records on which the mass update will run:
    
    ![A portion of the Mass Update Preview Results page showing an example of the records that the mass update will run on.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/MassProcessWorkflowPreviewResults.png)
8.  Do one of the following:
    
    -   To update immediately, in the **Apply** column, select the records you want to transition and click **Perform Update**. The status of the mass update is displayed on the **Mass Update Status** page.
        
    -   To save the update and update later, click **Save**. NetSuite saves the mass update and displays the **Saved Mass Updates** page. You can return to this page to transition the records by going to Lists > Mass Update > Saved Mass Updates. Click **Preview** next to the name of the update. On the **Mass Update Preview** page, click **Perform Update** to transition the records.
        

Note:

Optionally, from the **Mass Update** page, you can use the **Audit Trail** subtab to view the changes to the current mass update or use the **Action Title Translation** subtab to localize the title of the mass update.

### Related Topics

-   [Workflow Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2796043.html)
-   [Mass Initiating Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2796163.html)
-   [Mass Canceling Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103260636.html)
-   [Mass Transitioning Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1536603582.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
