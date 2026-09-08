---
id: "section_N2395573"
type: "section"
title: "Supervisors, Approvers, and Approval Limits"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > Approval Routing > Using the Approval Routing Feature > Supervisors, Approvers, and Approval Limits"
parent: "section_N2395258"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2395573.html"
anchors: []
sha256: "b6a2dd80750c7681f59c5f4a949502b27e027037d12a9015fd45c7603040cccd"
---

Use Approval Routing to set up a hierarchy of supervisors and approvers who approve purchase and expense transactions before they're processed.

For purchase approvals processes, clear the Purchase Order preference for Approval Routing. To learn more, see [Using Custom SuiteFlow Workflows for Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396465.html). For expense approvals, the process is the same and is not affected by the preference setting.

After a transaction is entered by or routed to an employee for approval, the employee's record settings define which transactions need additional approval. These settings include the following:

-   **Supervisor** - The employee's direct supervisor
    
-   **Expense Limit** - The amount the employee can expense without supervisor or approver approval
    
-   **Expense Approver** - The person who approves the employee's expense reports. If no approver is selected, the supervisor approves expense reports. If an expense approver is selected, the supervisor is no longer part of the approval hierarchy
    
-   **Expense Approval Limit** - The maximum amount an employee can approve on an expense report when specified as an approver for another employee
    
-   **Purchase Limit** - The amount an employee can purchase without supervisor or approver approval
    
-   **Purchase Approver** - The person who approves the employee's purchase requests. If no approver is selected, the supervisor approves purchase requests. If a purchase approver is selected, the supervisor is no longer part of the approval hierarchy
    
-   **Purchase Approval Limit** - The maximum amount an employee can approve on a purchase request when specified as an approver for an employee
    

To learn how to enter employee records settings, see [Entering Human Resources Information for an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N895403.html).

For each employee, set an expense or purchase limit to determine the highest transaction amount the they can enter without additional approval. If they enter an expense report or purchase request below their limit, the transaction is automatically approved.

If the employee enters a transaction over their limit, the transaction follows the approval routing process. The transaction goes to a supervisor or approver with an approval limit that's high enough for the amount.

Note:

Employee and approval limits are enforced using the currency set on the employee record. If a transaction is in a foreign currency, the total is converted to the employee's currency before checking the limits.

Approval is requested from the supervisor or approver listed on the employee record until enough approval authority is found.

If no one has enough authority, you'll see an alert on the transaction.

### Related Topics

-   [Using the Approval Routing Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2395258.html)
-   [Using Standard SuiteFlow Workflows (SuiteApps) for Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3959476640.html)
-   [Using Custom SuiteFlow Workflows for Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396465.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
