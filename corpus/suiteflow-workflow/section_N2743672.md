---
id: "section_N2743672"
type: "section"
title: "Lock Record Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Lock Record Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2743672.html"
anchors: ["bridgehead_4147087484"]
sha256: "e6cf6dfbc1b26f96b73d522e06fa0978fae2b9ff6011e88d4ef35e0d5196b37d"
---

Use the Lock Record action to remove the **Edit** button from a record belonging to the workflow's base record type. The record instance is locked during the time that it's in the workflow state where the Lock Record action is defined. To lock a record instance when it is in different workflow states, add the action to each state.

Besides the common workflow action parameters, the Lock Record does not have any additional configuration options. For more information about adding actions to a workflow, including common action properties, see [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Lock Record action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Lock Record Action Guidelines {#bridgehead_4147087484}

Use the following guidelines when working with the Lock Record action.

-   If you attempt to load a locked record using SOAP web services or SuiteScript, NetSuite throws an error and does not load the record.
    
-   The default trigger type for the Lock Record action is Before Record Load. Although the Entry and Exit triggers are available, the best practice is to lock the record before it loads into the browser.
    
-   Locked records still appear with the **Edit** option in the record list screen, but cannot be edited after they are loaded into the browser.
    
-   The Lock Record action is not available on a Before Record Load trigger for a time entry record.
    

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
