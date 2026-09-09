---
id: "section_N1129338"
type: "section"
title: "Commission Eligibility"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Employee Commission Schedules > Commission Eligibility"
parent: "section_N1123341"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1129338.html"
anchors: ["bridgehead_N1129406"]
sha256: "5ae13f16dc05534de056aa8d83d7834f88655fbfc76ff0a46f94850da867fd78"
---

Eligible commission is commission that can be authorized, and then paid. Commission becomes eligible when it meets the following conditions:

-   The commission passed the commission eligibility period set in the Commission Eligibility Period field. You can set the commission eligibility period at _Setup > Sales > Sales Management > Commissions_.
    
-   The commission has met the eligibility conditions set in the Eligible Amount field on the commission schedule.
    

## Collections-Eligible Commission and Credit Transactions {#bridgehead_N1129406}

If you use a commission schedule that calculates commission on collections, NetSuite determines the calculated or maximum commission to be paid on an order. (You can see this calculated or maximum amount on the Commission Overview or Estimated Commission reports.)

For collections-eligible commission schedules, this calculated amount is payable in an amount proportional to the payment collected on the invoice. This is the eligible amount that you can see when you authorize a commission payment, or on the Commissions Pending Authorization reports.

The calculated amount does not change based on the payments made to an invoice. The eligible amount changes when payment is made to the invoice.

When a credit memo is applied to an invoice, the payment collected reduces by the amount of the credit, decreasing the eligible commission amount, but not the calculated amount. For example, you use a commission schedule that pays 10% on sales and is eligible on collections. An invoice is entered in the amount of $1,000. The calculated commission is $100 payable proportional to payment collected. Due to a problem with the order, you apply a $200 credit memo to the invoice, in addition to the $800 payment. The invoice is now paid, and the eligible commission is $80. NetSuite did not create a negative commission amount. You applied the credit memo to the invoice, which removed $200 of commission eligibility.

An alternative example would be if the customer sends full payment on the invoice for $1,000, and then later you issue a $200 credit. You refund the customer $200. In this case, you received full payment and approved the full $100 commission. NetSuite then issued a negative eligible commission amount of -$20. The net commission is $80.

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Employee Commission Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1123341.html)
-   [Creating an Employee Commission Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1123495.html)
-   [Search-Based Commission Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1125679.html)
-   [Commission Calculation Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1126040.html)
-   [Commission Attainment and Payout Categorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1129540.html)
-   [Manager Commission Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1130290.html)
-   [Commission on Estimated Gross Profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1146536.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
