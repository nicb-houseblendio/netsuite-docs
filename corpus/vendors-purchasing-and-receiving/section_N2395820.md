---
id: "section_N2395820"
type: "section"
title: "Approving a Purchase Request"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Purchase Requests > Approving a Purchase Request"
parent: "chapter_N2393987"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2395820.html"
anchors: ["bridgehead_N2395889", "procedure_N2395918", "bridgehead_N2395987"]
sha256: "75e320f7b854174d59b40f9ecef2faa43281a59b6e59739e427dadd0cef6470c"
---

If you use the Approval Routing feature for purchase approvals, purchases must be approved before they can be processed.

Purchase approvals are generally processed through the Employee Center. You must have the Employee Center role to access the Employee Center. An administrator can add the Employee Center role on your employee record. For more information, see [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html).

If your company doesn't use the Approval Routing feature, the request becomes a purchase order as soon as the immediate supervisor approves it.

Note:

In OneWorld accounts, when a user who is a supervisor or approver logs in to the Employee Center, note the following. Approval queues display purchase requests, expense reports, and requisitions entered by employees associated with all subsidiaries. Role-level subsidiary restrictions that apply to other records and transactions do not apply to approvals of purchase requests, expense reports and requisitions.

## Approving Purchases Using the Approval Routing Feature {#bridgehead_N2395889}

A supervisor or approver must have a purchase approval limit greater than or equal to the amount of the purchase request. If the amount is greater than the purchase approval limit, the request is sent to the next level of management. This process continues until it is approved by an authorized supervisor or approver.

If a purchase approver is specified for an employee, the supervisor is not part of the approval hierarchy.

If you use the Approval Routing feature, you must first log in to the Employee Center to approve a purchase request. You must have the Employee Center role to access the Employee Center. An administrator can add the Employee Center role on your employee record. For more information, see [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html).

#### To approve a purchase request using approval routing: {#procedure_N2395918}

1.  Log in to the Employee Center.
    
2.  Click **Approve Purchase Requests**.
    
3.  Select the name of the employee who submitted the request.
    
4.  Check the box next to the purchase request you want to approve.
    
5.  Click **Save**.
    

Supervisors can automatically be notified when they have requests to approve. Only an administrator can enable supervisor notification. To enable this preference, go to _Setup > Accounting > Preferences > Accounting Preferences_. Check the Automatically Notify Supervisors box.

In the Employee Center, your employees can view the status and approval history of their purchase requests by clicking View Purchase Requests/Orders.

## Approving Purchases Using SuiteFlow {#bridgehead_N2395987}

If you use SuiteFlow for purchase approvals, the steps to approve a purchase are dependent on the way the workflow is set up. For more information, see [Using Custom SuiteFlow Workflows for Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396465.html) and [Custom Workflow-based Approvals for Purchases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396564.html).

### Additional Information

-   [Using the Approval Routing Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2395258.html)
-   [Supervisors, Approvers, and Approval Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2395573.html)
-   [Approving an Expense Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396195.html)

### Related Topics

-   [Enabling Purchase Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162488295069.html)
-   [Entering a Purchase Request](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2394196.html)
-   [Creating a Purchase Order From a Purchase Request](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2394526.html)
-   [Notifying Supervisors of Purchase Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2394761.html)
-   [Purchase Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2393987.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
