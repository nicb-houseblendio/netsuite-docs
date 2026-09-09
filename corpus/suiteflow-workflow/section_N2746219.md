---
id: "section_N2746219"
type: "section"
title: "Send Campaign Email Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Send Campaign Email Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2746219.html"
anchors: ["bridgehead_4147909200"]
sha256: "23ba6636d65ebcc0bfd0886059ce9598649af09767954228c3c1307e7b177725"
---

Use the Send Campaign Email action to send an email as part of a marketing initiative. You can use this action in a workflow for any record type, although it is commonly used with Customer, Lead, or Prospect record types. Use the Send Email Campaign action in a lead nurturing workflow to manage leads in a marketing campaign. For a sample workflow that uses a Send Campaign Email action, see [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html).

Use this action in conjunction with the Marketing Automation feature. For more information about the Marketing Automation feature, see [Marketing Automation Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N973384.html).

To use the Send Campaign Email action, you specify the recipient of the email and the campaign event, and an optional workflow field to track the customer responses to the campaign event. Use the Subscribe To Record action to track responses to the campaign event. For more information about campaign events, see [Managing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N985526.html).

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Send Campaign Email action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Send Campaign Email Action Parameters {#bridgehead_4147909200}

The following table describes the Send Campaign Email action properties:

| Property | Description |
| --- | --- |
| Record | Record that contains the entity from which the email address is used to send the campaign. The default selection is **Current Record**. |
| Field | An entity from the **Record** to which the email campaign is sent. For example, the current record's **Customer** field has an **Email** address that will receive the campaign. |
| Campaign Event | Title of the campaign event for the associated marketing campaign. For more information about campaign events, see [Campaign Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N987776.html). |
| Store Result In | Workflow field to store the campaign event response. Use this field in a Subscribe To Record action to track the response from the campaign recipient. See [Creating and Using Workflow Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103078253.html) and [Subscribe To Record Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2751816.html). |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
