---
id: "section_N1226820"
type: "section"
title: "Automating the Ship Date"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Advanced Shipping > Automating the Ship Date"
parent: "section_N1224089"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1226820.html"
anchors: ["procedure_N1226838"]
sha256: "3c76f230bfb4a6eff4bcea9020282ab8c8d56fbfdc1071289eadd2ed9addbc1c"
---

By default, an order's ship date is the same date that the order was entered. You can set a preference to automatically set the ship date at a certain number of days after the order is entered.

For example, if you normally ship orders three days after the order is received, you can set an automated ship date for every order that is three days past the date the order is entered, including or excluding weekends and holidays.

When you fulfill the order, the real ship date is displayed in the Actual field next to the Ship Date field.

#### To set up automated ship dates: {#procedure_N1226838}

1.  Go to _Setup > Accounting > Shipping_.
    
2.  In the **Number of Days to Shipment** field, set the average number of days between the date a sales order is entered and the date the order is shipped. This number of days is added to the date of the order to set the ship date on sales orders. The actual ship date updates when the order is fulfilled.
    
    The ship date respects weekends and holidays unless you ship on Saturday or Sunday. You can set the holidays you observe on the **Preferences** subtab.
    
    For example, if you have estimated three days to shipment and do not ship Saturday or Sunday, orders entered on Friday have an estimated ship date of the following Wednesday.
    
3.  In the **Cutoff Time for Shipments** field, enter the time of day after which orders stop being shipped.
    
    Orders entered after this time begin counting days to shipment with the next business day.
    
4.  Check the **Ship on Saturday** box to include Saturday in the days to shipment calculation.
    
    For example, if you ship on Saturday and have 3 days to shipment for an order placed before the cutoff time on Friday, the order is estimated to ship on Tuesday.
    
5.  Check the **Ship on Sunday** box to include Sunday in the days to shipment calculation.
    
6.  Click **Submit**.
    

### Related Topics

-   [Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1257369.html)
-   [Creating Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216500.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
