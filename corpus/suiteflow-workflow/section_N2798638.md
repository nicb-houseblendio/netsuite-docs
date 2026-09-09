---
id: "section_N2798638"
type: "section"
title: "Designing the Lead Nurturing Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Lead Nurturing Workflow > Designing the Lead Nurturing Workflow"
parent: "section_N2797000"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2798638.html"
anchors: ["bridgehead_N2798674"]
sha256: "3f5ade6c8b92d3515dd84261ce5ff608c2ae7a384556b972554b7d8117205bca"
---

Before building a workflow, determine the required workflow states for the campaign. The lead nurturing campaign for Wolfe Electronics requires one state for each lead nurturing campaign event.

## Lead Nurturing Campaign Summary {#bridgehead_N2798674}

The lead nurturing workflow uses the following workflow definition properties:

| Property | Value |
| --- | --- |
| **Record Type** | Customer |
| **Sub Types** | Lead |
| **Release Status** | Testing\* |
| **Initiation** | Event Based |
| **Trigger Type** | After Record Submit |
| \* Use **Testing** until the workflow is ready for production, then set it to **Released**. |

The following table describes the states and the required actions and transitions:

| State | Actions | Transitions |
| --- | --- | --- |
| [State 1 Webinar Invitation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799553.html) | 
-   Send Campaign Email: Email a webinar invitation
-   Subscribe To Record: Track response to the email

 | Transitions to the following states:

-   **State 1a Wait 1 day** if the campaign response is **Clicked Through**.
-   **State 4 Industry Comparison** if the campaign is not responded to after 14 days.
-   **State 6 Exit** if the lead status is **Closed Won**.

 |
| State 1a Wait 1 day | There are no actions for this state. | Transitions to the following state:

-   **State 2 Email Case Study**

 |
| [State 2 Email Case Study](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800127.html) | 

-   Send Campaign Email: Email a case study

 | Transitions to the following states:

-   **State 2a Wait 3 days** if the campaign response is **Clicked Through**.
-   **State 5 Free Trial Offer** if the campaign is not responded to after 14 days
-   **State 6 Exit** if the lead status is **Closed Won**.

 |
| State 2a Wait 3 days | There are no actions for this state. | Transitions to the following state:

-   **State 3 Customer Testimonia** l

 |
| [State 3 Customer Testimonial](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800762.html) | 

-   Send Campaign Email: Email a customer testimonial

 | Transitions to the following states:

-   **State 6 Exit** if the lead status is **Closed Won**.

 |
| [State 4 Industry Comparison](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800846.html) | 

-   Send Campaign Email: Email an industry comparison

 | \- |
| [State 5 Free Trial Offer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2800930.html) | 

-   Send Campaign Email: Email a free 30 day trial

 | \- |
| State 6 Exit | \- | \- |

**Next Step:** To begin with the lead nurturing workflow example, go to [Before You Build the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797138.html).

### Related Topics

-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)
-   [Configuring Your Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1003300.html)
-   [Before You Build the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797138.html)
-   [Building the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2799033.html)
-   [Testing the Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801095.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
