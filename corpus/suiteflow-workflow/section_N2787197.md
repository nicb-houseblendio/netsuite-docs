---
id: "section_N2787197"
type: "section"
title: "Testing for User Accessibility"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Testing and Troubleshooting Workflows > Testing a Workflow > Testing for User Accessibility"
parent: "section_N2786153"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2787197.html"
anchors: []
sha256: "3bab6a99d3640a843e764ced2979679f0d118f8498b943a647f8a18a9af347f2"
---

You must test a workflow for every user role you want it to run for. When you develop a workflow as an administrator, each workflow runs properly if it's designed correctly. However, you must test the workflow by logging in as the separate user roles for which the workflow will run.

You must test the following accessibility scenarios:

-   Access for a specific role. You must test that there are no permission or other restrictions on the record type that would prevent a workflow from running correctly for a specific role. For example, for a lead record that is updated by sales reps, log in with a sales rep role to test the workflow.
    
-   Access from within the Employee Center. If users create or update the record from within the Employee Center, access the record from within the Employee Center with the proper role to test the workflow.
    
-   Access to related records. If a workflow sets a value on a record using the Set Field Value action, and the Set Field Value action gets the value from a related record, you must test that the user role has access to the related record. For example, the record for the workflow is Purchase Order and the workflow runs a Set Field Value action. The Set Field Value action gets the value from a Vendor or Employee record. Verify that any role that works with the Purchase Order has at least View access to the Vendor and Employee records also.
    

For more information about accessing data in related records, see [Defining the Workflow Audience](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4082045210.html) and [Execute as Admin for Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2780140.html).

### Related Topics

-   [Testing a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2786153.html)
-   [Setting Up a Workflow for Testing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471802671.html)
-   [Testing Workflow Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2786511.html)
-   [Testing Actions and Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2786649.html)
-   [Testing Buttons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4471796885.html)
-   [Testing a Send Email Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4472473260.html)
-   [Testing Scheduled Workflows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3873172773.html)
-   [Testing Scheduled Actions and Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4472474105.html)
-   [Testing and Troubleshooting Workflows](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2786070.html)
-   [Defining the Workflow Audience](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4082045210.html)
-   [Execute as Admin for Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2780140.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
