---
id: "section_N1773719"
type: "section"
title: "Setting an Amortization Template on an Item Record"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Amortization Templates > Configuration for Amortization > Setting an Amortization Template on an Item Record"
parent: "section_N1773475"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773719.html"
anchors: ["procedure_N1773738"]
sha256: "6a90dcf76bdb636b192233761d6c140b8f50f28531d71f42be6539676213a93e"
---

You can set an amortization template on an item record. This template becomes the default for all purchases of the item.

#### To set up amortization on an item record: {#procedure_N1773738}

1.  Go to _Lists > Accounting > Items_, and click **Edit** next to an item.
    
    Only the following types of items can use amortization: Non-Inventory for Purchase/Resale, Other Charge for Purchase/Resale, and Service for Purchase/Resale.
    
2.  In the item record, click the **Accounting** subtab, and select an account in the **Deferred Expense Account** field.
    
    This enables the purchase amount to be posted to a deferred expense account instead of a standard expense account.
    
    Deferral accounts also can be specified in amortization template records. See [Specifying Deferral Accounts for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767540.html).
    
3.  Click the **Revenue Recognition / Amortization** subtab and complete the following fields:
    
    1.  Select a template in the **Amortization Template** list.
        
        This template is used by default on transactions. You can select a different template when you create the transaction.
        
    2.  In the **Residual** field, enter an amount or percentage to remain in the deferral account and not be amortized. A residual amount generally represents the salvage value of a fixed asset.
        
        A residual amount entered on a transaction overrides a residual amount entered on an item record.
        
    3.  In the **Amortization Period** field, enter the number of periods over which the purchase amount should be amortized. For example, enter **60** to amortize the amount over 60 periods starting from the amortization start date.
        
        The starting period is specified by the amortization start date on bills. If no amortization start date is specified, the posting date of the bill is the amortization start date.
        
4.  Click **Save**.
    

The item defaults to use the assigned template to generate an amortization schedule when it's billed or credited. You can change the amortization template on individual transaction lines. See [Setting an Amortization Template on a Vendor Bill Line Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773966.html) and [Setting an Amortization Template on a Vendor Credit Line Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1774211.html).

### Related Topics

-   [Configuration for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773475.html)
-   [Setting an Amortization Template on a Vendor Bill Line Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773966.html)
-   [Setting an Amortization Template on a Vendor Credit Line Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1774211.html)
-   [Vendor Credit Amortization Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1774542.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
