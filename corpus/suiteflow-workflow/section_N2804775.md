---
id: "section_N2804775"
type: "section"
title: "State 4 Rejected"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Estimate Approval Routing Workflow > Building the Estimate Approval Routing Workflow > State 4 Rejected"
parent: "section_N2802225"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2804775.html"
anchors: []
sha256: "f0f01a27dccbf1991cf7f855bd9e6cdede378afa1ae121dbae70088155884e24"
---

After you set up **State 3 Approved** to approve estimates and send an email to the sales rep, set up **State 4 Rejected**. Create a Set Field Value action to set the **Approval Status** to **Rejected** and create a Send Email action to notify the sales rep that the estimate was rejected.

#### To set up State 4 Rejected:

1.  Make sure the Estimate Approval Routing workflow is open from the step [State 3 Approved](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2804462.html).
    
2.  To create the Set Field Value action, do the following:
    
    1.  In the Workflow Diagrammer, click **State 4 Rejected**.
        
    2.  In the context panel, on the **State** tab, click **New Action**.
        
    3.  In the **New Action** window, click **Set Field Value**.
        
    4.  Enter the following properties:
        
        | Section | Property | Value |
        | --- | --- | --- |
        | Basic Information | Trigger On | Entry |
        | Parameters | Field | Approval Status |
        | Value | Static Value | selected |
        | Selection | Rejected |
        
    5.  Click **Save**.
        
3.  To create the Send Email action, do the following:
    
    1.  In the Workflow Diagrammer, click **State 4 Rejected**.
        
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
        | Subject | Your Estimate Has Been Rejected |
        | Body | Estimate {number} has been rejected by your supervisor. |
        | Include View Record Link | checked |
        
    5.  Click **Save**.
        

**Next Step:** Now that the workflow setup is complete, test and then release the workflow. To continue with the estimate approval workflow example, go to [Testing the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2805158.html).

### Related Topics

-   [Building the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2802225.html)
-   [Creating States for the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2802386.html)
-   [Creating Transitions for the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4157713078.html)
-   [Preparing an Estimate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1069843.html)
-   [Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801522.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
