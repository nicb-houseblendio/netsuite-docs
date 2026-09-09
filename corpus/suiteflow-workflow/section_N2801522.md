---
id: "section_N2801522"
type: "section"
title: "Estimate Approval Routing Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Estimate Approval Routing Workflow"
parent: "chapter_N2796642"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801522.html"
anchors: ["bridgehead_4157681492"]
sha256: "b20d7a86231a08e31d3e0ab2aefba43b29c28a1bdea540cfe618c3cb58e5940f"
---

The following sample workflow details approval routing used by the fictional company Wolfe Electronics. This workflow allows supervisors to approve or reject estimates entered by their sales reps.

This workflow initiates when a sales rep creates a new estimate record and clicks **Save**. At this point, the estimate is checked to see if the sales rep identified on the estimate has a supervisor on his or her employee record.

The behavior of the workflow depends on the sales rep supervisor:

-   Sales rep has a supervisor. The status of the estimate becomes Pending Approval. Buttons to approve or reject the estimate show when the sales rep supervisor views the estimate.
    
    If the supervisor clicks **Approve**, the status of the estimate becomes Approved and an email is sent to the sales rep. If the supervisor clicks **Reject**, the status of the estimate becomes Rejected and an email is sent to the sales rep.
    
-   Sales rep does not have a supervisor. The status of the estimate becomes Approved and an email is sent to the sales rep.
    

The following diagram shows the Wolfe Electronics estimate approval workflow:

![A diagram of an example of an estimate approval workflow.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/ARApprovalRouting_Sample1.png)

## Steps to Complete the Estimate Approval Workflow {#bridgehead_4157681492}

The following table lists the steps required to complete the estimate approval workflow:

| Step | Description |
| --- | --- |
| [Designing the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801832.html) | Review the workflow requirements, including the summary of the workflow definition properties, states, actions, and transitions. |
| [Before You Build the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801644.html) | Create a custom field to store the approval status for the estimate. |
| [Building the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2802225.html) | Create the states and the actions and transitions for each state. |
| [Testing the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2805158.html) | Complete the steps necessary to test the workflow and then release the workflow. |

Note:

For more information about the elements of a workflow, see [Workflow Elements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071953058.html).

### Related Topics

-   [Workflow Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2796642.html)
-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)
-   [Lead that Did Not Convert to Customer Within Three Days](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801202.html)
-   [Welcome Email Sent to Customers Three Days After First Order Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2806856.html)
-   [Storing a Return Value from a Custom Action Script in a Workflow Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2807069.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
