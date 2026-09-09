---
id: "section_N2797000"
type: "section"
title: "Lead Nurturing Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Lead Nurturing Workflow"
parent: "chapter_N2796642"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html"
anchors: ["bridgehead_4156915682"]
sha256: "52886c86b1c3b8a45f3d9093923c306a98f646a486e4fadb1fa95471c666d9b2"
---

The following sample workflow details a lead nurturing campaign created by the fictional company Wolfe Electronics. The Wolfe Electronics marketing department designed this campaign and workflow to market their security software.

The workflow executes the following basic steps after a lead is created in NetSuite, if the lead is part of the software industry:

1.  Send an invitation to a webinar. The workflow sends the lead an invitation to a webinar titled 'Trends in Internet Security', with a link to an online registration form.
    
    If the lead does not respond to the webinar invitation in 14 days, the workflow sends an email message titled 'Best Internet Security Services of 2014' and the workflow completes.
    
    If the lead responds to the webinar invitation, the workflow waits one day and proceeds to the next step.
    
2.  Email a case study. The workflow sends an email with link to a case study that describes Wolfe Electronics security offerings.
    
    If the lead does not click through to the case study, the workflow sends an email 7 days later with a free trial offer and the workflow completes.
    
    If the lead clicks through to the case study, the workflow waits 3 days and proceeds to the next step.
    
3.  Email a customer testimonial. The workflow sends an email with a customer testimonial and the workflow completes.
    

The following diagram shows the lead nurturing workflow for Wolfe Electronics:

![A diagram depicting an example of a lead nurturing workflow.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/leadnurturingsample_diagram.png)

## Steps to Complete the Lead Nurturing Workflow {#bridgehead_4156915682}

The following table lists the steps required to complete the lead nurturing workflow:

| Step | Description |
| --- | --- |
| [Designing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2798638.html) | Review the workflow requirements, including the summary of the lead nurturing campaign, workflow definition properties, states, actions, and transitions. |
| [Before You Build the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797138.html) | Create the required marketing templates, lead nurturing campaign record, and Industry custom field to store the recipient of the lead nurturing campaign. |
| [Building the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799033.html) | Create the states and the actions and transitions for each state. |
| [Testing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801095.html) | Review the steps necessary to test the workflow and then release the workflow. |

Note:

For more information about the elements of a workflow, see [Workflow Elements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071953058.html).

### Related Topics

-   [Workflow Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2796642.html)
-   [Lead that Did Not Convert to Customer Within Three Days](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801202.html)
-   [Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801522.html)
-   [Welcome Email Sent to Customers Three Days After First Order Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2806856.html)
-   [Storing a Return Value from a Custom Action Script in a Workflow Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2807069.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
