---
id: "section_N2804462"
type: "section"
title: "State 3 Approved"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Estimate Approval Routing Workflow > Building the Estimate Approval Routing Workflow > State 3 Approved"
parent: "section_N2802225"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2804462.html"
anchors: []
sha256: "60d46f6180ecef6f151bc504309cc49706f2ffd14551616a81e8a73895e28ba5"
---

After you set up **State 2 Pending Approval** to enable supervisors to approve or reject estimates, set up **State 3 Approved**. Create a Set Field Value action to set the **Approval Status** to **Approved** and create a Send Email action to notify the sales rep that the estimate was approved.

#### To set up State 3 Approved:

1.  Make sure the Estimate Approval Routing workflow is open from the step [State 2 Pending Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2804001.html).
    
2.  To create the Set Field Value action, do the following:
    
    1.  In the Workflow Diagrammer, click **State 3 Approved**.
        
    2.  In the context panel, on the **State** tab, click **New Action**.
        
    3.  In the **New Action** window, click **Set Field Value**.
        
    4.  Enter the following properties:
        
        | Section | Property | Value |
        | --- | --- | --- |
        | Basic Information | Trigger On | Entry |
        | Parameters | Field | Approval Status |
        | Value | Static Value | selected |
        | \- | Selection | Approved |
        
    5.  Click **Save**.
        
3.  To create the Send Email action, do the following:
    
    1.  In the Workflow Diagrammer, click **State 3 Approved**.
        
    2.  In the context panel, on the **State** tab, click **New Action**.
        
    3.  In the **New Action** window, click **Send Email**.
        
    4.  Enter the following properties:
        
        | Section | Property | Value |
        | --- | --- | --- |
        | Sender | From Field | selected |
        | Record | Sales Rep |
        | Field | Supervisor |
        | Recipient | From Field | selected |
        | Record | Current Record |
        | Field | Sales Rep |
        | Content | Custom | selected |
        | Subject | Your Estimate Has Been Approved |
        | Body | Estimate {number} has been approved by your supervisor. |
        | Include View Record Link | checked |
        
    5.  Click **Save**.
        

**Next Step:** To continue with the estimate approval workflow example, go to [State 4 Rejected](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2804775.html).

### Related Topics

-   [Building the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2802225.html)
-   [Creating States for the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2802386.html)
-   [Creating Transitions for the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4157713078.html)
-   [Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801522.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
