---
id: "section_N1743516"
type: "section"
title: "Contingent Revenue Handling"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > EITF 08-01 Revenue Recognition Feature > Contingent Revenue Handling"
parent: "chapter_N1742394"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743516.html"
anchors: []
sha256: "43594e2da147830e32234e0500baa3349b1f26785fc55a34691b4fcdd19f774e"
---

Important:

EITF 08-01 Revenue Recognition is a managed SuiteApp (Bundle ID: 29321).

The EITF 08-01 Revenue Recognition feature supports contingent revenue handling for professional service items. Contingent revenue handling stipulates that the allocated amount of revenue for delivered items can't be contingent on the delivery of additional items or other specified performance issues. This prevents over-allocating revenue for recognition purposes. It's applied when the ratio of the estimated selling price of professional services items on the sales order is greater than the ratio of the selling price of those items. When this occurs, the transaction is no longer considered a bundle, and revenue must be recognized based on the sales price of the items.

In the example below, the sales order includes subscription items and professional services.

|  | Order Value | VSOE/TPE/ESP | Preliminary Allocated Value | Final Allocated Value |
| --- | --- | --- | --- | --- |
| Subscription Items | $ 65,000 | $ 40,000 | $ 61,600 | $ 65,000 |
| Professional Services | **12,000** | 10, 000 | **15,400** | **12,000** |
| Total | $ 77,000 | $ 50,000 | $ 77,000 | $ 77,000 |
| PS Ratio | 16% | 20% | 20% | 16% |

Professional services are 16% of the total order (12,000 / 77,000). The ratio of the VSOE/ESP amount for professional services is 20% of the order (10,000 / 50,000). Using the VSOE/ESP ratio, the preliminary allocated revenue amount for professional services is $15,400. This amount exceeds the transaction amount of $12,000 and triggers contingent revenue handling. The transaction is no longer considered a bundle for revenue recognition, and the final revenue allocation for professional service is based on the sales order amount, $12,000.

To use contingent revenue handling, enable the Allow Contingent Revenue Handling preference at Setup > Company > General Preferences > Custom Preferences.

When you enable Contingent Revenue Handling, sales order transactions display the following fields:

-   **Contingent Revenue Handling Triggered** - is set to Yes when the ESP ratio of professional services is greater than the ratio of the selling price of those items. It indicates that the allocated value of the order is based on the sales order price to comply with contingent revenue handling rules.
    
-   **Contingent Revenue Handling Run** - is set to Yes upon saving an order that contains professional services items. It indicates that the ratios have been calculated for sales prices and ESP prices.
    

In addition, NetSuite displays a message alerting you that contingent revenue handling has been triggered and clears the Transaction is VSOE Bundle box.

### Related Topics

-   [EITF 08-01 Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1742394.html)
-   [Understanding EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1742630.html)
-   [EITF 08-01 Allocation Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743302.html)
-   [Contingent Revenue Handling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743516.html)
-   [About Installing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746114.html)
-   [Implementing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746357.html)
-   [Applying EITF 08-01 Scripts to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0806035426.html)
-   [Working with Estimated Selling Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1747534.html)
-   [How Can I Get This Feature?](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1749904.html)
-   [Revenue and Expense Recognition Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1675871.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
