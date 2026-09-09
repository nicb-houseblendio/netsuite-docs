---
id: "bridgehead_N1319780"
type: "bridgehead"
title: "Support for Multiple Sales Channels"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Contract Renewals Overview > Support for Multiple Sales Channels"
parent: "section_4442063121"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1319780.html"
anchors: []
sha256: "79333eb7aabb1f29e58ef2d08031e40f5bef25a6e722bee198bb8205b3db140a"
---

The Software Vertical Contract Renewals SuiteApp enables you to track and manage multi-tiered sales interactions with distributors, resellers, and end users.

The Channel Tier field on the customer record defines the relationship each customer has with your company. Choose one of these:

-   **End User** - The end user is the customer who uses or registers the product. The end user may purchase the product from you or from a reseller or a distributor.
    
-   **Reseller** - The reseller purchases the product from you and resells it to an end user. The product can be delivered from you either through the reseller or directly to the end user.
    
-   **Distributor** - Distributors purchase from your company and sell the product to a reseller or end user. The distributor delivers the product and bills the purchaser.
    

Important:

Every end user of your products needs a customer record in your NetSuite account even if they purchase through a distributor or a reseller.

With Contract Renewals, these channels are managed through two fields on sales transactions: End User and Bill To Customer.

On the Channel subtab of the transaction form, do these steps:

-   If you're creating a contract for an end user who purchased through a reseller, on the Channel subtab of the transaction form, select the reseller or distributor for the transaction, and select Reseller in the Bill To Tier field.
    
-   If the contract is for an end user who purchased through a distributor, select Distributor in the Bill To Tier field.
    
-   Select the end user in the End User field.
    

Note:

For transactions submitted through SOAP web services, the SuiteApp throws an error if the Bill To Customer value isn't the same as either the End User, Reseller, or Distributor specified on the web service request. If a Distributor is specified on the request, the Bill To Tier field on the transaction is set to Distributor. If a Reseller is provided on the request instead of a Distributor, the Bill To Tier field on the transaction is set to Reseller. If neither Distributor nor Reseller is provided on the request, the Bill To Tier field on the transaction is set to End User.

If you've partners who sell your products, you can track them with partner records in your NetSuite account. You can associate partners with customers and with sales transactions. For more information, see [Associating Partners With Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167413.html).

A variety of channel-based reports are available on the Contract Renewals tab.

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
