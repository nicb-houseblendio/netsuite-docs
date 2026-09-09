---
id: "section_N2396564"
type: "section"
title: "Custom Workflow-based Approvals for Purchases"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Purchasing > Purchase Order Approval Workflow SuiteApp > Custom Workflow-based Approvals for Purchases"
parent: "section_N2398841"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396564.html"
anchors: ["procedure_N2397148", "procedure_3892851084"]
sha256: "2786a39a05ffc8302679e5829a46f30962b5a8f678b507dafdeee8022f96e026"
---

You can choose to use SuiteFlow to create your own custom workflow to process purchase requests and purchase orders. Using SuiteFlow for purchases allows more flexible processes for approvals.

Note:

If you previously used the Approval Routing feature for purchase approvals, before you proceed, read [Switching From the Approval Routing Feature to SuiteFlow for Purchases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3960256538.html).

#### To use SuiteFlow to process purchase approvals:

1.  To enable features, go to _Setup > Company > Setup Tasks > Enable Features (Administrator)_.
    
    1.  On the **Transactions** subtab, verify that you have enabled the **Purchase Requests** or **Purchase Orders** feature.
        
    2.  On the **SuiteCloud** subtab, check the **SuiteFlow** box.
        
    3.  Click **Save**.
        
    4.  On the **Employees** subtab, check the **Approval Routing** box.
        
    5.  click **Save**
        
        This feature must be enabled to use these fields on employee records:
        
        -   Purchase Limit
            
        -   Purchase Approver
            
            These fields are required for use with the workflow.
            
2.  To enable the **Purchase Order Approval Routing** preference, go to _Setup > Accounting > Preferences > Accounting Preferences_.
    
    1.  On the **Approval Routing** subtab, check the **Purchase Order** box.
        
3.  Set up an approval workflow.
    
    You must use SuiteFlow to create a workflow to apply to your purchase requests and purchase orders. For details about setting up approval workflows, see [Creating Your First Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2725813.html).
    
    The following are some options you may consider incorporating into your purchase approvals workflow:
    
    -   Hierarchical or custom routing rules
        
    -   Email notifications that include links to drill down to records for approval
        
    -   Approve and Reject buttons
        
    -   Respecting approval limits
        
    -   Updating the Approval Status and Next Approver field on records
        
    -   Preventing records that are pending approval from being edited
        
    -   Designating an alternate approver
        

Note:

When using approval workflows, if the record is processed through multiple levels of approval by different users in a routing loop, note the following. You should use a custom workflow field that refer to the current approver's approval status. This enables you to track the current approver's approval status separately from the overall approval status of the record.

If you use SuiteFlow for purchase order approval, all purchase orders are created with a Pending Approval status by default. This includes drop ship and special order purchase orders.

You can always still manually set a purchase to an approved status for simple approvals.

## Employee Center {#procedure_N2397148}

When you use SuiteFlow for purchase approvals, the Employee Center is the primary workspace for processing purchase approvals.

-   The Employee Centers shows the Purchase Requests to Approve reminder and Approve Purchase Requests queue.
    
-   Employees are shown all purchases for which they are the next approver.
    
-   Users are not required to have the Full permission for the Employee Center to approve and reject purchases through the Employee Center. They can do so with only the View permission.
    
-   Reminders that show in the Employee Center drill down to the approval queue page for purchase requests, but not for expense reports. You can still click through notification email and use the buttons on the purchase form (such as Approve, Reject, etc.)
    
-   An approver that is associated with one subsidiary is able to see records that are associated with another subsidiary to make approvals.
    

#### To approve a purchase request using SuiteFlow: {#procedure_3892851084}

1.  Log in to the Employee Center.
    
2.  Click **Approve Purchase Requests**.
    
3.  Select a process in the **Action** field.
    
    The Action field lists the available actions of all purchase order workflows. For example, you can select the workflow action of Approve, or alternately select the action Reject.
    
    **Actions** available in the field are shown as follows:
    
    -   Workflow name
        
    -   Workflow state
        
    -   Workflow action
        
    
    For example, a workflow action selection could display:
    
    -   PO Approval Routing
        
    -   Pending Approval
        
    -   Approve
        
    
    The third section shows the action that will be implemented for the selected purchases. In the case above, that action is to Approve.
    
    The selection you make in the Action field filters the list of purchases that are displayed.
    
    For example, you select the action 'PO Approval Routing : Pending Approval : Approve'. The list of purchases that show are only ones that meet the following conditions:
    
    -   Uses the workflow named PO Approval Routing
        
    -   Has a status of Pending Approval
        
4.  After you select the workflow and action, check the **Select** box next to each purchase you want to process using the action.
    
5.  Click **Submit**.
    

You also have the option of manually selecting a status in the Approval Status field on a purchase.

### Additional Information

-   [SuiteFlow Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4068260113.html)
-   [Editing a Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4101529978.html)
-   [Supervisors, Approvers, and Approval Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2395573.html)
-   [Approving a Purchase Request](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2395820.html)
-   [Approving an Expense Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396195.html)

### Related Topics

-   [Purchase Order Approval Workflow Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2398992.html)
-   [Purchase Order Approval Workflow SuiteApp States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4158616141.html)
-   [Customizing the Purchase Order Approval Workflow SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2399147.html)
-   [Creating a Custom Purchase Order Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4158624611.html)
-   [Switching From the Approval Routing Feature to SuiteFlow for Purchases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3960256538.html)
-   [Purchase Order Approval Workflow SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2398841.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
