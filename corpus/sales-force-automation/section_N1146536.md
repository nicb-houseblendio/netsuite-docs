---
id: "section_N1146536"
type: "section"
title: "Commission on Estimated Gross Profit"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Employee Commission Schedules > Commission on Estimated Gross Profit"
parent: "section_N1123341"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1146536.html"
anchors: []
sha256: "3962cb7acdb07337e4a39985d02c2f425ffcaaef55dd63d238244ad16ffd14b5"
---

You can pay commissions based on the estimated gross profit at the transaction line item level.

When you use estimated gross profit, you can compensate sales people throughout the sales cycle.

-   On the revenue side, the gross profit calculation could use the expected revenue for an opportunity, estimate, sales order, cash sale, or invoice.
    
-   On the cost side, you could use a user-defined amount, such as standard cost, average purchase cost, or most recent purchase cost. You could use the price charged by your preferred vendor, or price of the most recent purchase order your company issued to a vendor.
    

Important:

NetSuite flexibility lets you select revenue and cost values to calculate estimated gross profit that may not conform to Generally Accepted Accounting Principles (GAAP).

For information about how NetSuite calculates estimated gross profit, see [Estimating Gross Profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1752442.html).

To pay commission on estimated gross profit, you must use SuiteScript to populate the Alt. Sales (Alternate Sales Amount, ASA) field. This field appears on the Sales Order and Return Authorization forms. Use the following formula:

          `Amount - Est Extended Cost = Gross Profit` 
        

For detailed instructions and an example of how to calculate commissions with Alternate Sales Amount, see [Basing Commission on ASA](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1050405.html).

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Employee Commission Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1123341.html)
-   [Creating an Employee Commission Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1123495.html)
-   [Search-Based Commission Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1125679.html)
-   [Commission Calculation Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1126040.html)
-   [Commission Eligibility](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1129338.html)
-   [Commission Attainment and Payout Categorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1129540.html)
-   [Manager Commission Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1130290.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
