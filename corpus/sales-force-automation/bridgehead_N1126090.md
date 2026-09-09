---
id: "bridgehead_N1126090"
type: "bridgehead"
title: "Marginal Calculation Scale"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Employee Commission Schedules > Commission Calculation Options > Marginal Calculation Scale"
parent: "section_N1126040"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1126090.html"
anchors: []
sha256: "db8fe09cc66dc9070d53c5766471fa3fb2a50c1552e44a8c9f468fd62beef79e"
---

Commission calculated on a marginal scale looks separately at the commission in each bracket.

NetSuite applies each percentage or amount you enter in the matrix only to the amount included in that bracket. NetSuite awards commission for each bracket at the rate you enter for that bracket.

In some cases, a transaction may cause a sales rep to qualify for a higher commission bracket. The portion of the transaction in the lower bracket receives the commission rate for the lower bracket. The portion of the transaction in the higher bracket generates commission at the rate of the higher bracket.

Note:

The exceptions to this are sales-based and quota-based commission schedules that consider categories for the purpose of commission payout, for example, when you selected Payout Only in the Categorization Applies To field. When a transaction makes the sales total for the period qualify for the next bracket, NetSuite applies this bracket rate to the entire transaction.

For example, if a schedule awards commission based on sales by period using a marginal scale, the commission matrix would look like this:

![Screenshot of a sample commission calculation using a marginal scale.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/MarketingSalesForceAutomationPartners/SalesForceAutomation/comm_calculation_marginal_matrix.png)

A rep with this schedule in their plan would earn commission on the following transactions:

| Tran. # | Transaction Amount | Period Total | Commission | Notes |
| --- | --- | --- | --- | --- |
| 1 | $8,000 | $8,000 | $0 | No commission is earned until the transaction total for the period reaches $10,000. |
| 2 | $3,000 | $11,000 | $40 | The first $2,000 of this transaction earns no commission. $1,000 of this transaction generates 4% commission, or $40. |
| 3 | $5,000 | $16,000 | $202.50 | The first $4,000 of this transaction earns $160, or 4%. The other $1,000 of this transaction generates 4.25% commission, or $42.50. |
| 4 | $2,000 | $18,000 | $85 | This entire transaction is within the 4.25% bracket. |

The total commission for the period (the sum of the Commission column in this example) is $327.50.

A rep assigned a quota-based schedule on a marginal scale that categorizes by class to determine payout only, would have the following commission matrix:

![Screenshot of a sample commission using a marginal scale that categorizes by class to determine payout only.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/MarketingSalesForceAutomationPartners/SalesForceAutomation/commission_marginal_PayoutOnlyMatrix.png)

In this example, the rep's overall quota for the period is $10,000. Their sales and commission amounts for the period are the following. The fourth column shows how much of each transaction is classified as recurring business.

| Tran. # | Transaction Amount | Period Total | Recurring Business Amount | Commission | Notes |
| --- | --- | --- | --- | --- | --- |
| 1 | $8,000 | $8,000 | $4,000 | $0 | No commission is earned until the transaction total for the period reaches $10,000. |
| 2 | $2,500 | $10,500 | $1,000 | $30 | Because this transaction brings the total into the second bracket, the commission rate of 3% is applied to the recurring business amount of the whole transaction. |
| 3 | $1,000 | $11,500 | $1,000 | $35 | This transaction qualifies for the 3.5% rate in the third bracket. |
| 4 | $2,000 | $13,500 | $5,000 | $225 | This transaction qualifies for the 4.5% rate in the highest bracket. |

The total commission earned for the period (the sum of the Commission column) is $290.

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Commission Calculation Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1126040.html)
-   [Commission Eligibility](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1129338.html)
-   [Flat Rate Calculation Scale](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1126056.html)
-   [Linear Calculation Scale](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1129208.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
