---
id: "section_N1687732"
type: "section"
title: "Setting a Revenue Recognition Template on an Item Record"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Associating Revenue Recognition Templates with Items > Setting a Revenue Recognition Template on an Item Record"
parent: "section_N1687451"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687732.html"
anchors: ["procedure_N1687745"]
sha256: "342e4770fca35c42c186882c47ca6a631324d69dfa9e84991b7d59924c4146f3"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For equivalent information about the current feature, see [Item Configuration for Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4340443927.html).

You can set a revenue recognition template on an item record. This template becomes the default for all sales of the item.

#### To select a default revenue recognition template for an item: {#procedure_N1687745}

1.  Go to _Lists > Accounting > Items_, and click **Edit** next to an item.
    
2.  In the Item record, click the **Accounting** subtab.
    
3.  Ensure that an account is selected in the **Deferred Revenue Account** field.
    
    This field must be populated for revenue recognition to be available for an item on transactions.
    
4.  Click the **Revenue Recognition / Amortization** subtab, and select a template in the **Revenue Recognition Template** list.
    
5.  Click **Save**.
    

Now the item is associated with the revenue recognition template and the item defaults to use the template when it's sold. You can change the revenue recognition template on individual transaction lines as needed. See [Setting a Revenue Recognition Template on a Transaction Item Line](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1688475.html).

On the item record, you can also set the default to delay posting from the schedule that's created for the item. See [Delaying Revenue Recognition for an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1688873.html).

### Related Topics

-   [Associating Revenue Recognition Templates with Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687451.html)
-   [Setting a Revenue Recognition Template on a Transaction Item Line](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1688475.html)
-   [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html)
-   [Deferring Revenue for Discount and Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1688734.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
