---
id: "section_N2751816"
type: "section"
title: "Subscribe To Record Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Subscribe To Record Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2751816.html"
anchors: ["bridgehead_4150463114", "bridgehead_0318113633"]
sha256: "2fa72d20709613ce5a5abf3c368b54aeb14bef7cb746e7a3c1c20c1597bd0a4f"
---

You're welcome to use the Subscribe To Record action to track any changes to a record instance after the action runs. Since the record is being tracked, you're able to create conditions for actions or transitions in the current workflow that rely on field value changes in the referenced record.

The Subscribe To Record action works best when paired with the Create Record action. For example, you're creating a Phone Call record in a workflow and then subscribing to it. You're then able to create another action that runs only if the status of the Phone Call record changes.

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Subscribe To Record action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Subscribe To Record Action Parameters {#bridgehead_4150463114}

The following table describes the Subscribe To Record action parameters:

| Parameter | Description |
| --- | --- |
| Field | Record field, from the record instance the workflow is processing, to track for changes. |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

## Subscribe To Record Action Guidelines {#bridgehead_0318113633}

Use the following guidelines when working with the Subscribe To Record action.

-   The Subscribe To Record action is not available on a Before Record Load trigger for a time entry record.
    
-   For an example of:
    
    -   Creating and subscribing to a Phone Call record, see [Creating and Subscribing to a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4144476357.html).
        
    -   A complete workflow that uses the Create Record and Subscribe To Record actions, see the [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html).
        
    -   Creating workflow and state fields to use with the Create Record and Subscribe To Record actions, see [Creating and Using Workflow Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103078253.html) and [Creating and Using State Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4108151274.html).
        

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Creating and Subscribing to a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4144476357.html)
-   [Create Record Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2741165.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
