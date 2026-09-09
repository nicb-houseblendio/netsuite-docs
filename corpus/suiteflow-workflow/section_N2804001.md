---
id: "section_N2804001"
type: "section"
title: "State 2 Pending Approval"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Estimate Approval Routing Workflow > Building the Estimate Approval Routing Workflow > State 2 Pending Approval"
parent: "section_N2802225"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2804001.html"
anchors: []
sha256: "0291d364068cc18d621a4b1533065501e58cfb885c0199c21bf362f78af31d85"
---

After you set up **State 1 Entry** to determine which estimates require approval routing, set up **State 2 Pending Approval** to enable supervisors to approve or reject estimates. Create the two Add Button actions to add the **Approve** and **Reject** buttons. Then set up the transitions, which depend on which button is clicked when the supervisor views the record.

Note:

The **Approve** and **Reject** buttons only appear if the user viewing the record is the supervisor for the sales rep.

#### To set up State 2 Pending Approval:

1.  Make sure the Estimate Approval Routing workflow is open from the step [State 1 Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164260556832.html).
    
2.  To create the Add Button action for the **Approve** button, do the following:
    
    1.  In the Workflow Diagrammer, click **State 2 Pending Approval**.
        
    2.  In the context panel, on the **State** tab, click **New Action**.
        
    3.  In the **New Action** window, click **Add Button**.
        
    4.  In the **Basic Information** section, in the **Trigger On** field, select **Before Record Load**.
        
    5.  In the **Condition** section, select **Visual Builder**.
        
    6.  Click the **Open** icon to open the Condition Builder, and create a condition with the following properties:
        
        | Column Name | Value |
        | --- | --- |
        | Record | Sales Rep |
        | Field | Supervisor |
        | Compare Type | any of |
        | Selection | Current User |
        
    7.  Click **Add**, and then click **Save** to save the condition.
        
    8.  In the **Parameters** section, in the **Label** field, enter **Approve**.
        
    9.  Click **Save** to save the action.
        
3.  To create the Add Button action for the **Reject** button, do the following:
    
    1.  In the Workflow Diagrammer, click **State 2 Pending Approval**.
        
    2.  In the context panel, on the **State** tab, click **New Action**.
        
    3.  In the **New Action** window, click **Add Button**.
        
    4.  In the **Basic Information** section, in the **Trigger On** field, select **Before Record Load**.
        
    5.  In the **Condition** section, select **Visual Builder**.
        
    6.  Click the **Open** icon to open the Condition Builder, and create a condition with the following properties:
        
        | Column Name | Value |
        | --- | --- |
        | Record | Sales Rep |
        | Field | Supervisor |
        | Compare Type | any of |
        | Selection | Current User |
        
    7.  Click **Add**, and then click **Save** to save the condition.
        
    8.  In the **Parameters** section, in the **Label** field, enter **Reject**.
        
    9.  Click **Save** to save the action.
        
4.  To set up the transition to **Step 3 Approve** if the supervisor clicks the **Approve** button, do the following:
    
    1.  In the Workflow Diagrammer, double-click the transition arrow from **State 2 Pending Approval** to **State 3 Approve**.
        
    2.  In the **Workflow Transition** window, in the **Execute on Button** field, select **Approve**.
        
    3.  Click **Save** to save the transition.
        
5.  To set up the transition to **Step 4 Reject** if the supervisor clicks the **Reject** button, do the following:
    
    1.  In the Workflow Diagrammer, double-click the transition arrow from **State 2 Pending Approval** to **State 4 Reject**.
        
    2.  In the **Workflow Transition** window, in the **Execute on Button** field, select **Reject**.
        
    3.  Click **Save** to save the transition.
        

**Next Step:** To continue with the estimate approval workflow example, go to [State 3 Approved](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2804462.html).

### Related Topics

-   [Building the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2802225.html)
-   [Creating States for the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2802386.html)
-   [Creating Transitions for the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4157713078.html)
-   [Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801522.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
