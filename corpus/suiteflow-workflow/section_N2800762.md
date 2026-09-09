---
id: "section_N2800762"
type: "section"
title: "State 3 Customer Testimonial"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Lead Nurturing Workflow > Building the Lead Nurturing Workflow > State 3 Customer Testimonial"
parent: "section_N2799033"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800762.html"
anchors: ["procedure_N2800778"]
sha256: "028892610a9292b2b92f0d9863b1be575c2889d1fae176e3e003a0d102ca6ea3"
---

After you set up **State 2 Email Case Study**, set up **State 3 Customer Testimonial**. If a lead clicked through the case study sent in State 2, this state sends an email with a customer testimonial to the lead. To set up State 3, create a Send Campaign Email action.

#### To set up State 3 Customer Testimonial: {#procedure_N2800778}

1.  Make sure the Lead Nurturing workflow is open from the step [State 2 Email Case Study](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800127.html).
    
2.  Select **State 3 Customer Testimonial** in the diagrammer.
    
3.  To create the Send Campaign Email action:
    
    1.  Click **New Action** on the **State** tab in the context panel.
        
    2.  Click **Send Campaign Email** in the **New Action** window.
        
    3.  Enter the following properties:
        
        | Property | Value |
        | --- | --- |
        | Trigger On | Entry |
        | Recipient | Send To Current Record |
        | Campaign Event | New Lead Nurturing : What our customers are saying |
        
    4.  Click **Save**.
        

**Next Step:** To continue with the lead nurturing workflow example, go to [State 4 Industry Comparison](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800846.html).

### Related Topics

-   [Building the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799033.html)
-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)
-   [Designing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2798638.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
