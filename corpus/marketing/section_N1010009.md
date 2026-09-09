---
id: "section_N1010009"
type: "section"
title: "Limits on Upsell Manager Data"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Upsell Manager > Limits on Upsell Manager Data"
parent: "chapter_N1006631"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1010009.html"
anchors: []
sha256: "85054cad2fd56231311f8b0aef8bd74126aa2b1dbbbcfe81d45b5ad2b8c33ef3"
---

The amount of upsell data that NetSuite stores on your account depends on how many items or customers you have. NetSuite uses the larger of these two values to determine your allocation. The following table provides allocation examples.

| **Number of customers / items** | **Number of correlations / recommendations allowed** |
| --- | --- |
| <2000 | 100 |
| 5000 | 40 |
| 10000 | 20 |
| 25000 | 8 |
| 50000 | 4 |
| 100000 | 2 |

For accounts with more than 2000 items or customers, NetSuite calculates the maximum number of correlated items and customer recommendations by the following method:

1.  Determine the number of items or customers in your account and use the larger of these two values (for example, 4500 customers).
    
2.  Divide this number by 2000\* (4500 / 2000 = 2.25).
    
3.  Divide 100\*\* by the figure above (100 / 2.25 = 44).
    
4.  This value is the number of correlated items and customer recommendations NetSuite allocates to your account. For example, NetSuite allows an account with 4500 customers 44 recommendations per customer and 44 correlations per item.
    

\* the customer/items threshold.

\*\* the correlations/recommendations threshold.

### Related Topics

-   [Using the Upsell Manager Wizard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1008542.html)
-   [Upselling From Customer Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1009337.html)
-   [Upselling on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1009585.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
