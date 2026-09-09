---
id: "section_N2743016"
type: "section"
title: "Transform Record Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Transform Record Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2743016.html"
anchors: ["bridgehead_4150503917", "bridgehead_4448307314"]
sha256: "34e4e6b64ef13081cc408a435b1016b83c029bd50b06ff547c2c01a833f6e0c8"
---

Use the Transform Record action to transform the data on a transaction record into another transaction record type. When the action runs, you're getting a new instance of the target record type. You can create workflows that process transactions by turning them into the next record type in a transaction life cycle. For example, you can create a workflow to handle sales orders and generate invoices based on the right date range, amounts, or other criteria.

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Transform Record action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Transform Record Action Parameters {#bridgehead_4150503917}

The following table describes the Transform Record action parameters:

| Parameter | Description |
| --- | --- |
| Record Type | Type of record to create by transforming the workflow's current record. Only supported record types for the workflow's current record appear. |
| Store Result In | Workflow field or state field in which to store a reference to the created record. Create the field before configuring the Transform Record action. Use this field to subscribe to a created record with the Subscribe To Record action. See [Creating and Subscribing to a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4144476357.html). |
| Redirect without saving | Select to permit the user to edit the transaction before saving. |
| Field | Field values to populate when creating the new record instance of the selected **Record Type**. For each field, select the field name, set the appropriate properties in the corresponding columns, and click **Add**. The list of properties in the **Field** column changes depending on the selected **Record Type**. For more information, see [Setting Field Values in Action Definitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103787257.html). |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

## Transform Record Action Guidelines {#bridgehead_4448307314}

Use the following guidelines when working with the Transform Record action.

-   The Transform Record action does not appear on the **New Action** window if the base record type of the workflow does not support record transformation.
    
-   When you transform a record, the base record type for the workflow does not change.
    
-   The Transform Record action is not available on a **Before Record Submit** or **After Record Submit** trigger for a time entry record.
    
-   If the **Intercompany Cross-Subsidiary Fulfillment** feature is enabled, use SuiteScript to transform Sales Orders to Item Fulfillments. SuiteScript will let you pass the `inventoryLocation` transformation parameter. If SuiteScript is not an option and a workflow must be used, set Allow Cross Subsidiary Transaction to F and Inventory Location to blank for future transactions.
    
-   The functionality of the Transform Record action is the same as the SuiteScript 2.x method - [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html)
    

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Creating and Subscribing to a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4144476357.html)
-   [Setting Field Values in Action Definitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103787257.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
