---
id: "section_N2395258"
type: "section"
title: "Using the Approval Routing Feature"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > Approval Routing > Using the Approval Routing Feature"
parent: "chapter_N2394992"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2395258.html"
anchors: ["bridgehead_3960260128"]
sha256: "2ea651eba4ef228e10d29699aa9f03f3a90d29df08176b5cb7aae66a1a32b495"
---

Approval Routing lets users with the Administrator or Employee Center role to require approval for specific purchase and expense transactions before they're processed. You set up an approval hierarchy to specify approvers for employees and set approval limits for expense reports, purchase requests, and purchase orders.

Note:

If you enable Approval Routing for specific purchase and expense transactions, you can only approve 25 of those transactions at a time.

To use this method, enable [Setting up Approval Routing](#bridgehead_3960260128). You don't use SuiteFlow workflows with this feature.

You can incorporate the Approval Routing feature into your workflow to process the following transaction types:

-   [Blanket Purchase Order Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4236988757.html)
    
-   [Approving an Expense Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396195.html)
    
-   [Invoice Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4171524249.html)
    
-   [Journal Entry Approval Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1471271.html)
    
-   [Purchase Contract Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4210416570.html)
    
-   [Purchase Order Approval Workflow SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2398841.html)
    
-   [Requisition Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3960249592.html)
    
-   [Revenue Arrangement Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1489444938.html)
    
-   [Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2376194.html)
    

After an employee enters an expense report, purchase request, or time transaction, the approval routing workflow may need extra steps depending on the following:

-   the employee's expense limit or purchase limit
    
-   the employee's designated supervisor or approver
    
-   the approval limit of the supervisor or approver
    

For example, an employee enters a purchase request for a new computer that costs $5000. According to our approval routing rules, the employee's supervisor must approve all purchase orders over $500. After it's approved, the request goes to purchasing for processing.

Note:

A supervisor needs access to the Employee Center to approve requests. A user with the Administrator role can add the Employee Center role to an employee record.

## Setting up Approval Routing {#bridgehead_3960260128}

To use the Approval Routing feature, a user with the Administrator role must enable the feature, assign roles, to employees, designate an approver, and set approval limits.

#### To use approval routing:

1.  Enable the Approval Routing feature.
    
    1.  Go to _Setup > Company > Setup Tasks > Enable Features_.
        
    2.  In the **Employees** subtab, check the **Approval Routing** checkbox.
        
    3.  Click **Save**.
        
2.  Assign [Assigning Roles to an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N897798.html).
    
3.  Designate [Supervisors, Approvers, and Approval Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2395573.html) on employee records.
    
4.  Set [Supervisors, Approvers, and Approval Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2395573.html).
    

Note:

To maintain the approval routing hierarchy, enter all expense reports and purchase requests through the Employee Center, even if employees have other roles.

For example, your A/P clerk can enter purchase requests in the A/P Clerk role, but to maintain proper approval routing, they must change to the Employee Center to enter the request. The supervisor can then approve the purchase request by logging in to the Employee Center.

### Related Topics

-   [Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2394992.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
