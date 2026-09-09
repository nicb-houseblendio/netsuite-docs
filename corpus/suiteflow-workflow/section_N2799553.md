---
id: "section_N2799553"
type: "section"
title: "State 1 Webinar Invitation"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Lead Nurturing Workflow > Building the Lead Nurturing Workflow > State 1 Webinar Invitation"
parent: "section_N2799033"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799553.html"
anchors: ["procedure_N2799569"]
sha256: "faf6a941af4bd833cc5c71e2622f541c524d4608c136b6b6d5e3bd8a38d5066c"
---

After you're done creating the states and transitions, you're ready to set up **State 1 Webinar Invitation**. This state marks the start of the workflow, where the first email goes out to leads in the software industry. To set up State 1, you're creating a Send Campaign Email action and a Subscribe To Record action, and you're setting up the transitions. After you create the states and transitions, you can set up **State 1 Webinar Invitation**. This state is the point in the workflow where the workflow initiates and the initial email is sent to leads in the software industry. To set up State 1, create a Send Campaign Email action and a Subscribe To Record action and set up the transitions.

#### To set up State 1 Webinar Invitation: {#procedure_N2799569}

1.  Make sure the Lead Nurturing workflow is open from the step [Creating Transitions for the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4157473879.html).
    
2.  Select **State 1 Webinar Invitation** in the diagrammer.
    
3.  To create the Send Campaign Email action:
    
    1.  Click **New Action** on the **State** tab in the context panel.
        
    2.  Click **Send Campaign Email** in the **New Action** window.
        
    3.  Enter the following properties:
        
        | Property | Value |
        | --- | --- |
        | Transition On | Entry |
        | Recipient | Send To Current Record |
        | Campaign Event | New Lead Nurturing : Trends in Internet Security |
        | Store Result In | Webinar.Response (Workflow) |
        
    4.  Click **Save**.
        
    
    Since the lead nurturing workflow determines which template to send based on campaign response, subscribe to the campaign response field for the webinar. This way the workflow instance on the lead record triggers each time the campaign response changes.
    
4.  To create the Subscribe To Record action for the campaign response:
    
    1.  Click **New Action** on the **State** tab in the context panel.
        
    2.  Click **Subscribe To Record** in the **New Action** window.
        
    3.  In the **Field** dropdown list, select **Webinar.Response**.
        
    4.  Click **Save**.
        
    
    If the lead's record is closed during this workflow, it leaves the workflow and does not receive further email. Each non-exit state in the workflow has a transition to the exit state.
    
5.  To set up the transition to **State 6 Exit**:
    
    1.  In the diagrammer, double-click the transition from **State 1 Webinar Invitation** to **State 6 Exit**.
        
    2.  In the **Workflow Transition** window, select **Visual Builder** and click the **Open** icon to open the Condition Builder.
        
    3.  In the **Workflow Condition** window, enter the following condition properties:
        
        | Column Name | Value |
        | --- | --- |
        | Field | Status |
        | Compare Type | any of |
        | Selection | Closed Won |
        
    4.  Click **Add**.
        
    5.  Click **Save** to save the condition.
        
    
    If the lead clicks on a link in the Webinar Invitation, they move to **State 1a Wait for 1 day** where they will wait for 1 day before moving to **State 2 Email Case Study**.
    
6.  To set up the transition to **State 2 Email Case Study**:
    
    1.  In the diagrammer, double-click the transition from **State 1 Webinar Invitation** to **State 1a Wait 1 day**.
        
    2.  In the **Workflow Transition** window, select **Visual Builder**, click the **Open** icon to open the Condition Builder, and create a condition with the following properties:
        
        | Column Name | Value |
        | --- | --- |
        | Record | Webinar.Response |
        | Field | Response |
        | Compare Type | any of |
        | Selection | Clicked Through |
        
    3.  Click **Add**.
        
    4.  Click **Save** to save the condition.
        
7.  Click **Save** to save the transition.
    
    If the lead does not click on a link in the Webinar Invitation, the record moves to State 4 two weeks later.
    
8.  To set up the transition to **State 4 Industry Comparison**:
    
    1.  In the diagrammer, double-click the transition from **State 1 Webinar Invitation** to **State 4 Industry Comparison**.
        
    2.  In the **Workflow Transition** window, set the following properties:
        
        | Property | Value |
        | --- | --- |
        | Transition On | Scheduled |
        | Delay | 14 |
        | Unit | Day |
        
9.  Click **Save** to save the changes to the transition.
    

**Next Step:** To continue with the lead nurturing workflow example, go to [State 1a Wait for 1 day](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4303454508.html).

### Related Topics

-   [Building the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799033.html)
-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)
-   [Designing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2798638.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
