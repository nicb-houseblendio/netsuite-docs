---
id: "section_N2800846"
type: "section"
title: "State 4 Industry Comparison"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Lead Nurturing Workflow > Building the Lead Nurturing Workflow > State 4 Industry Comparison"
parent: "section_N2799033"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800846.html"
anchors: ["procedure_4157580598"]
sha256: "82dff54d0186ba7ea3aa42871359ca102a520db933a9548c00c14be8ea5617b6"
---

After you set up **State 3 Customer Testimonial**, set up **State 4 Industry Comparison**. If a lead did not click through the webinar invitation, this state sends an industry comparison email. To set up State 4, create a Send Campaign Email action.

#### To set up State 4 Industry Comparison: {#procedure_4157580598}

1.  Make sure the Lead Nurturing workflow is open from the step [State 3 Customer Testimonial](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800762.html).
    
2.  Select **State 4 Industry Comparison** in the diagrammer.
    
3.  To create the Send Campaign Email action:
    
    1.  Click **New Action** on the **State** tab in the context panel.
        
    2.  Click **Send Campaign Email** in the **New Action** window.
        
    3.  Enter the following properties:
        
        | Property | Value |
        | --- | --- |
        | Trigger On | Entry |
        | Recipient | Send To Current Record |
        | Campaign Event | New Lead Nurturing : Best Internet Security Services 2014 |
        
    4.  Click **Save**.
        

**Next Step:** To continue with the lead nurturing workflow example, go to [State 5 Free Trial Offer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800930.html).

### Related Topics

-   [Building the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799033.html)
-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)
-   [Designing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2798638.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
