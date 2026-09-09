---
id: "section_N1767540"
type: "section"
title: "Specifying Deferral Accounts for Amortization"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Setup for Amortization > Specifying Deferral Accounts for Amortization"
parent: "section_N1766651"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767540.html"
anchors: ["bridgehead_N1767581", "bridgehead_N1767611", "bridgehead_N1767642", "procedure_N1767654"]
sha256: "fee6a2c265e2374e33c244bcf5f9a2f13de9b92c43cc362eb4426e7aae739825"
---

Deferred expenses must be posted to a deferral account until they're shifted to an expense account by amortization journal entries based on the amortization schedule. If you don't specify a deferral account, amortization isn't possible. Accounts of the type Deferred Expense are included as Other Current Assets on the balance sheet.

For an item, a deferral account must be specified either on the item record or on the associated template record. Costs for this item on a vendor bill or credit can then be amortized if the item has an associated amortization template on the item record or transaction line.

For an expense charge, a deferral account must be specified on the expense account record or the associated template record. Costs for an expense line on a vendor bill or credit can then be amortized if the expense has an associated amortization template on the transaction line.

Important:

The deferral account specified in an amortization template takes precedence over a deferral account specified in an item record and over a deferral account specified in an expense account record.

If you change the deferral account, the change applies only to new amortization schedules. Existing amortization schedules and amortization journal entries don't change.

Note:

Use GL Impact to view the deferral account posted for a transaction line. On the transaction, the expense line displays the target account.

## Specifying a Deferral Account on an Amortization Template {#bridgehead_N1767581}

For information about specifying a deferral account in an amortization template, see [Amortization Template Term Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1768001.html) and [Creating Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1772949.html).

## Specifying a Deferral Account on an Item Record {#bridgehead_N1767611}

You can specify a deferral account on an item record in the Deferred Expense Account field on the Accounting subtab. Only the following types of items support amortization:

-   Non-inventory Item for Purchase/Resale
    
-   Other Charge for Purchase/Resale
    
-   Service for Purchase/Resale
    

#### To specify the deferral account on an item record:

1.  Go to _Lists > Accounting > Items_, and click **Edit** next to an item.
    
2.  In the item record, click the **Accounting** subtab, and select an account in the **Deferred Expense Account** field.
    
3.  Click **Save**.
    

For other steps required to configure an item for amortization, see [Setting an Amortization Template on an Item Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773719.html).

## Specifying a Deferral Account on an Expense Account {#bridgehead_N1767642}

You can specify a deferral account on Expense, Other Expense, and Cost of Goods Sold types of general ledger accounts.

#### To set up a general ledger account for amortization expense: {#procedure_N1767654}

1.  Go to _Lists > Accounting > Accounts_.
    
2.  In the Chart of Accounts page, click **Edit** next to the account you want to set up.
    
3.  In the **Deferral Account** field, select the deferred expense account you want to use.
    
4.  Click **Save**.
    

Now, when you use this expense account, amounts are deferred to the appropriate account.

### Related Topics

-   [Setup for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1766651.html)
-   [Enabling the Amortization Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1766842.html)
-   [Setting Amortization Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767069.html)
-   [Enabling Auto-Numbered Amortization Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767306.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
