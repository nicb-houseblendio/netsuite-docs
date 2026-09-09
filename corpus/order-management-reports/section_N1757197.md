---
id: "section_N1757197"
type: "section"
title: "Setting the Recalculate Estimated Cost on Creation of Linked Transactions Preference"
branch: "order-management-reports"
category: "order-management"
breadcrumb: "Order Management > Order Management Reports > Estimating Gross Profit > Setting Up Gross Profit > Setting the Recalculate Estimated Cost on Creation of Linked Transactions Preference"
parent: "section_N1756747"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757197.html"
anchors: []
sha256: "7bae246a28bd647536fe0f6b0936865db5d280af6af25efe89560f66375f5afd"
---

The following figure shows the **Recalculate Estimated Cost on Creation of Linked Transactions** preference at _Setup > Accounting > Accounting Preferences_, on the Items/Transactions tab:

![location of the Recalculate Estimated Cost on Dreation of Linked Transactions preference (under Other Transaction Preferences)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/OrderManagementReports/OtherTransPref.png)

Because a sales cycle can take weeks, months, or even longer, the estimated costs and resulting gross profit of a transaction can change. For example, estimated cost can change as a sale progresses from opportunity to estimate to sales order to invoice. The **Recalculate Estimated Cost on Creation of Linked Transactions** preference controls whether NetSuite automatically updates estimated cost and gross profit values as a transaction moves through the sales cycle. When you create a transaction from another transaction, this preference can allow you to recalculate the gross profit using the latest cost estimate.

This preference has three options:

-   **Through Sales Order -** Triggers the recalculation of estimated gross profit on transactions up to and including sales orders, but excludes invoices. Provides the most up-to-date cost and gross profit estimates.
    
-   **Always -** Causes the recalculation of estimated gross profit at all stages in the sales cycle. This option would result in a gross profit estimate closer, over time, to the final actual costs and gross profit.
    
-   **Never -** Prevents the recalculation of estimated gross profit when an item's cost changes.
    

Be aware that these preferences only apply to linked transactions, meaning transactions that are generated from other transactions.

You also can assign a permission to users to allow them to modify estimated costs on transactions. See [Granting the Override Estimated Costs on Transactions Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757391.html).

### Related Topics

-   [Setting Up Gross Profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1756747.html)
-   [Enabling the Gross Profit Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1756926.html)
-   [Granting the Override Estimated Costs on Transactions Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757391.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
