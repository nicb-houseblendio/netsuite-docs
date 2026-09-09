---
id: "section_N2786511"
type: "section"
title: "Testing Workflow Conditions"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Testing and Troubleshooting Workflows > Testing a Workflow > Testing Workflow Conditions"
parent: "section_N2786153"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2786511.html"
anchors: ["bridgehead_N2786562"]
sha256: "1c1a3409842770c70156e873b608bdf13f369a4b9f2a1b36a00a2f9315a99831"
---

If you use conditions in your workflow, use the workflow execution log to make sure that the conditions work as designed. In general, make sure that you create conditions that can be met. Otherwise, the condition can never evaluate to true and the workflow doesn't run as expected.

Run the following condition tests on a workflow:

-   Test a scenario when the condition evaluates to true to make sure that the workflow executes the actions and transitions as expected.
    
-   Test a scenario when the condition evaluates to false to make sure that the workflow doesn't process the actions and transitions.
    
-   If you have a condition on the workflow initiation, verify that the workflow does or doesn't initiate based on the condition.
    

## Tip {#bridgehead_N2786562}

If actions or transitions with conditions don't process, temporarily remove the condition and then run the workflow again. If the workflow runs correctly, the condition has an error.

### Related Topics

-   [Testing a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2786153.html)
-   [Setting Up a Workflow for Testing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471802671.html)
-   [Testing Actions and Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2786649.html)
-   [Testing Buttons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471796885.html)
-   [Testing a Send Email Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4472473260.html)
-   [Testing Scheduled Workflows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3873172773.html)
-   [Testing Scheduled Actions and Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4472474105.html)
-   [Testing for User Accessibility](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2787197.html)
-   [Testing and Troubleshooting Workflows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2786070.html)
-   [Workflow Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954369.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
