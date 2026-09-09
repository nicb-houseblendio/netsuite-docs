---
id: "bridgehead_N1321133"
type: "bridgehead"
title: "Creating a Zero Price Item"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Setting Up Contract Renewals > Initial Setup Tasks for Contract Renewals > Creating a Zero Price Item"
parent: "section_N1321054"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1321133.html"
anchors: ["procedure_0118022732"]
sha256: "8b760ba73b1d7ccfce2ce34fe35d76e4fa405c40069ed4f2ffa90b85ec872fa8"
---

Zero price item is used by Contract Renewals to retrieve dynamic values when generating renewal transactions; but it isn't saved or added to any transactions. To make it work, you must set it up as an item that is available to all transactions in the account. For OneWorld accounts, the zero price item should be allowed on all subsidiaries.

#### To create a zero price item: {#procedure_0118022732}

1.  Go to _Lists > Accounting > Items > New (Administrator)_, and select the item type.
    
2.  In the **Item Name/Number** field, enter a name for the item.
    
3.  On the **Sales / Pricing** subtab, set the **Base Price** to **0**.
    
4.  For OneWorld accounts, select the root parent subsidiary in the **Subsidiary** field, and then check the **Include Children** box.
    
5.  Click **Save**.
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
