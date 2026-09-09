---
id: "section_N2473428"
type: "section"
title: "Authorization and Capture with PayPal Express Checkout on Web Stores"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Web Store Transactions > Payment Options for Commerce Web Stores > PayPal Integration and Express Checkout for Commerce Web Stores > Authorization and Capture with PayPal Express Checkout on Web Stores"
parent: "section_N2470255"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2473428.html"
anchors: []
sha256: "409ff4e834f52887623cc0d4aa466581c29c6bde1905b74c5e63da29027a8b42"
---

After an order is created, NetSuite initiates an authorization request to PayPal for the full order amount. When the shopper approves the authorization, a three-day honor period starts. PayPal holds the order amount on the shopper's account to make sure funds are available for capture.

During this three-day honor period, you're guaranteed to capture funds if the authorization is valid. Contact PayPal for more information about their validation process.

You've got three days from when the order's created to fulfill it and capture the funds. If you try to capture funds after the three-day period, NetSuite voids the original authorization, starts a new one, and tries to capture the funds again. By default your PayPal account is restricted to a single authorization. NetSuite can initiate only as many authorizations as your PayPal account allows within a 29-day period.

Important:

Your PayPal account manager can tell you how many authorizations are allowed in your account and increase the limit if needed.

### Related Topics

-   [PayPal Integration and Express Checkout for Commerce Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470255.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
