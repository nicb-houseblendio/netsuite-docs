---
id: "section_N1226246"
type: "section"
title: "Fulfilling Orders Using Advanced Shipping with Advanced Billing"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Advanced Shipping > Fulfilling Orders Using Advanced Shipping with Advanced Billing"
parent: "section_N1224089"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1226246.html"
anchors: []
sha256: "eb13d4b3f5a69dc35819d02a956d3203ed0c7336068f3d6bd6b0fc31e8478e0d"
---

When you process orders using both the Advanced Billing and Advanced Shipping features, fulfillment forms function differently than when you do not use both of these features.

When you use both features and bulk fulfill orders by going to _Transactions > Order Management > Fulfill Orders_, the fulfillment list automatically filters out orders that do not include any fulfillable items. Orders that include both fulfillable items and non-fulfillable items show in the list only until all fulfillable items have been fulfilled.

The Fulfill button appears on orders only if the order includes fulfillable items with a remaining quantity to be fulfilled. When you click the Fulfill button, a new fulfillment opens that includes the remaining items.

Note:

When both the Advanced Shipping and Advanced Billing features are enabled, your setting for the Fulfill Based on Commitment preference does affect fulfillments.

Warning:

If this preference is set to Limit to Committed even though the Fulfill button is not available on an unfulfillable sales order, the order does show in the fulfillments list when the Filter By option is set to Ignore Item Availability. However, if you click the Fulfill link on this sales order, it cannot be fulfilled. You receive the message "There are no items committed in this transaction---it cannot be fulfilled."

Warning:

If the preference is set to Allow Uncommitted or Ignore Commitment: The Fulfill button shows on an unfulfillable sales order and it can be fulfilled by clicking the Fulfill button or by clicking on the Fulfill link beside the sales order at _Transactions > Order Management > Fulfill Orders_.

For detailed instructions on fulfilling an order, read [Fulfill a Single Order Using Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1224254.html).

### Related Topics

-   [Fulfill a Single Order Using Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1224254.html)
-   [Fulfill Multiple Orders Using Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1225980.html)
-   [Advanced Billing and Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256787.html)
-   [Billing Orders Using Advanced Shipping with Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1257068.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
