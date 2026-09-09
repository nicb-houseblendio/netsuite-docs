---
id: "section_N2381204"
type: "section"
title: "Customizing for the Vendor Bill Approval Workflow"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Bills > Vendor Bill Approval Workflow > Customizing for the Vendor Bill Approval Workflow"
parent: "section_N2376194"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2381204.html"
anchors: ["bridgehead_N2381216", "bridgehead_N2381264", "procedure_N2381276", "procedure_N2381357", "bridgehead_N2381460", "procedure_N2381475", "bridgehead_N2381505", "bridgehead_N2381521"]
sha256: "d0f0dcf7cdd3f6a3a50a209b3ea619a926cb7fb15e63e3b99d7ae626ea18c56b"
---

After you have installed the Vendor Bill Approval Workflow, you can customize the workflow and searches to suit your specific needs.

## Customizing the Saved Searches {#bridgehead_N2381216}

The following saved searches show in your NetSuite account after your successful installation:

-   Vendor Bill PO Amount Check
    
-   Vendor Bill PO Quantity Check
    
-   Vendor Bill PO Partial Rcpt QTY Check
    
-   Vendor Bill Standalone Check
    

To customize one of these reports, go to _Reports > Saved Searches > All Saved Searches_, and click Edit next to the name of the search.

## Customizing the Workflow {#bridgehead_N2381264}

After you install Vendor Bill Approval, the workflow that is used is set to have default parameters. You can change the workflow to incorporate new parameters that are tailored to your needs.

Note:

The workflow may be locked. For information about editable options, see [Editing a Locked Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4846726513.html).

#### To customize the default workflow states: {#procedure_N2381276}

1.  Disable the Vendor Bill Approval Workflow.
    
2.  Copy the bundle workflow.
    
3.  Modify the workflow as required.
    
    For information about workflow, see [SuiteFlow (Workflow)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N2723865.html).
    
4.  Deploy the new workflow.
    

The following defines the default states for the installed workflow:

-   Bill Validation
    
-   Exceptions
    
-   Pending Approval
    
-   Approved
    
-   Rejected
    

## Bill Validation State {#procedure_N2381357}

If a vendor bill is Pending Approval, the workflow sets the initial state of the transaction to bill validation. This bill validation state will set the next approver to the supervisor of the individual entering the transaction.

The bill validation state will have several transitions to the following states.

-   **Exceptions**
    
    The vendor bill will transition to the Exceptions state if the following is true:
    
    -   The purchase order is only partially received.
        
    -   The purchase order amount is less than the bill amount.
        
    -   The purchase order quantity is less than the bill quantity.
        
-   **Pending Approval**
    
    The vendor bill will be considered for transitioning to the pending approval state if the vendor bill is a standalone bill.
    
-   **Approved**
    
    The vendor bill will transition to an Approved state if the bill doesn't transition to the Exceptions or Pending Approval state.
    

## Exception State {#bridgehead_N2381460}

When a vendor bill transitions to an Exception state, NetSuite identifies the exact exception by a message in the Memo field. This message can be customized.

Any vendor bill in an Exception state will next transition to the Pending Approval state.

## Pending Approval State {#procedure_N2381475}

When a transaction is in the Pending Approval state, a user with permission has the option to approve or reject a transaction. Vendor bills in this state display an Approve button and a Reject button for this purpose.

-   Click Approve to prompt NetSuite to move the bill to [Approved State](#bridgehead_N2381505) state.
    
-   Click Reject to prompt NetSuite to move the bill to [Rejected](#bridgehead_N2381521) state.
    

## Approved State {#bridgehead_N2381505}

A vendor bill that reaches the Approved state has its approval status set to Approved.

The Approved state is an end state. After this state is reached, you can"t change the state from Approved to any prior state.

## Rejected {#bridgehead_N2381521}

A vendor bill that reaches the Rejected state has its approval status set to Rejected.

A vendor bill in the Rejected state can be changed back to a Pending Approval status.

### Additional Information

-   [Vendor Bill Approvals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373552.html)
-   [3 Way Match Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4096219721.html)
-   [Vendor Bill Approvals in the Employee Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157528106765.html)

### Related Topics

### Related Topics

-   [Installing the Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2380890.html)
-   [Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2376194.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
