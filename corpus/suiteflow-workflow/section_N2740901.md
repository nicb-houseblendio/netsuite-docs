---
id: "section_N2740901"
type: "section"
title: "Remove Button Action"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > SuiteFlow Reference and Examples > Workflow Actions Overview > Remove Button Action"
parent: "section_4103695593"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2740901.html"
anchors: ["bridgehead_0311114950", "bridgehead_4147117610"]
sha256: "206af9d1ec8b062e9cd0550c231367801073ed45bf1ed76ea1ae302d9aec12b0"
---

Use the Remove Button action to remove buttons from a record form based on conditions, such as the user that views the record or the record's state.

Note:

Workflow definitions require a trigger configuration that initiates the workflow, executes an action within a workflow or transitions the workflow from one state to another.

-   For more information about which workflow triggers the Remove Button action supports, see [Workflow Triggers Quick Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150693781.html).
    
-   To understand when different workflow triggers run and which trigger you should use, see [Workflow Triggers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954788.html) and the [SuiteFlow Trigger Execution Model](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4077993199.html).
    

## Remove Button Action Parameters {#bridgehead_0311114950}

The following table describes the Remove Button action parameters:

| Property | Description |
| --- | --- |
| Button ID | ID of the button to remove from the record form. This can be either a standard NetSuite or custom button id. |

Note:

For more information about adding actions to a workflow, including common action properties and conditions, see [Action Conditions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html#bridgehead_4074297277) and [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html).

## Remove Button Action Guidelines {#bridgehead_4147117610}

Use the following guidelines when working with the **Remove Button** action.

-   You cannot use the **Remove Button** action to remove a button added with the Add Button action. To remove buttons added with the Add Button action, delete or inactivate the **Add Button** action.
    
-   The default trigger type for the **Remove Button** action is **Before Record Load**. Although the Entry and Exit triggers are available, the best practice is to remove the button before the record loads into the browser. In the Workflow FAQ section, see [Why do the buttons I have added to the record disappear when I refresh the browser?](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554318378.html#question_1554396621).
    

### Related Topics

-   [Workflow Actions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103695593.html)
-   [Creating an Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103049209.html)
-   [Workflow Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4071954161.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
