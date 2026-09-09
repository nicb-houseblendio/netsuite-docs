---
id: "section_N2799369"
type: "section"
title: "Creating States for the Lead Nurturing Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Lead Nurturing Workflow > Building the Lead Nurturing Workflow > Creating States for the Lead Nurturing Workflow"
parent: "section_N2799033"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799369.html"
anchors: ["procedure_N2799393"]
sha256: "a3ceda21e7fb4f2353ae951a7a42fa113eec3f0d39ebab341e4f90c1c39802e4"
---

After you create the workflow definition, next create a workflow state for each of the five events in the lead nurturing campaign and an exit state for leads whose records are closed at any point in the workflow. After you create the states, create transitions and then set up each state by creating the actions and setting up the transitions.

#### To create states for each campaign event: {#procedure_N2799393}

1.  Make sure the Lead Nurturing workflow is open from the step [Building the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799033.html).
    
2.  In the workflow diagrammer, click **New State**.
    
    A new state appears in the diagrammer.
    
3.  Select the state in the diagrammer and click the **Edit** icon on the **State** tab in the context panel.
    
4.  In the **Name** field, enter **State 1: Webinar Invitation**.
    
5.  Repeat the above steps to create states for the campaign events in the workflow and the exit state:
    
    -   [State 1a Wait for 1 day](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4303454508.html)
        
    -   [State 2 Email Case Study](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800127.html)
        
    -   [State 2a Wait for 3 days](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4303985000.html)
        
    -   [State 3 Customer Testimonial](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800762.html)
        
    -   [State 4 Industry Comparison](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800846.html)
        
    -   [State 5 Free Trial Offer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800930.html)
        
    -   State 6 Exit
        
    
    Note:
    
    State 6 Exit does not have a section in this sample. It has no actions or transitions because it is the end of the workflow. For more information, see [Exit States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2734255.html)
    

**Next Step:** To continue with the lead nurturing workflow example, go to [Creating Transitions for the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4157473879.html).

### Related Topics

-   [Building the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799033.html)
-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)
-   [Designing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2798638.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
