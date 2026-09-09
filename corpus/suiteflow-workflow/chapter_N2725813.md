---
id: "chapter_N2725813"
type: "chapter"
title: "Creating Your First Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Creating Your First Workflow"
parent: "book_N2723865"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2725813.html"
anchors: []
sha256: "ab66f8f3c3a84b9728266cc6a416ca1379b406e21d903677f849d9df95564751"
---

This tutorial describes the necessary steps to create and run a workflow in NetSuite. Use these steps to get familiar with the Workflow Manager user interface and the parts of a workflow.

In this tutorial, you will create a workflow that runs when a user creates a new Opportunity record. The workflow makes the **Title** field on the opportunity record required and sends the user to the Opportunities list page after they save the opportunity.

To view, create, or edit workflows, you need the right permissions for the base record types in the workflow. To access all of SuiteFlow functionality, use the Administrator role. For more information, see [Required Permissions for SuiteFlow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1489429737.html).

The following table describes the tutorial steps. Each step builds on the previous step, so you must complete them in order.

| Step | Description |
| --- | --- |
| Define basic workflow properties | Create the workflow and define the basic properties on the workflow definition page, including the workflow name, workflow base record, owner, and release status. See [Step 1 Define Workflow Basic Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726220.html). |
| Define workflow initiation | Define the workflow initiation on the workflow definition page. The workflow initiates on creation of an Opportunity record. See [Step 2 Define Workflow Initiation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726358.html). |
| Define the workflow condition | Define a condition that must be met for the workflow to initiate. See [Step 3 Define the Workflow Condition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726518.html). |
| Create workflow states | Create the two states required by the workflow: the entry state and the exit state. See [Step 4 Create Workflow States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726745.html). |
| Create actions | Create the actions to make a field required and to go to the Opportunities list page. See [Step 5 Create Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2726890.html). |
| Create a transition | Create a transition between the entry and exit states. See [Step 6 Create a Transition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2727164.html) |
| Initiate and validate the workflow | Create an opportunity and verify that the workflow executes as expected. See [Step 7 Initiate and Validate the Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2727383.html). |

Tip:

See the **Related Topics** sections in each step to get more information about the concepts or properties.

### Related Topics

-   [SuiteFlow (Workflow)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N2723865.html)
-   [SuiteFlow Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4068260113.html)
-   [Working with Workflows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4101515562.html)
-   [Workflow Administration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4103088279.html)
-   [SuiteFlow Reference and Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4103690129.html)
-   [Testing and Troubleshooting Workflows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2786070.html)
-   [Workflow Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2796642.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
