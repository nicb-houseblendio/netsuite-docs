---
id: "section_N1050405"
type: "section"
title: "Basing Commission on ASA"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Sales Forecasting > Alternate Sales Amounts > Basing Commission on ASA"
parent: "section_N1049780"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1050405.html"
anchors: []
sha256: "76e974293a9a6b0a116c34ab1780cf545953ba078b38dbfa04d892f64b2a5384"
---

With the Alternate Sales Amount feature, two new commission types are available on commission schedules: Alt. Sales Amount and Quota (Alt. Sales Amount).

Commission schedules based on ASA are similar to schedules based on sales. Commission schedules based on Quota (ASA) generate commission on the percentage of ASA quota met.

The commission preferences at _Setup > Sales > Sales Management > Commissions_ include a preference called Default ASA Collections Eligibility Type. Use this preference to define the default commission eligibility on ASA-based schedules as follows:

-   **First In** - Select this option to consider the amount paid on an order to first satisfy the ASA of a transaction for commission eligibility.
    
-   **Percent of Order** - Select this option if you want the ASA collections-based commission schedules to determine eligibility of calculated commissions. Eligibility is based on the proportion of cash collected against the sales order amount, rather than the ASA total.
    
-   **Whichever Is Greater** - Select this option to use the greater of the two preceding amounts when NetSuite determines commission eligibility.
    
-   **Whichever Is Less** - Select this option to use the lesser of the two preceding amounts when NetSuite determines commission eligibility
    

For example, a sales order has a total of $1,000 and the alternate sales amount is $500. The commission amount for this transaction is 10% of the ASA, or $50. A payment of $400 is received on the order.

**First In** - The $400 payment counts towards the ASA, making 80% ($400/$500), or $40, eligible for commission payment.

**Percent of Order** - The $400 payment is 40% of the order total, so 40%, or $20, of the calculated commission is eligible.

**Whichever Is Greater** - $40 is eligible because counting the payment towards the ASA gives a greater eligible amount.

**Whichever Is Less** - $20 is eligible because counting the payment as a percentage of the order total gives a smaller eligible amount.

For more information about creating commission schedules, see [Creating an Employee Commission Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1123495.html).

Sales orders and return authorizations include an Exclude Commissions box. Check this box to exclude the transaction from commission calculations.

### Related Topics

-   [Setting Up ASA](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1049956.html)
-   [Calculating ASA](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1050106.html)
-   [ASA Sales Forecasts and Quotas](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1050636.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
