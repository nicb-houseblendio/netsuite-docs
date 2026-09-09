---
id: "section_N1147526"
type: "section"
title: "Recalculating Commission"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Employee Commission Plans > Recalculating Commission"
parent: "section_N1146679"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1147526.html"
anchors: []
sha256: "e7615c38ba525022e752088a433c23cd15809872f0babc5776f1085b3283adba"
---

Many commission-related changes prompt NetSuite to automatically recalculate commission amounts, such as the following changes made to commission plans or schedules:

-   Change the date range a rep is assigned to a plan
    
-   Assign new sales reps to a plan
    
-   Edit a commission schedule assigned to a plan
    
-   Add or remove commission schedules to or from a plan
    

Also, the following changes to transactions can require commission recalculation:

-   Changes to dates, amounts, and other transaction fields
    
-   Change the order in which transactions are entered
    
    For example, you backdate a transaction to a previous month that requires an update to YTD Quota schedules.
    

The following changes do not automatically prompt commission recalculation, but might cause a change to commission amounts:

-   Changes in the sales rep hierarchy (for example, a change in supervisors)
    
-   Changes to quotas
    
-   Adjustments to profit and Cost of Goods Sold (COGS)
    
-   Item fulfillment
    

If you make a change that does not automatically recalculate commission, you can manually recalculate commission. Open the commission schedule or commission plan for which you want to recalculate commission, and then click the Recalc button.

Note:

When a change occurs that triggers an automatic recalculation, it is not in real time. NetSuite adds the recalculation operation to a queue to be processed. The number, complexity, and size of the items in this queue determine the time it takes to process. Even when you choose to manually recalculate, NetSuite adds the recalculation operation to the queue. You can view the status of the recalculation operation on the commission plan and commission schedule list pages in the Recalculating column.

NetSuite automatically recalculates commission when an order is billed. For commission based on profitability or total profit, you may be required to recalculate commission. For example, if you bill or invoice customers prior to fulfillment, you must manually recalculate prior to commission authorization.

Important:

Sales transaction pages such as Sales Order, Invoice, Credit Memo, Cash Sales, Cash Refunds, and Return Authorizations, have an **Exclude Commissions** box. If you check this box on a sales transaction page, NetSuite excludes the transaction and its subordinate transactions from inclusion in all commission calculations.

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Employee Commission Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1146679.html)
-   [Creating an Employee Commission Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1146859.html)
-   [Assigning Sales Reps to a Commission Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1147232.html)
-   [Sales Effective Date](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1147809.html)
-   [Split Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1148007.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
