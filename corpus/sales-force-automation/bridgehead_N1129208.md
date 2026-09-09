---
id: "bridgehead_N1129208"
type: "bridgehead"
title: "Linear Calculation Scale"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Employee Commission Schedules > Commission Calculation Options > Linear Calculation Scale"
parent: "section_N1126040"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1129208.html"
anchors: ["bridgehead_N1129251"]
sha256: "416b9c6ef25a8b9d7b6a93c939b7726735188b53e2a8f00b3adc99f87ac2647c"
---

For commission schedules that use a linear calculation scale, NetSuite applies the highest qualified bracket rate to the total sales for that period or transaction.

When the lowest commission bracket is reached, NetSuite does not calculate the eligible total or calculated amount for the sales order. For example, using the schedule shown, if a commission transaction base amount is below the first bracket, calculated and eligible amounts are zero.

This differs from the marginal calculation scale, which awards the sales amounts in each bracket at that bracket's rate. For example, a schedule awards commission based on sales that use a linear scale have a commission matrix like this:

![Screenshot of a sample commission calculation using a linear scale.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/MarketingSalesForceAutomationPartners/SalesForceAutomation/comm_calculation_marginal_matrix.png)

A rep with this schedule in their plan made $22,000 in sales during the period, the commission amount is 4.35% of $22,000, or $957.

## Target Factor Commission {#bridgehead_N1129251}

If you create a schedule based on quota that uses a linear scale, choose **Target Factor** for the **Rate** setting. These schedules award a percentage of the target factor as commission. NetSuite determines the percentage by the percentage of quota met, for example, a schedule awards commission based on quota and calculates commission amounts from a target amount of $10,000. If a rep with this schedule in their plan made 125% of their quota, they would earn $7,500, computed as follows:

factor of quota attained \* attainment bucket factor \* target amount

1.25 \* .60 \* 10,000

Important:

Sales transaction pages such as Sales Order, Invoice, Credit Memo, Cash Sales, Cash Refunds, and Return Authorizations have an Exclude Commissions box. If a user checks this box on a sales transaction page, NetSuite excludes the transaction and its subordinate transactions from inclusion in commission calculations. For example, if a user checks this box on a sales order, NetSuite excludes the sales order and the subsequent invoice from all commission calculations for all sales people.

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Commission Calculation Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1126040.html)
-   [Commission Eligibility](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1129338.html)
-   [Flat Rate Calculation Scale](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1126056.html)
-   [Marginal Calculation Scale](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1126090.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
