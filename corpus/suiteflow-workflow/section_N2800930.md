---
id: "section_N2800930"
type: "section"
title: "State 5 Free Trial Offer"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Lead Nurturing Workflow > Building the Lead Nurturing Workflow > State 5 Free Trial Offer"
parent: "section_N2799033"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800930.html"
anchors: ["procedure_4157581984"]
sha256: "91ebe1414dd01fb7e5fa53383f9af046bbbda6735dc69d1eb7a02cccf2b8e843"
---

After you set up **State 4 Industry Comparison**, set up **State 5 Free Trial Offer**. If a lead did not click through the case study, this state sends a free trial offer email. To set up State 5, create a Send Campaign Email action.

#### To set up State 5 Free Trial Offer: {#procedure_4157581984}

1.  Make sure the Lead Nurturing workflow is open from the step [State 4 Industry Comparison](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800846.html).
    
2.  Select **State 5 Free Trial Offer** in the diagrammer.
    
3.  To create the Send Campaign Email action:
    
    1.  Click **New Action** on the **State** tab in the context panel.
        
    2.  Click **Send Campaign Email** in the **New Action** window.
        
    3.  Enter the following properties:
        
        | Property | Value |
        | --- | --- |
        | Trigger On | Entry |
        | Recipient | Send To Current Record |
        | Campaign Event | New Lead Nurturing : Try us free for 30 days |
        
    4.  Click **Save**.
        

**Next Step:** Now that the workflow setup is complete, test and then release the workflow. To continue with the lead nurturing workflow example, go to [Testing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801095.html).

### Related Topics

-   [Building the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799033.html)
-   [Lead Nurturing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1003092.html)
-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)
-   [Testing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801095.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
