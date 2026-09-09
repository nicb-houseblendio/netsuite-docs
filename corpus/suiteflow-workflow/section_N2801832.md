---
id: "section_N2801832"
type: "section"
title: "Designing the Estimate Approval Routing Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Estimate Approval Routing Workflow > Designing the Estimate Approval Routing Workflow"
parent: "section_N2801522"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801832.html"
anchors: ["bridgehead_N2801844"]
sha256: "7fca004f8ebdee2b5a246ef1a661f9e491c9f95be80d0bb56879e0f8fb6effbf"
---

Before building the workflow, determine the workflow states required by estimate approvals. The Wolfe Electronics estimate approval workflow requires one state for each approval status.

## Estimate Approval Routing Summary {#bridgehead_N2801844}

The lead nurturing workflow uses the following workflow definition properties:

| Property | Value |
| --- | --- |
| **Record Type** | Transaction |
| **Sub Types** | Estimate |
| **Release Status** | Testing\* |
| **Initiation** | Event Based |
| **Trigger Type** | Before Record Submit |
| \* Use **Testing** until the workflow is ready for production, then set it to **Released**. |

The following table describes the states and the required actions and transitions:

| State | Actions | Transitions |
| --- | --- | --- |
| [State 1 Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164260556832.html) | 
-   Set Field Value: Set the **Approval Status** field to **Pending Approval**

 | Transitions to the following states:

-   **State 2 Pending Approval** if the estimate shows a default sales rep and that sales rep has a supervisor on their employee record.
-   **State 3 Approved** if the estimate shows a default sales rep and that sales rep has no supervisor on their employee record..

 |
| [State 2 Pending Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2804001.html) | 

-   Add Button: Add an **Approve** button
-   Add Button: Add a **reject** button

 | Transitions to the following states:

-   **State 3 Approved** if the supervisor clicks the **Approved** button.
-   **State 4 Rejected** if the supervisor clicks the **Reject** button.

 |
| [State 3 Approved](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2804462.html) | 

-   Set Field Value: Set the **Approval Status** field to **Approved**
-   Send Email: Send email to the sales rep

 | \- |
| [State 4 Rejected](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2804775.html) | 

-   Set Field Value: Set the **Approval Status** field to **Reject**
-   Send Email: Send email to the sales rep

 | \- |

**Next Step:** To begin with the estimate approval workflow example, go to [Before You Build the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801644.html).

### Related Topics

-   [Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801522.html)
-   [Before You Build the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801644.html)
-   [Building the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2802225.html)
-   [Testing the Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2805158.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
