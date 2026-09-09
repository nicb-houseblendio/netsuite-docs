---
id: "section_N1688873"
type: "section"
title: "Delaying Revenue Recognition for an Item"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Associating Revenue Recognition Templates with Items > Delaying Revenue Recognition for an Item"
parent: "section_N1687451"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1688873.html"
anchors: []
sha256: "e3c859c2a0cfb2caba757a2f6afefdfc8abd5df957073035d72765ad5c657632"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For equivalent information about the current feature, see [Item Configuration for Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4340443927.html).

You can choose to delay posting from a revenue recognition schedule by putting it on hold. You may want to do this if, for example, delivery is delayed or your ability to collect payment becomes uncertain. When a schedule is on hold, the total balance of the delayed item remains in the Deferred Revenue account until you cancel the hold.

Revenue recognition can be delayed for any item that has a deferred revenue account identified on its item record, regardless of whether it has a revenue recognition schedule. If the **Hold Revenue Recognition** box is checked for such an item, when the delay is canceled, all revenue for the item is immediately recognized.

You can set Hold Revenue Recognition on an item record. This setting becomes the default for all sales of the item.

#### To set Hold Revenue Recognition for an item:

1.  Go to _Lists > Accounting > Items_, and click **Edit** next to an item.
    
2.  In the Item record, click the **Accounting** subtab and ensure that an account is selected in the **Deferred Revenue Account** field.
    
    This field must be populated for revenue recognition to be available for an item on transactions.
    
3.  Click the **Revenue Recognition / Amortization** subtab, and check the **Hold Revenue Recognition** box.
    
4.  Click **Save**.
    

### Related Topics

-   [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html)
-   [Managing Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4029604484.html)
-   [Associating Revenue Recognition Templates with Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687451.html)
-   [Setting a Revenue Recognition Template on an Item Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687732.html)
-   [Setting a Revenue Recognition Template on a Transaction Item Line](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1688475.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
