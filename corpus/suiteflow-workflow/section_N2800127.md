---
id: "section_N2800127"
type: "section"
title: "State 2 Email Case Study"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Lead Nurturing Workflow > Building the Lead Nurturing Workflow > State 2 Email Case Study"
parent: "section_N2799033"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800127.html"
anchors: ["procedure_N2800143"]
sha256: "b066a84d6958ef6cc36bc640806196b6581ab52ff87d60700cb50fa400174575"
---

After you set up **State 1a Wait 1 day**, set up **State 2 Email Case Study**. If a lead clicked through the webinar invitation, this state sends an email with a case study to the lead. To set up State 2, create a Send Campaign Email action and a Subscribe To Record action and set up the transitions.

#### To set up State 2 Email Case Study: {#procedure_N2800143}

1.  Make sure the Lead Nurturing workflow is open from the step [State 1a Wait for 1 day](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4303454508.html).
    
2.  Select **State 2 Email Case Study** in the diagrammer.
    
3.  To create the Send Campaign Email action:
    
    1.  Click **New Action** on the **State** tab in the context panel.
        
    2.  Click **Send Campaign Email** in the **New Action** window.
        
    3.  Enter the following properties:
        
        | Property | Value |
        | --- | --- |
        | Trigger On | Entry |
        | Recipient | Send To Current Record |
        | Campaign Event | New Lead Nurturing : Secure your network with Wolfe Electronics |
        | Store Result In | CaseStudy.Response (Workflow) |
        
    4.  Click **Save**.
        
    
    Since the lead nurturing workflow determines which template to send based on campaign response, subscribe to the campaign response field for the case study.
    
4.  To create the Subscribe To Record action for the campaign response:
    
    1.  Click **New Action** on the **State** tab in the context panel.
        
    2.  Click **Subscribe To Record** in the **New Action** window.
        
    3.  In the **Field** dropdown list, select **CaseStudy.Response (Workflow)**.
        
    4.  Click **Save**.
        
5.  To set up the transition to **State 6 Exit**:
    
    1.  In the diagrammer, double-click the transition from **State 2 Email Case Study** to **State 6 Exit**.
        
    2.  In the **Workflow Transition** window, select **Visual Builder** and click the **Open** icon to open the Condition Builder.
        
    3.  In the **Workflow Condition** window, enter the following condition properties:
        
        | Column Name | Value |
        | --- | --- |
        | Field | Status |
        | Compare Type | any of |
        | Selection | Closed Won |
        
    4.  Click **Add**.
        
    5.  Click **Save** to save the condition.
        
6.  Click **Save** to save the transition.
    
    If the lead clicks on a link in the Case Study, they move to **State 2a Wait 3 days** where they will wait 3 days before moving to **Step 3 Customer Testimonial**.
    
7.  To set up the transition to **State 2a Wait 3 days**:
    
    1.  In the diagrammer, double-click the transition from **State 2 Webinar Invitation** to **State 2a Wait for 3 days**.
        
    2.  Select **Visual Builder**, click the **Open** icon to open the Condition Builder, and create a condition with the following properties:
        
        | Column Name | Value |
        | --- | --- |
        | Record | CaseStudy.Response (Workflow) |
        | Field | Response Type |
        | Compare Type | any of |
        | Selection | Clicked Through |
        
    3.  Click **Add**.
        
    4.  Click **Save** to save the condition.
        
8.  Click **Save** to save the transition.
    
    If the lead does not click on the link in the case study, the record moves to **State 5 Free Trial Offer** seven days later.
    
9.  To set up the transition to **State 5 Free Trial Offer**:
    
    1.  In the diagrammer, double-click the transition from **State 2 Email Case Study** to **State 5 Free Trial Offer**.
        
    2.  In the **Workflow Transition** window, set the following properties:
        
        | Property | Value |
        | --- | --- |
        | Transition On | Scheduled |
        | Delay | 7 |
        | Unit | Day |
        
    3.  Select **Visual Builder** , click the **Open** icon to open the Condition Builder, and create a condition with the following properties:
        
        | Column Name | Value |
        | --- | --- |
        | Record | CaseStudy.Response (Workflow) |
        | Field | Response Type |
        | Compare Type | any of |
        | Selection | Received, Sent |
        
    4.  Click **Add**.
        
    5.  Click **Save** to save the condition.
        
10.  Click **Save** to save the changes to the transition.
     

**Next Step:** To continue with the lead nurturing workflow example, go to [State 2a Wait for 3 days](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4303985000.html).

### Related Topics

-   [Building the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799033.html)
-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)
-   [Designing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2798638.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
