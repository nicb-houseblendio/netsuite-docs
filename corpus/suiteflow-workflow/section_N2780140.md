---
id: "section_N2780140"
type: "section"
title: "Execute as Admin for Workflow Instances"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Working with Workflows > Creating a Workflow > Execute as Admin for Workflow Instances"
parent: "section_4101527388"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2780140.html"
anchors: ["bridgehead_4122050844"]
sha256: "70bd07bc9bb7a07080b621bc5a8b5e22d8a80e01af8bd7a8eb3020b66f9825ec"
---

On the workflow definition page, you can check the **Execute As Admin** box to have NetSuite to execute workflow instances as a user with the Administrator role. These privileges override the role of the user who initiated the workflow instance.

![A portion of the workflow definition page with the Execute As Admin checkbox highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/ExecuteAsAdmin_2.png)

Some workflows may require administrator privileges. For example, you create a workflow that adds follow-up tasks after a sales order is saved and it needs to read data from employee records. The workflow instance won't work if the user doesn't have access to those records.

## Rules and Guidelines for Using Execute As Admin {#bridgehead_4122050844}

Important:

Use **Execute As Admin** only when required. Otherwise, you may give users more data access than intended.

Use the following rules and guidelines with this property:

-   If you check **Execute As Admin**, any action with a record join must execute on a server trigger, not a client trigger. Actions on a client trigger won't run as expected. For more information about the difference between server and client triggers, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html).
    
-   Only users with the Administrator role can check **Execute As Admin**. This box is disabled for all other roles, even those with the full Workflow permission. The same applies for the **Execute As Admin** box on the SuiteScript Deployment page.
    
-   If you check **Execute As Admin**, the Override Period Restrictions permission isn't enabled for the workflow. Instead, the logged in user's permission is used to determine if the workflow can update Posting Period fields. This prevents users without the Override Period Restrictions permission from posting transactions in locked periods. However, other updates such as changes to **Approval Status** may still change Posting Period values, even if the user doesn't have the Override Period Restrictions permission.
    
-   The Execute As Admin feature doesn't affect the Allow Non G/L Changes permission for editing period end journals. When you check the Allow Non G/L Changes box, users with the Allow Non G/L changes permission can edit journals that don't affect the general ledger. If you check **Execute As Admin**, that doesn't change the editing permissions for period end journals.
    
-   If you create a workflow that is initiated by users in the Employee Center, you'll usually need to enable **Execute As Admin**.
    

Note:

If your workflow has an Add Button action, when someone clicks the button and saves the record, the System Notes show the role of the user as Administrator, no matter what role they use. This is expected and is not related to the Execute As Admin box.

### Related Topics

-   [Creating a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4101527388.html)
-   [Release Status for Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2779229.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
