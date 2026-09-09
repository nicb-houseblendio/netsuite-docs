---
id: "section_N1743302"
type: "section"
title: "EITF 08-01 Allocation Example"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > EITF 08-01 Revenue Recognition Feature > EITF 08-01 Allocation Example"
parent: "chapter_N1742394"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743302.html"
anchors: []
sha256: "199a98f99a8e5dae1574fac6d5520be7f4844078f512552c65bbd88591934614"
---

Important:

EITF 08-01 Revenue Recognition is a managed SuiteApp (Bundle ID: 29321).

The chart below shows how EITF 08-01 Revenue Recognition allocates ESP amounts for revenue recognition.

![Screenshot of a chart that shows how revenue is allocated for EITF 08-01](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/RevenueExpenseRecognition/allocation.png)

In this example, the sales order has three typical items sold by a software company: a license for 12 months, a support contract, and a services contract for installation. The total order amount based on item prices is $47,200, and the three transaction items represent 76%, 3%, and 21% of the total order amount respectively.

The VSOE (ESP) amounts for the transaction lines are $28,800, $960, and $9,000. This is based on the estimated selling price for each item and the sales dimension combination identified for the order. EITF 08-01 Revenue Recognition feature calculates the VSOE (ESP) amounts upon saving the order. It determines the ratio of each item to the total VSOE (ESP) amount of the order. The percentages are 74.3%, 2.5%, and 23.2%. These percentages are then used to allocate how much of the total sales price of the order is to be recognized on each transaction line. The Allocation Amounts column shows the allocated amount that will be recognized using the revenue recognition schedule associated with the order.

For information about using price ranges with EITF 08-01 Revenue Recognition, see [Using Estimated Selling Price Ranges](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1747534.html#bridgehead_N1748877).

Note:

If using the M/S as a % of License revenue model, the Maintenance/Support transaction line items must always come after License - Term line items. For more information, see [Implementing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746357.html).

### Related Topics

-   [EITF 08-01 Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1742394.html)
-   [Understanding EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1742630.html)
-   [Contingent Revenue Handling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743516.html)
-   [About Installing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746114.html)
-   [Implementing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746357.html)
-   [Applying EITF 08-01 Scripts to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0806035426.html)
-   [Working with Estimated Selling Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1747534.html)
-   [How Can I Get This Feature?](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1749904.html)
-   [Revenue and Expense Recognition Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1675871.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
