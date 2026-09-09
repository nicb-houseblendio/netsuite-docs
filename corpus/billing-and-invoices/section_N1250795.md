---
id: "section_N1250795"
type: "section"
title: "Advanced Billing Overview"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Advanced Billing > Advanced Billing Overview"
parent: "section_N1250607"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1250795.html"
anchors: []
sha256: "d7615cc8a090ac23eb2d750bf347e0e18797a74879a2980c035020eeb9cedf53"
---

Advanced billing enables you to create billing schedules to invoice sales over a range of time or a contract term. For example, a service company can use advanced billing for recurring sales like a monthly membership.

Billing schedules manage the billing process to track when to invoice customers and how much to bill.

When you assign a billing schedule to a sale, NetSuite adds a bill to the billing queue at the scheduled intervals. Then, you're able to create the invoices in the billing queue by going to _Transactions > Sales > Bill Sales Orders_.

The initial bill for each schedule is created on the date entered in the Start Date field of the order. If you don't enter a start date, the first invoice is created when you fulfill or partially fulfill the order.

For example, you can apply a billing schedule with an initial 50% billing amount, monthly recurrence, and two recurrences. If the sales order totals $1,000.00 and the Start date is January 15th, the sales order will be billed as below:

-   Initial invoice for 50% of the sale = $500.00 billed on January 15th
    
    The balance of the amount due is automatically split evenly between remaining bills.
    
-   Second invoice for 25% of the sale = $250.00 billed on February 15th
    
-   Third invoice for 25% of the sale = $250.00 billed on March 15th
    

When viewing a sales order, you can click the Schedule link at the top of the page to open the schedule record.

For orders with outstanding billings, you can manually create the remaining bills before they're generated from the billing schedule. You can create the next bill on the billing schedule, or you can bill all of the remaining unbilled portion of the order.

You can set a preference to Invoice in Advance of Fulfillment:

-   Enable this preference to invoice customers for the full amount before an order is fully fulfilled. With this preference, you can invoice your customers in advance for an entire order that is shipped in parts.
    
-   Disable this preference to limit fulfillment quantities to the remaining quantities.
    

Set the preference at _Setup > Accounting > Preferences > Accounting Preferences_ > Order Management > Invoicing. For more information, read [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1384948.html) and [Billing Orders Using Advanced Shipping with Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1257068.html).

Important:

The Advanced Billing feature requires that you also enable the Sales Orders feature.

Billing schedules can also be used with the Project Management feature. For details, read [Project Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html#bridgehead_N1180158).

### Related Topics

-   [Enabling Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251128.html)
-   [Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251398.html)
-   [Creating Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1252880.html)
-   [Creating Billing Schedules From an Estimate or Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253492.html)
-   [Applying Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253848.html)
-   [Discount and Markup Items and Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254542.html)
-   [Billing Customers Using Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254744.html)
-   [Viewing Invoice Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256403.html)
-   [Advanced Billing and Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256787.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
