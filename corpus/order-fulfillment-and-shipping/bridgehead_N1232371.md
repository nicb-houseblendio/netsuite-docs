---
id: "bridgehead_N1232371"
type: "bridgehead"
title: "Email Templates for OneWorld Accounts that Support Multiple Languages"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Order Fulfillment Confirmation Email > Email Templates for OneWorld Accounts that Support Multiple Languages"
parent: "section_N1231778"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1232371.html"
anchors: []
sha256: "5ec75583a532cce5826a41a01cc3274e41eac773caed27ee1ce29270a0c9d284"
---

In OneWorld accounts with multiple languages, checking the Use Web Site Template for Fulfillment Emails box might not always result in all fulfillment email messages using the same customized web site text group because of dependencies on language preferences. See [Using Web Site Text Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2609031.html) for more information about customized web site text group.

Note the following:

-   If you check the **Use Web Site Template For Fulfillment Emails** box, the text specified on the Custom Web Site Text page is used for fulfillment email messages, sent for sales orders entered from the Transactions tab in NetSuite. However, fulfillment email messages, sent for web store order, do not use this text. It is no longer possible to use the same email template for fulfilment emails for orders from both sources. For information about customizing and sending fulfillment email for web store orders, see [Templates for Website Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530715267.html).
    
-   A user's language preference defaults to the language that is configured for the user's subsidiary at _Setup > Company > Classifications > Subsidiaries_.
    
-   Each customized web site text group for order fulfillment has a locale (preferred language) defined, and this locale may differ from the locale set for some customers. Any customer that has a locale different from that of the customized web site text group cannot use the customized web site text group.
    

Important:

When using customized web site text groups for order fulfillments, verify that a customized web site text group has been created for every language used by customers. If a customized web site text group with a matching language is not found for a customer, that customer's orders default to using the standard order status email message.

### Related Topics:

-   [Fulfilling Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1223349.html)
-   [Order Fulfillment Confirmation Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231778.html)
-   [Sending Order Fulfillment Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231841.html)
-   [Templates for Website Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530715267.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
