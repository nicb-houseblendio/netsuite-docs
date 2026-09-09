---
id: "section_N2473533"
type: "section"
title: "Managing Customer Records with PayPal Express Checkout on Web Stores"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Web Store Transactions > Payment Options for Commerce Web Stores > PayPal Integration and Express Checkout for Commerce Web Stores > Managing Customer Records with PayPal Express Checkout on Web Stores"
parent: "section_N2470255"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2473533.html"
anchors: []
sha256: "c2aae382f80d6738ba4239933b98394c381695fba4eecb58233f9509d1d58c4d"
---

When you enable PayPal Express Checkout in NetSuite, a new customer record is created each time a shopper uses this payment method, regardless of whether they are a new or returning customer. This means that even if a shopper already has a customer record in your NetSuite account, checking out with PayPal Express will still generate an additional customer record.

Duplicate customer records show up in the list of customers with a number after the name. For example, Jane Smith and Jane Smith1.

To manage duplicates, turn on the Merge Duplicates feature (Setup > Enable Features > CRM). After you enable it, you can periodically run the duplicate merge operation from the Search menu.

Note:

If customers use PayPal Express Checkout before logging in or registering, a customer record is created. However, they don't get login or password information and can't access the Customer Center or My Account page.

### Related Topics

-   [PayPal Integration and Express Checkout for Commerce Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470255.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
