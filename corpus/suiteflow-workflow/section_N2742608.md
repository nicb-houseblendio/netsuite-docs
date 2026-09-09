---
id: "section_N2742608"
type: "section"
title: "Go To Page Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Go To Page Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2742608.html"
anchors: ["bridgehead_4144571588", "bridgehead_4144595185"]
sha256: "5aab06c412012cfaad4886f649d96b207d0cd25c0e47a6a50be57a4c73c84906"
---

Use the Go To Page action to redirect users from a record in a workflow to a NetSuite page, including list views or reports.

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Go To Page action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Go To Page Action Parameters {#bridgehead_4144571588}

The following table describes the Go To Page action parameters:

| Property | Description |
| --- | --- |
| Page | Where you can select the NetSuite page or report to redirect to when the action executes. |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

## Go To Page Action Guidelines {#bridgehead_4144595185}

Use the following guidelines when working with the Go To Page action.

-   The Go To Page action is not available on a Before Record Submit or After Record Submit trigger for a time entry record.
    
-   If you want to redirect to a specific record instead of a list page or report, use the Go To Record action. See [Go To Record Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2742767.html).
    

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Go To Record Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2742767.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
