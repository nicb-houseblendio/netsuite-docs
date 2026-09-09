---
id: "section_N2740335"
type: "section"
title: "Add Button Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Add Button Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2740335.html"
anchors: ["subsect_157142435072", "subsect_157142432519"]
sha256: "3cc1fd73c8f6d56522094d76a33d713220f5ff7acf0cbd809ac3a67ebb122151"
---

The Add Button action is used to add a button to a record form. You can use the Add Button action to do any of the following:

-   Transition a record to the next state in a workflow. For more information, see [Using Buttons to Run Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103786185.html).
    
-   Go to another page or record. For more information, see [Using Buttons for Navigation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103786876.html).
    
-   Initiate mass processing for a specific base record type. For more information, see [Mass Processing Records in a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2796312.html).
    

In this example, we use the Add Button action to add Approve and Reject buttons to the purchase order form. For more information about transitions, see [Using Buttons to Run Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103786185.html).

![A purchase order with approve and reject buttons added with the Add Button action.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/AddButtonActionPurchaseOrderV2.png)

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Add Button action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Add Button Action Parameters {#subsect_157142435072}

The following table describes the Add Button action parameters:

| Parameter | Description |
| --- | --- |
| Label | Text that represents the button on the record form. If the Multi-Language feature is enabled on your account, you can add label translations. For more information, see [Configuring Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N247147.html) |
| Save Record First | Clear by default. When you check this option, if a user edits a record tied to the workflow, the button label (formatted as Save & <\_button label\_>) is added as an option to the Save button on the form. For example, if you add a button labeled Accept, the Save button will offer an option to Save & Accept. |
| Check Condition Before Execution | When you check this option, the workflow evaluates the conditions before executing the Add Button action. If the action has a saved search condition, the workflow will also evaluate if the record exists in the saved search results before executing the Add Button action. If you use this property in combination with the Save Record First box, when the user edits a record, the workflow evaluates the conditions using the updated and saved field values. If the updated field values cause the conditions to evaluate as false, or if the workflow can't evaluate the conditions, the workflow doesn't run the action. This property has no effect on an Add Button action that doesn't have a condition or saved search defined. **Tip:** Consider enabling Check Condition Before Execution for Add Button actions that depend on the record remaining in the current state. This option is especially useful when the state also includes conditions that can move the record automatically. |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

## Add Button Action Guidelines {#subsect_157142432519}

Following are behaviors to consider when using Add Button actions:

-   If you want the buttons to appear every time a user accesses the record, use the Before Record Load action trigger, and don't use the Entry trigger.
    
    Important:
    
    A button added during record load can remain visible after the workflow leaves the state. In that case, the button may no longer be valid for the current state.
    
    **Tip:** If a state includes an Add Button action and an automatic transition, add a condition to the Add Button action. Show the button only when the record is expected to remain in that state.
    
    For more information about action and transition processing order, see [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    
-   If a button should appear in multiple states, add the Add Button action to each state.
    
-   If you use the Add Button action to add buttons to a newly created record (triggered On Create), the buttons display but are disabled on the new record form.
    
-   If you create a workflow that includes an Add Button action, when a user interacts with the button and the record is saved, the System Notes will list the role of the user as Administrator, regardless of the role the user is logged in as.
    
-   SuiteFlow prevents workflow instances and actions from processing simultaneously in the following scenarios:
    
    -   A user double-clicks a workflow button.
        
    -   A user clicks workflow button A, then clicks workflow button B before the record page automatically refreshes.
        
    -   A user double-clicks a workflow button or clicks a sequence of workflow buttons. In this case, SuiteFlow alerts the user and asks whether to start processing the action when the previous action is still in progress.
        

Note:

A workflow button is a button added by an Add Button action.

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)
-   [Using Buttons to Run Transitions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103786185.html)
-   [Using Buttons for Navigation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103786876.html)
-   [Mass Processing Records in a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2796312.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
