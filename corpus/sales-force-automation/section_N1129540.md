---
id: "section_N1129540"
type: "section"
title: "Commission Attainment and Payout Categorization"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Employee Commission Schedules > Commission Attainment and Payout Categorization"
parent: "section_N1123341"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1129540.html"
anchors: []
sha256: "e6188bace5d1931d45f8bb95804f4b0fa8c1b8db939f89bb385ca9b7ae82600c"
---

In a quota-based schedule or schedule based on sales on a marginal scale, you can decide how to use categories - either to determine payout alone, or both payout and attainment of commission.

For schedules that categorize both attainment and payout, the percentages in the header row of the matrix refer to the categorized quota or sales. The categorized quota or sales are based on class, location, items, or departments. After you determine which bracket the categorized amount fulfills, NetSuite applies the percentage to the category amount.

Note:

The exceptions to this are sales-based and quota-based commission schedules that consider categories like class or location for the purpose of commission payout (schedule where **Payout Only** is the default in the **Categorization Applies To** list). Therefore, when a transaction makes the period sales total qualify for the next bracket, NetSuite applies this bracket rate to the entire transaction.

For more information about how NetSuite calculates commissions, see [Commission Calculation Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1126040.html).

![Screenshot of a sample commisson calculation using the attainment categorization.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/MarketingSalesForceAutomationPartners/SalesForceAutomation/commission_marginal_AttainmentAndPayout.png)

You must establish an uncategorized quota and a quota for categories (class, location, department, or item) on which you base your quota. For example, Wolfe Electronics uses a schedule where **Calculation Scale** is **Marginal**, **Rate** is **Percentage**, and **Categorization applies to** is **Both Attainment AND Payout**.

Reps have a monthly Recurring Business quota of $10,000. The following transactions occurred during this period:

| Tran. # | Recurring Business Amount | Period Total | Commission | Notes |
| --- | --- | --- | --- | --- |
| 1 | $8,000 | $8,000 | $0 | No commission is earned until the recurring business amount for the period reaches $10,000. |
| 2 | $3,000 | $11,000 | $30 | The first $2,000 of this transaction does not qualify for commission. The other $1,000 generates commission at the 3% rate, or $30. |
| 3 | $1,500 | $12,500 | $55 | $1,000 of this transaction is in the 3.5% bracket, and $500 is in the 4% bracket. |
| 4 | $2,000 | $14,500 | $87.50 | The first $500 qualifies at 4%, and the other $1,500 is in the 4.5% bracket. |

The total commission earned on the schedule is $172.50.

On commission schedules that apply categorization to payout only, the percentages in the header row of the matrix refer to the non-categorized quota (quota not based on class, location, items, or departments). In these schedules, you must decide the commission rate. First, determine how much of a transaction fulfills the non-categorized quota. Then, apply the percentage in the column for that category to the sales amount associated with that category on the transaction.

![Screenshot of a sample commission calculation using the payout categorization.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/MarketingSalesForceAutomationPartners/SalesForceAutomation/commission_quotaPayoutSchedule.png)

For example, Wolfe Electronics uses a schedule where **Calculation Scale** is **Marginal**, **Rate** is **Percentage**, and **Categorization applies to** is **Payout Only**. The bracket used to calculate commission is determined by the extent to which reps attained their overall, uncategorized quota. NetSuite applies the percentage rate to the sales in each class to calculate commission.

One Wolfe Electronics sales rep closed a sale categorized as **New Business : Large** , which enabled them to reach the 110% of quota bracket. They received 6% of that transaction amount. If they were assigned the preceding schedule (**Categorization applies to** is **Both Attainment AND Payout**), they would have quotas established for each class:

| Class | Quota |
| --- | --- |
| Reseller | $2,000 |
| Recurring Business | $3,000 |

When they reach their quota for sales to resellers, they earn 5% of each sale to resellers up to $2,200 (110% of their Reseller quota). When their recurring customer sales reach $3,600 (120% of quota), they receive 4% of each sale in this class, up to the next commission bracket ($3,900, or 130% of recurring customer quota.)

The **Categorization applies to** field appears on commission schedules that meet the following criteria:

-   Based on Quota (Sales Amount), YTD Quota, Quota (Alt. Sales Amount), YTD Quota (Alt. Sales Amount), and Sales
    
-   Categorized by class, items, locations, departments, or parents of any of these categories
    

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Employee Commission Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1123341.html)
-   [Creating an Employee Commission Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1123495.html)
-   [Search-Based Commission Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1125679.html)
-   [Commission Calculation Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1126040.html)
-   [Commission Eligibility](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1129338.html)
-   [Manager Commission Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1130290.html)
-   [Commission on Estimated Gross Profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1146536.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
