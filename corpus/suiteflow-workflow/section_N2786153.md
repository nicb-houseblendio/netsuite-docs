---
id: "section_N2786153"
type: "section"
title: "Testing a Workflow"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Testing and Troubleshooting Workflows > Testing a Workflow"
parent: "chapter_N2786070"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2786153.html"
anchors: []
sha256: "05cced3d6994e336df917839557dbbc61e3733ff10e5354975a511b316e8c727"
---

Before making a workflow available to all users, test it to make sure that the workflow runs correctly. Complete the following steps to test a workflow:

-   Set up the workflow for testing. Enable logging and set the release status. For more information, see [Setting Up a Workflow for Testing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471802671.html).
    
-   Test conditions. Set up a testing scenario where you can verify that the conditions can evaluate to both true and false. For more information, see [Testing Workflow Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2786511.html).
    
-   Test actions and transitions. Make sure that actions and transitions appear in the workflow execution log and complete successfully. For more information, see [Testing Actions and Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2786649.html).
    
-   Test buttons. Make sure buttons appear in all states of the workflow where they're required. For more information, see [Testing Buttons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471796885.html).
    
-   Test Send Email actions. Use the workflow execution log to make sure that the Send Email actions send an email. For more information, see [Testing a Send Email Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4472473260.html).
    
-   Test scheduled workflows. Initiate a scheduled workflow to start immediately and quickly test the logic in the workflow. For more information, see [Testing Scheduled Workflows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3873172773.html).
    
-   Test scheduled actions and transitions. Set the smallest possible delay on a scheduled action or transition for testing. For more information, see [Testing Scheduled Actions and Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4472474105.html).
    
-   Test for user access. Test access for specific roles, test from within the Employee Center, and test access to related records. For more information, see [Testing for User Accessibility](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2787197.html).
    

Note:

Workflow errors can occur due to incorrect triggers on actions and transitions. Make sure you review triggers and the SuiteFlow trigger execution model. For information, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).

### Related Topics

-   [Testing and Troubleshooting Workflows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2786070.html)
-   [Viewing Workflow Activity](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2788150.html)
-   [Troubleshooting a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2787352.html)
-   [SuiteFlow Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540490044.html)
-   [FAQ: SuiteFlow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554318378.html)
-   [Workflow Execution Log](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4472471134.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
