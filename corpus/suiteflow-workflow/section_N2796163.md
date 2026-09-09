---
id: "section_N2796163"
type: "section"
title: "Mass Initiating Workflow Instances"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Administration > Workflow Mass Updates > Mass Initiating Workflow Instances"
parent: "section_N2796043"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2796163.html"
anchors: []
sha256: "8d45389dd9895c976d8e34585703dfd44876da8c1467143a464c55be091cf33e"
---

You can initiate multiple instances of a specific workflow simultaneously on multiple records in NetSuite. You can mass-initiate workflow instances for standard NetSuite record types or custom record types. Use this feature to avoid viewing each record individually to initiate a workflow instance on the record.

For example, use this feature if your company recently imported a large number of employee records for an acquisition. After they're imported, you decide that you want to initiate a workflow named **New Employee Process** on each employee record. NetSuite can initiate a separate workflow instance for each employee record, based on the filters you specify for the mass update.

Note:

You can also use a scheduled workflow to initiate multiple instances of a specific workflow simultaneously on multiple records. See [Scheduling a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4108268619.html).

#### To mass initiate a workflow on multiple records:

1.  Go to Lists > Mass Update > Mass Updates.
    
2.  On the Mass Updates page, expand **Workflow**.
    
    For each record type in NetSuite, the Mass Updates page lists the workflows that are available to initiate, process, cancel, or transition.
    
3.  Click **Initiate <workflow name>** to initiate the appropriate workflow. The **Mass Update** page displays.
    
4.  On the **Mass Updates** page, enter a **Title** and define the filters and other options on the following subtabs:
    
    | Subtab | Required / Optional | Description |
    | --- | --- | --- |
    | Criteria | Required | Select a field or formula in the dropdown list and enter values in the popup that appears. See [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html). |
    | Results | Optional | Set display options for mass update results. The results appear when you preview the records for the mass update. See [Search Results Display Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648053.html). |
    | Audience | Optional | Choose the users who can run the mass update. |
    | Schedule | Optional | Define a schedule on which to perform the mass update. See [Scheduling a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668529.html). |
    
    The following screenshot shows the **Mass Updates** page for employee records created between two dates:
    
    ![A portion of the Mass Updates page for employee records with the title of the action highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/MassInitiateWorkflowFilters.png)
5.  Click **Preview** to view the records on which the mass update will run:
    
    ![A portion of the Mass Update Preview Results page showing an example of the records that the mass update will run on.A portion of the Mass Update Preview Results page showing an example of the records that the mass update will run on.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/MassInitiateWorkflowPreviewResults.png)
6.  Do one of the following:
    
    -   To update immediately, in the **Apply** column, select the records you want to initiate the workflow on and click **Perform Update**. The status of the mass update is on the **Mass Update Status** page.
        
    -   To save the update and run it later, click **Save**. NetSuite saves the mass update and displays the **Saved Mass Updates** page. You can return to this page to initiate the workflow instances by going to Lists > Mass Update > Saved Mass Updates. Click **Preview** next to the name of the update. On the **Mass Update Preview** page, click **Perform Update** to initiate the workflow instances.
        

Note:

Optionally, from the **Mass Update** page, you can use the **Audit Trail** subtab to view the changes to the current mass update or use the **Action Title Translation** subtab to localize the title of the mass update.

### Related Topics

-   [Workflow Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2796043.html)
-   [Mass Processing Records in a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2796312.html)
-   [Mass Canceling Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103260636.html)
-   [Mass Transitioning Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1536603582.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
