---
id: "section_N1251398"
type: "section"
title: "Billing Schedules"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Advanced Billing > Billing Schedules"
parent: "section_N1250607"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251398.html"
anchors: []
sha256: "afd1ea9d1eeb74b038a24935ef42a669d514852f2363bcfa69a50648bc987cc2"
---

A billing schedule outlines when to bill a sale over time or a contract term. For example, you might bill monthly for a one-year membership or quarterly for a three-year service contract. Billing schedules manage the billing process by tracking when to invoice customers and how much to bill.

For example, you're able to create a billing schedule with an initial 50% billing amount, monthly recurrence, and two recurrences. When you apply this billing schedule to a $1,000.00 service contract sales order, it's billed as follows:

-   Initial invoice for 50% of the sale = $500.00
    
    The balance of the amount due is automatically split evenly between remaining bills.
    
-   Second invoice one month later for 25% of the sale = $250.00
    
-   Third invoice one month after the second for 25% of the sale = $250.00
    

You can set up billing schedules to accommodate various sales types. Some sales require a fixed currency amount upfront, while others need a percentage of the total. Sales may require weekly, monthly or quarterly recurrent invoices. You can set billing to recur monthly 12 times or quarterly 3 times, or even customize bill recurrence schedules to suit your needs.

You can apply a billing schedule to an entire sales order or choose a different schedule for each line item. You can assign a default billing schedule to an item record, which then appears on sales orders when you select that item.

You can also create a new billing schedule from an estimate or sales order. Billing schedules created from estimates or sales orders can be marked as Public or Private. Private billing schedules show in the list of billing schedules only on the transaction it is created from. Note that milestone billing schedules cannot be marked Public. If you manually click Next Bill to bill a sales order and there are remaining lines from the previous schedule that weren't billed, NetSuite bills them on the next billing date. Now, click Next Bill again to move to the next billing date. To remove a line from a billing schedule, close the line on the sales order. If you delete the line, your billing schedule amounts could be different from expected.

With a billing schedule, NetSuite requires fulfillable items to be fulfilled and fully billed on the first invoice before moving to the next one. If an item isn't fulfilled or fully billed, the billing schedule doesn't advance.

When you view an estimate or sales order, you can click the Schedule link at the top of the page to open the schedule record. On sales orders, you can view the billing schedule by clicking the Schedule subtab.

Note:

You can edit a billing schedule associated with an open sales order, but it won't update existing instances for that order. To update existing instances, go to _Transactions > Sales > Enter Sales Orders_ > List to open the sales order and re-save it. Upon saving, the billing schedules are updated with your changes.

Billing schedules affect your sales forecast report by dividing revenue across the billing schedule period. A sales order with a billing schedule is calculated into forecast schedules based on the initial and subsequent billing amounts and on the billing start date. Sales forecasts for a particular period include amounts set to be billed in that period.

### Related Topics

-   [Advanced Billing Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1250795.html)
-   [Enabling Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251128.html)
-   [Creating Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1252880.html)
-   [Creating Billing Schedules From an Estimate or Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253492.html)
-   [Applying Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253848.html)
-   [Discount and Markup Items and Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254542.html)
-   [Billing Customers Using Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254744.html)
-   [Viewing Invoice Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256403.html)
-   [Advanced Billing and Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256787.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
