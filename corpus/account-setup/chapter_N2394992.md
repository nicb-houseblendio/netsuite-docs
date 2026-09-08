---
id: "chapter_N2394992"
type: "chapter"
title: "Approval Routing"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > Approval Routing"
parent: "book_N125907"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2394992.html"
anchors: ["subsect_156806140378"]
sha256: "5cd7d1d1587332efcbcf93a3ba7216e209f389d91e738ecc893ce43ee49f2088"
---

NetSuite Approval Routing helps your organization define who can approve employee purchase transactions and limit approval amounts by authorizer level and department. This feature helps you control spending by letting managers better understand your organization's approval process. When everyone's more aware of costs, management and staff can work together to reduce unnecessary spending.

-   The **Approval Routing Feature** is the most basic NetSuite approval routing option.
    
    To learn more, see [Using the Approval Routing Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2395258.html).
    
-   **Standard Suiteflow Workflows** provide a simple and flexible approvals process.
    
    To learn more, see [Using Standard SuiteFlow Workflows (SuiteApps) for Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3959476640.html).
    
-   **Customized SuiteFlow Workflows** offer the most flexibility for processing approvals.
    
    To learn more, see [Using Custom SuiteFlow Workflows for Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396465.html).
    

Important:

No matter which approval method you use, your approval settings apply to everyone in your company.

## Posting Period for Transactions Subject to Approval {#subsect_156806140378}

When a posting transaction needs approval, the posting period is set after the transition is approved. (Non-posting transactions don't have a posting period.) The Posting Period shown for transactions that are pending approval can change when the transaction is approved.

The Posting Period value you see for **pending approval** transactions depends on your role, accounting preferences, and the status of the period as follows:

-   If the period for the transaction date is open and not locked, you'll see that period in the Posting Period field.
    
-   If the period for the transaction date is open but locked and you have the **Override Period Restrictions** permission, you'll see that period as the Posting Period.
    
-   If the matching period is open but locked and you **don't** have the override permission, the system treats it as closed.
    
-   If the matching period is closed, you'll see either the first open period or the current period for the Posting Period, depending on the . The accounting preference **Default Posting Period When Transaction Date in Closed Periods** determines which period is displayed.
    

When you approve a posting transaction, you can select a different Posting Period than the one shown initially. You can't select a closed period, but you may be able to select an open and locked period if you have the Override Period Restrictions permission.

When you save approved transactions, you may see warnings or errors, depending on the transaction and your accounting settings. The following accounting preferences also affect the posting period. For details, see [General Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html).

-   Allow Transaction Date Outside of Posting Period
    
-   Create and Edit Inventory Transactions Dated in Closed Period
    
-   Allow Inventory Transactions Dated Outside the Posting Period
    

### Related Topics

-   [Account Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N125907.html)
-   [Centers Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N131898.html)
-   [Enabling Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N232138.html)
-   [NetSuite Company Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N239909.html)
-   [Classifications in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N261411.html)
-   [NetSuite Users & Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N284861.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
