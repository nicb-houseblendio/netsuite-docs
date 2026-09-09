---
id: "section_N1718126"
type: "section"
title: "Understanding VSOE Prices and Allocation"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > Understanding VSOE Prices and Allocation"
parent: "chapter_N1717900"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1718126.html"
anchors: []
sha256: "fa19478b2fa8f361dff6a8a66ea8760da03825009a4da90b7b387443989afb3b"
---

The items that your company sells as part of a bundle can have a vendor-specific objective evidence (VSOE) price. This price is based on its fair market value, in addition to an invoice price as part of the bundle. VSOE prices are assigned to items that are part of the bundle and dependent on each other. As you sell bundles, it's the VSOE price of each item in the bundle, not its invoice price, that is the revenue amount recognized for the sale. Using the VSOE price, you can recognize deferred revenue according to the fair value of the items in a bundle.

For example, you may sell software that requires an implementation service and a maintenance contract. In the following example, these three items sell for $20,000 as a bundle:

| Bundle Members | Invoice price | VSOE price |
| --- | --- | --- |
| Software, Product 099 | $10,000 | $8,000 |
| Professional Services, 100 hours | 8,000 | 10,000 |
| Maintenance, 1 year | 2,000 | 2,000 |
| Total | $20,000 | $20,000 |

If the sales amount of a bundle differs from the bundle's VSOE amount, each member item is assigned an amount to be recognized by allocating the total sales amount across all bundle member items.

Note:

To allocate amounts in a bundle, each item must have a VSOE amount on its item record. The system can't calculate the VSOE allocation if any item in a bundle doesn't have a VSOE value, and an error occurs.

The VSOE settings and statuses of an item determine the amount of revenue allocated and when it's recognized. These settings include the following:

-   When you sell a bundle, the revenue allocation may be delayed so that a schedule isn't created until appropriate conditions are met.
    
-   When the bundle is billed, the allocated value of the bundle is recognized according to the associated recognition schedule.
    

When the VSOE amount is properly allocated for an order and the order is billed, the revenue can be recognized for each item based on the revenue recognition schedule generated from the assigned revenue recognition template. See [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html) and [Working with Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689004.html).

### Related Topics

-   [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html)
-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Setting Up the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1718515.html)
-   [Creating VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1719451.html)
-   [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html)
-   [VSOE Revenue Recognition Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1736679.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
